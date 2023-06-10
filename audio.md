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
            "knee": -3.0,
            "lpf-frequency": 11000.0,
            "lpf-mode": "off",
            "makeup": 1.0,
            "mode": "Downward",
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
            "bypass": false,
            "dry": -100.0,
            "hpf-frequency": 10.0,
            "hpf-mode": "off",
            "input-gain": 0.0,
            "knee": 0.0,
            "lpf-frequency": 20000.0,
            "lpf-mode": "off",
            "makeup": 4.0,
            "mode": "Boosting",
            "output-gain": 0.0,
            "ratio": 2.0,
            "release": 140.0,
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
        "limiter#1": {
            "alr": false,
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
            "threshold": -8.0
        },
        "plugins_order": [
            "compressor#2",
            "compressor#1",
            "limiter#1"
        ]
    }
}

```
