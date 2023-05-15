# Loudness filter (normalize audio)

- ``easyeffects``

```json
{
    "output": {
        "autogain#0": {
            "bypass": true,
            "input-gain": 0.0,
            "maximum-history": 15,
            "output-gain": 0.0,
            "reference": "Geometric Mean (MI)",
            "silence-threshold": -70.0,
            "target": -26.999999999999957
        },
        "bass_enhancer#0": {
            "amount": 5.0,
            "blend": 5.0,
            "bypass": false,
            "floor": 20.0,
            "floor-active": false,
            "harmonics": 8.5,
            "input-gain": 0.0,
            "output-gain": 0.0,
            "scope": 100.0
        },
        "blocklist": [],
        "compressor#0": {
            "attack": 20.0,
            "boost-amount": 6.0,
            "boost-threshold": -60.0,
            "bypass": false,
            "dry": -100.0,
            "hpf-frequency": 10.0,
            "hpf-mode": "off",
            "input-gain": 0.0,
            "knee": -3.0,
            "lpf-frequency": 20000.0,
            "lpf-mode": "off",
            "makeup": -10.0,
            "mode": "Upward",
            "output-gain": 0.0,
            "ratio": 4.0,
            "release": 100.0,
            "release-threshold": -100.0,
            "sidechain": {
                "lookahead": 0.0,
                "mode": "RMS",
                "preamp": 0.0,
                "reactivity": 10.0,
                "source": "Middle",
                "type": "Feed-forward"
            },
            "threshold": -10.0,
            "wet": 3.0
        },
        "limiter#1": {
            "alr": true,
            "alr-attack": 5.0,
            "alr-knee": 0.0,
            "alr-release": 100.0,
            "attack": 5.0,
            "bypass": false,
            "dithering": "None",
            "external-sidechain": false,
            "gain-boost": true,
            "input-gain": 0.0,
            "lookahead": 5.0,
            "mode": "Herm Thin",
            "output-gain": 0.0,
            "oversampling": "None",
            "release": 5.0,
            "sidechain-preamp": 0.0,
            "stereo-link": 100.0,
            "threshold": -3.0
        },
        "loudness#0": {
            "bypass": false,
            "clipping": false,
            "clipping-range": 12.0,
            "fft": "4096",
            "input-gain": 0.0,
            "output-gain": 0.0,
            "std": "ISO226-2003",
            "volume": 0.0
        },
        "plugins_order": [
            "compressor#0",
            "bass_enhancer#0",
            "autogain#0",
            "limiter#1",
            "loudness#0"
        ]
    }
}

```
