# Traffic_Flow_Analysis
🚦 Lane-wise Traffic Vehicle Counter using YOLOv8
A Google Colab–ready AI system to detect, track, and count vehicles lane by lane in real time using YOLOv8 and OpenCV.
Counts are triggered only when a vehicle crosses a virtual line in its lane preventing duplicate counts .

📌 Features
 Detects cars, buses, trucks, motorcycles
 Tracks vehicles using IoU + Hungarian algorithm
 Counts only on line crossing in the correct lane
 Exports results to CSV (Vehicle ID, Lane, Timestamp)

🎥 Produces an overlay video with live counts & bounding boxes
☁ Runs fully in Google Colab
| Tool              | Purpose                             |
| ----------------- | ----------------------------------- |
| **YOLOv8**        | Vehicle detection                   |
| **OpenCV**        | Video processing & drawing overlays |
| **NumPy / SciPy** | Tracker & math                      |
| **yt-dlp**        | YouTube video download in Colab     |

🚀 How It Works
Input Video → https://youtu.be/MNn9qKG2UFI?si=2Ri4dRrgg_aj5egb

YOLOv8 Detection → Finds vehicles in each frame.
Tracking → Matches vehicles across frames using IoU & Hungarian method.

Counting →
Each lane has a counting line; 
vehicle is counted once when centroid crosses the line.

Overlay Video:
Red lines = counting lines
Green/Orange boxes = tracked vehicles
Top-left = lane counts in real time

💡 Use Cases
Smart city traffic monitoring
Lane usage analytics
Accident detection & traffic management
Adaptive traffic signal control



