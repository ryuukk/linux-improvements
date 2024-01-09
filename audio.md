# Loudness filter (normalize audio)

- package: ``easyeffects``

```json
{
    "output": {
        "blocklist": [],
        "compressor#1": {
            "attack": 13.938555717468262,
            "boost-amount": 6.0,
            "boost-threshold": -72.0,
            "bypass": true,
            "dry": -100.0,
            "hpf-frequency": 112.6872787475586,
            "hpf-mode": "off",
            "input-gain": 0.0,
            "knee": -12.0,
            "lpf-frequency": 4045.922119140625,
            "lpf-mode": "off",
            "makeup": 0.0,
            "mode": "Downward",
            "output-gain": 0.0,
            "ratio": 3.172457218170166,
            "release": 200.0,
            "release-threshold": -100.0,
            "sidechain": {
                "lookahead": 0.0,
                "mode": "RMS",
                "preamp": 0.0,
                "reactivity": 20.0,
                "source": "Middle",
                "stereo-split-source": "Left/Right",
                "type": "Feed-forward"
            },
            "stereo-split": false,
            "threshold": -24.0,
            "wet": 0.0
        },
        "compressor#2": {
            "attack": 20.0,
            "boost-amount": 7.999999523162842,
            "boost-threshold": -60.0,
            "bypass": false,
            "dry": -100.0,
            "hpf-frequency": 2000.0,
            "hpf-mode": "off",
            "input-gain": 0.0,
            "knee": -14.000000953674316,
            "lpf-frequency": 800.0,
            "lpf-mode": "off",
            "makeup": 0.0,
            "mode": "Boosting",
            "output-gain": 0.0,
            "ratio": 2.0,
            "release": 100.0,
            "release-threshold": -100.0,
            "sidechain": {
                "lookahead": 5.0,
                "mode": "RMS",
                "preamp": 0.0,
                "reactivity": 100.0,
                "source": "Middle",
                "stereo-split-source": "Left/Right",
                "type": "Feed-forward"
            },
            "stereo-split": false,
            "threshold": -18.0,
            "wet": 0.0
        },
        "limiter#0": {
            "alr": false,
            "alr-attack": 5.0,
            "alr-knee": 0.0,
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
            "threshold": -6.233997344970703
        },
        "plugins_order": [
            "compressor#2",
            "compressor#1",
            "limiter#0"
        ]
    }
}

```
