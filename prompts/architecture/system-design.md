
# System Design Prompt

## Prompt

"Design a system for a homelab that allows a user to upload a video file, have it automatically transcoded to different resolutions (e.g., 1080p, 720p, 480p), and then make it available for streaming.

The system should be:
- **Asynchronous:** The transcoding process should happen in the background without blocking the user.
- **Scalable:** The system should be able to handle multiple video uploads and transcoding jobs at the same time.
- **Resilient:** The system should be able to recover from failures during the transcoding process.

Please provide a high-level system design diagram and describe the components of the system and how they interact with each other.

Consider using the following technologies:
- A web server to handle file uploads.
- A message queue (e.g., RabbitMQ, Redis Queue) to manage transcoding jobs.
- A fleet of worker nodes to perform the transcoding (e.g., using FFmpeg).
- A storage solution to store the original and transcoded video files (e.g., a NAS, MinIO).
- A media server (e.g., Plex, Jellyfin) to stream the transcoded videos."
