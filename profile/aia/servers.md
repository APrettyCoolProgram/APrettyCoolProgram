# Servers

## Raider

```json
[
  {
    "modelCompatibilityType": "gguf",
    "runtime": {
      "hardwareSurveyResult": {
        "compatibility": {
          "status": "compatible"
        },
        "cpuSurveyResult": {
          "result": {
            "code": "Success",
            "message": ""
          },
          "cpuInfo": {
            "name": "Intel(R) Core(TM) i7-10700K CPU @ 3.80GHz",
            "architecture": "x86_64",
            "supportedInstructionSetExtensions": [
              "AVX",
              "AVX2"
            ]
          }
        },
        "memoryInfo": {
          "ramCapacity": 34274566144,
          "vramCapacity": 12878086144,
          "totalMemory": 47152652288
        },
        "gpuSurveyResult": {
          "result": {
            "code": "Success",
            "message": ""
          },
          "gpuInfo": [
            {
              "name": "NVIDIA GeForce RTX 4070",
              "deviceId": 0,
              "totalMemoryCapacityBytes": 12878086144,
              "dedicatedMemoryCapacityBytes": 12878086144,
              "integrationType": "Discrete",
              "detectionPlatform": "CUDA",
              "detectionPlatformVersion": "",
              "otherInfo": {
                "deviceUUID": "8ed5757e3f7cf1177766e79c8d8e7f69",
                "computeCapability": "8.9",
                "driverVersion": "13010"
              }
            }
          ]
        }
      }
    }
  }
]
```


## Surface Pro 8 (i7-1185G7, 16GB RAM)

```json
[
  {
    "modelCompatibilityType": "gguf",
    "runtime": {
      "hardwareSurveyResult": {
        "compatibility": {
          "status": "compatible"
        },
        "cpuSurveyResult": {
          "result": {
            "code": "Success",
            "message": ""
          },
          "cpuInfo": {
            "name": "11th Gen Intel(R) Core(TM) i7-1185G7 @ 3.00GHz",
            "architecture": "x86_64",
            "supportedInstructionSetExtensions": [
              "AVX",
              "AVX2"
            ]
          }
        },
        "memoryInfo": {
          "ramCapacity": 17014194176,
          "vramCapacity": 8507097088,
          "totalMemory": 25521291264
        },
        "gpuSurveyResult": {
          "result": {
            "code": "Success",
            "message": ""
          },
          "gpuInfo": [
            {
              "name": "Intel(R) Iris(R) Xe Graphics",
              "deviceId": 0,
              "totalMemoryCapacityBytes": 8507097088,
              "dedicatedMemoryCapacityBytes": 8507097088,
              "integrationType": "Integrated",
              "detectionPlatform": "Vulkan",
              "detectionPlatformVersion": "1.3.283",
              "otherInfo": {
                "deviceLUIDValid": "true",
                "deviceLUID": "582f010000000000",
                "deviceUUID": "8680499a010000000002000000000000",
                "driverID": "5",
                "driverName": "Intel Corporation",
                "driverInfo": "101.6737",
                "vendorID": "32902"
              }
            }
          ]
        }
      }
    }
  }
]
```
