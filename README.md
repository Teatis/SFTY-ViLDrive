# README

## Abstract
Identifying risky driving behavior in real-world situations is essential for the safety of both drivers and pedestrians. However, integrating natural language models in this field remains relatively untapped. To address this, we created a novel multi-modal instruction tuning dataset and driver coaching inference system. Our primary use case is dashcam-based coaching for commercial drivers. The North American Dashcam Market is expected to register a CAGR of 15.4% from 2022 to 2027.

Our dataset enables language models to learn visual instructions across various risky driving scenarios, emphasizing detailed reasoning crucial for effective driver coaching and managerial comprehension. The model is trained on road-facing and driver-facing RGB camera footage, capturing the comprehensive scope of driving behavior in vehicles equipped with dashcams.

## Example JSON Structure

```json
{
  "id": 762,
  "video": "1154511278.mp4",
  "conversations": [
    {
      "from": "human",
      "value": "What is happening in the video?"
    },
    {
      "from": "gpt",
      "value": "You were driving at a speed of 28 mph when you reached for your cell phone."
    },
    {
      "from": "human",
      "value": "What is the recommended action for the ego-car?"
    },
    {
      "from": "gpt",
      "value": "Using a cell phone while driving can significantly distract you and increase the risk of an accident. Please refrain from using your phone and focus on the road to ensure your safety and the safety of others."
    }
  ]
}
