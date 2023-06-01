# Loudness filter (normalize audio)

- package: ``easyeffects``

```json
{
    "output": {
        "blocklist": [],
        "compressor#1": {
            "attack": 30.0,
            "boost-amount": 10.0,
            "boost-threshold": -72.0,
            "bypass": false,
            "dry": -100.0,
            "hpf-frequency": 8000.0,
            "hpf-mode": "off",
            "input-gain": 0.0,
            "knee": -6.0,
            "lpf-frequency": 11000.0,
            "lpf-mode": "off",
            "makeup": 0.0,
            "mode": "Upward",
            "output-gain": 0.0,
            "ratio": 2.0,
            "release": 140.0,
            "release-threshold": -100.0,
            "sidechain": {
                "lookahead": 0.0,
                "mode": "Low-Pass",
                "preamp": 10.0,
                "reactivity": 10.0,
                "source": "Middle",
                "type": "Feed-forward"
            },
            "threshold": -24.0,
            "wet": 4.0
        },
        "limiter#1": {
            "alr": true,
            "alr-attack": 100.0,
            "alr-knee": -2.0,
            "alr-release": 500.0,
            "attack": 5.0,
            "bypass": false,
            "dithering": "None",
            "external-sidechain": false,
            "gain-boost": false,
            "input-gain": 0.0,
            "lookahead": 10.0,
            "mode": "Herm Thin",
            "output-gain": 0.0,
            "oversampling": "None",
            "release": 5.0,
            "sidechain-preamp": 0.0,
            "stereo-link": 100.0,
            "threshold": -4.0
        },
        "loudness#0": {
            "bypass": false,
            "clipping": true,
            "clipping-range": 12.0,
            "fft": "4096",
            "input-gain": 0.0,
            "output-gain": 0.0,
            "std": "ISO226-2003",
            "volume": 0.0
        },
        "plugins_order": [
            "compressor#1",
            "limiter#1",
            "loudness#0"
        ]
    }
}

```
