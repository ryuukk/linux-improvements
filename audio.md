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
            "hpf-frequency": 8000.0,
            "hpf-mode": "off",
            "input-gain": 0.0,
            "knee": -6.0,
            "lpf-frequency": 11000.0,
            "lpf-mode": "off",
            "makeup": 0.0,
            "mode": "Boosting",
            "output-gain": 0.0,
            "ratio": 2.0,
            "release": 140.0,
            "release-threshold": -100.0,
            "sidechain": {
                "lookahead": 5.0,
                "mode": "RMS",
                "preamp": -10.0,
                "reactivity": 10.0,
                "source": "Middle",
                "type": "Feed-forward"
            },
            "threshold": -10.0,
            "wet": -4.0
        },
        "compressor#2": {
            "attack": 30.0,
            "boost-amount": 6.0,
            "boost-threshold": -72.0,
            "bypass": true,
            "dry": -100.0,
            "hpf-frequency": 10.0,
            "hpf-mode": "off",
            "input-gain": 0.0,
            "knee": 0.0,
            "lpf-frequency": 20000.0,
            "lpf-mode": "off",
            "makeup": 0.0,
            "mode": "Downward",
            "output-gain": 0.0,
            "ratio": 2.0,
            "release": 600.0,
            "release-threshold": -100.0,
            "sidechain": {
                "lookahead": 5.0,
                "mode": "RMS",
                "preamp": 10.0,
                "reactivity": 10.0,
                "source": "Middle",
                "type": "Feed-forward"
            },
            "threshold": -10.0,
            "wet": -2.0
        },
        "equalizer#0": {
            "balance": 0.0,
            "bypass": false,
            "input-gain": 0.0,
            "left": {
                "band0": {
                    "frequency": 33.71373705661655,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.229195839085688,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band1": {
                    "frequency": 79.94786957565145,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.229195839085688,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band2": {
                    "frequency": 189.58627573536728,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.2291958390856883,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band3": {
                    "frequency": 449.57990923317016,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.2291958390856883,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band4": {
                    "frequency": 1066.1219753492933,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.2291958390856883,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band5": {
                    "frequency": 2528.173619371377,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.229195839085688,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band6": {
                    "frequency": 5995.2444443247405,
                    "gain": -1.96,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.2291958390856883,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band7": {
                    "frequency": 14216.965034285808,
                    "gain": -1.96,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.229195839085688,
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
                    "frequency": 33.71373705661655,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.229195839085688,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band1": {
                    "frequency": 79.94786957565145,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.229195839085688,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band2": {
                    "frequency": 189.58627573536728,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.2291958390856883,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band3": {
                    "frequency": 449.57990923317016,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.2291958390856883,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band4": {
                    "frequency": 1066.1219753492933,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.2291958390856883,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band5": {
                    "frequency": 2528.173619371377,
                    "gain": 0.0,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.229195839085688,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band6": {
                    "frequency": 5995.2444443247405,
                    "gain": -1.96,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.2291958390856883,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                },
                "band7": {
                    "frequency": 14216.965034285808,
                    "gain": -1.96,
                    "mode": "RLC (BT)",
                    "mute": false,
                    "q": 1.229195839085688,
                    "slope": "x1",
                    "solo": false,
                    "type": "Bell"
                }
            },
            "split-channels": false
        },
        "limiter#1": {
            "alr": true,
            "alr-attack": 30.0,
            "alr-knee": -2.0,
            "alr-release": 100.0,
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
            "threshold": -6.0
        },
        "plugins_order": [
            "compressor#1",
            "compressor#2",
            "equalizer#0",
            "limiter#1"
        ]
    }
}

```
