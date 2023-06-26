# Loudness filter (normalize audio)

- package: ``easyeffects``

```json
{
    "output": {
        "blocklist": [],
        "compressor#1": {
            "attack": 30.0,
            "boost-amount": 10.0,
            "boost-threshold": -100.0,
            "bypass": false,
            "dry": -100.0,
            "hpf-frequency": 120.0,
            "hpf-mode": "36 dB/oct",
            "input-gain": 0.0,
            "knee": -4.0,
            "lpf-frequency": 2518.0,
            "lpf-mode": "off",
            "makeup": 0.0,
            "mode": "Downward",
            "output-gain": 0.0,
            "ratio": 8.0,
            "release": 100.0,
            "release-threshold": -100.0,
            "sidechain": {
                "lookahead": 5.0,
                "mode": "Peak",
                "preamp": 10.0,
                "reactivity": 10.0,
                "source": "Middle",
                "type": "Feed-forward"
            },
            "threshold": -12.0,
            "wet": 0.0
        },
        "compressor#2": {
            "attack": 1.0,
            "boost-amount": 20.0,
            "boost-threshold": -100.0,
            "bypass": false,
            "dry": -100.0,
            "hpf-frequency": 632.0,
            "hpf-mode": "off",
            "input-gain": 0.0,
            "knee": -8.0,
            "lpf-frequency": 5024.0,
            "lpf-mode": "off",
            "makeup": 10.0,
            "mode": "Upward",
            "output-gain": 0.0,
            "ratio": 1.0,
            "release": 90.0,
            "release-threshold": -100.0,
            "sidechain": {
                "lookahead": 5.0,
                "mode": "Peak",
                "preamp": 0.0,
                "reactivity": 100.0,
                "source": "Middle",
                "type": "Feed-forward"
            },
            "threshold": -6.0,
            "wet": -4.0
        },
        "equalizer#0": {
            "balance": 0.0,
            "bypass": true,
            "input-gain": 0.0,
            "left": {
                "band0": {
                    "frequency": 10.0,
                    "gain": 2.57,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.650449464127273,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band1": {
                    "frequency": 21.0,
                    "gain": 4.12,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band2": {
                    "frequency": 42.0,
                    "gain": 5.15,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band3": {
                    "frequency": 83.0,
                    "gain": 3.6,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band4": {
                    "frequency": 166.0,
                    "gain": 3.57,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band5": {
                    "frequency": 333.0,
                    "gain": 1.73,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.650449464127276,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band6": {
                    "frequency": 577.0,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.650449464127273,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band7": {
                    "frequency": 1000.0,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                }
            },
            "mode": "IIR",
            "num-bands": 8,
            "output-gain": 0.0,
            "pitch-left": 0.0,
            "pitch-right": 0.0,
            "right": {
                "band0": {
                    "frequency": 10.0,
                    "gain": 2.57,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.650449464127273,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band1": {
                    "frequency": 21.0,
                    "gain": 4.12,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band2": {
                    "frequency": 42.0,
                    "gain": 5.15,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band3": {
                    "frequency": 83.0,
                    "gain": 3.6,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band4": {
                    "frequency": 166.0,
                    "gain": 3.57,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band5": {
                    "frequency": 333.0,
                    "gain": 1.73,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.650449464127276,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band6": {
                    "frequency": 577.0,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.650449464127273,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band7": {
                    "frequency": 1000.0,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 4.6504494641272744,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                }
            },
            "split-channels": false
        },
        "limiter#1": {
            "alr": false,
            "alr-attack": 30.0,
            "alr-knee": -2.0,
            "alr-release": 60.0,
            "attack": 1.0,
            "bypass": true,
            "dithering": "None",
            "external-sidechain": false,
            "gain-boost": false,
            "input-gain": 0.0,
            "lookahead": 5.0,
            "mode": "Herm Thin",
            "output-gain": 0.0,
            "oversampling": "None",
            "release": 20.0,
            "sidechain-preamp": 0.0,
            "stereo-link": 100.0,
            "threshold": -8.0
        },
        "limiter#2": {
            "alr": false,
            "alr-attack": 10.0,
            "alr-knee": -4.0,
            "alr-release": 50.0,
            "attack": 5.0,
            "bypass": false,
            "dithering": "None",
            "external-sidechain": false,
            "gain-boost": false,
            "input-gain": 0.0,
            "lookahead": 5.0,
            "mode": "Herm Thin",
            "output-gain": 0.0,
            "oversampling": "None",
            "release": 5.0,
            "sidechain-preamp": 0.0,
            "stereo-link": 100.0,
            "threshold": -4.0
        },
        "plugins_order": [
            "compressor#2",
            "equalizer#0",
            "compressor#1",
            "limiter#1",
            "limiter#2"
        ]
    }
}
```
