
## Questions

#### 1. What is the primary function of E142? Is it only used for uploading and downloading maps?

#### 2. Does E142 rely on ALPS? Can E142 be used independently without an ALPS license?

#### 3. If only E142 is used without ALPS, does E142 have basic format conversion functionality? Can it convert other types of maps into the E142 standard protocol .xml format? If not, which specific format conversions does it support? Or, does it reduce any conversion work?

#### 4. When using only E142 for uploading and downloading maps, which map formats need to be compatible? Are these formats limited to Ascii, Decimal, Hexadecimal, and Integer2?

- Source: Cimetrix

![](https://easyimage.ghuang.top/i/2024/09/05/103709-1.webp)

#### 5. What map format conversions does ALPS support? Does it support the formats listed in the table below?

- Source: Internet
![](https://easyimage.ghuang.top/i/2024/09/05/135605-1.webp)

#### 6. How to select the final software configuration?

  - Optional configurations: SECS/GEM, E142, ALPS
  - E142: Primarily used for map uploading and downloading.
  - ALPS: Supports map visualization, format conversion, editing, and traceability features.

  **Configuration options:**

  - 6.1 Basic version
  - 6.2 Basic version + SECS/GEM (VRO)
  - 6.3 Basic version + SECS/GEM + E142
  - 6.4 Basic version + SECS/GEM + ALPS (supports map format conversion)
  - 6.5 Basic version + SECS/GEM + E142 + ALPS

#### 7. How to use ALPS to create and edit maps?

- Source: Cimetrix
![](https://easyimage.ghuang.top/i/2024/09/05/142426-1.webp)

## Development Steps

### I. E142 Upload and Download

#### 1. E142.2 is suitable for projects sending data less than 16MB. (Older version of the protocol, sufficient for most scenarios)
- S14, F1/F2 
- S6, F11/F12

| Service Name  | Stream, Function | SECS II Message Name                         |
| ------------- | ---------------- | -------------------------------------------- |
| MapDownload   | S14, F1/2        | Object Service (SEMI E39.1) – GetAttr Request/GetAttr Data |
| MapUpload     | S6, F11          | Data Collection (SEMI E5) – Event Report Sent |

#### 2. E142.4 is suitable for projects sending data larger than 16MB (New version of the protocol, supports more features, sufficient for all scenarios)
- S21 F1/F2
- S21 F3/F4
- S21 F5/F6
- S21 F15/F16
- S21 F17/F18

- **Device Upload/Download** ✔️
- **Host-initiated Retrieval** ❌ (rarely used)

| **Service Name**          | **Stream, Function**       | **SECS II Message Name**                                                                                                                | **Support Status**                                                                                     |
| ------------------------- | -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| **MapDownload**           | Device-initiated single message | S21F5/6: The device sends a S21F5 request for map data. If accepted, the host responds with map data in S21F6.                        | ✔️                                                                                                       |
|                           | Device-initiated multiple messages | S21F15/16 and S21F17/18: The device sends a S21F15 request for map data. If accepted, the host sends the map data through S21F17.    | ✔️                                                                                                       |
|                           | Host-initiated single message   | S21F1/F2 and S21F3/F4: The host sends a S21F1 request to permit the device to send map data. If accepted, the host sends the map data in S21F3. | ❌                                                                                                       |
|                           | Host-initiated multiple messages | S21F13/14 and S21F17/18: The host sends a S21F13 request to permit the device to send map data. If accepted, the host sends the map data through S21F17. | ❌                                                                                                       |
| **MapUpload**             | Device-initiated single message | S21F1/F2 and S21F3/F4: The device sends a S21F1 request to send map data. If accepted, the device sends the map data in S21F3.         | ✔️                                                                                                       |
|                           | Device-initiated multiple messages | S21F13/14 and S21F17/18: The device sends a S21F13 request to send map data. If accepted, the device sends the map data through S21F17. | ✔️                                                                                                       |
|                           | Host-initiated single message   | S21F5/6: The host requests map data via S21F5. If accepted, the device returns the map data in S21F6.                                    | ❌                                                                                                       |
|                           | Host-initiated multiple messages | S21F15/16 and S21F17/18: The host requests map data via S21F15. If accepted, the device sends the map data through S21F17.             | ❌                                                                                                       |

### II. Map Visualization

- Use ALPS to generate the corresponding Map.xml file based on the device, import it into the demo for testing, and verify the accuracy of the coordinate output using map animation.

#### 1. StripMap (Clip)
#### 2. WaferMap
#### 3. TransferMap (Strip + Wafer) (Die)

![](https://easyimage.ghuang.top/i/2024/09/04/165539-1.webp)

### III. Integration into Existing Software

- After completing map visualization tests, integrate the map functionality into the equipment.
- During the early stages of development, it's essential to select the appropriate configuration (SECS/GEM, E142, ALPS), as this impacts both cost and software architecture. Changing the architecture later may lead to software instability and increased development effort.

#### 1. Die (Add StripMap)
#### 2. Clip (Add TransferMap)