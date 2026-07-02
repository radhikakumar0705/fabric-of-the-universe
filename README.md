# Event Horizon: Schwarzschild Raytracer
This project is a real-time, relativistic raytracer that simulates the appearance of an accretion disk around a non-rotating black hole using the Schwarzschild metric. Every pixel integrates light trajectories frame-by-frame through curved spacetime, calculating gravitational lensing, gravitational redshift, and Doppler beaming directly on the GPU.

## Technical Overview
Raymarching & Integration: Uses a custom WebGL fragment shader to step photons through the geodesic equations of a Schwarzschild mass, rather than using traditional linear rasterization.

Dynamic Performance Scaling: Switches between high-step/high-resolution configurations during idle states and lower-overhead configurations during viewport manipulation to maximize interface responsiveness.

Dynamic Resolution Scaling: Monitors continuous frame-render intervals to dynamically alter internal drawing buffer boundaries to target consistent refresh rates.
