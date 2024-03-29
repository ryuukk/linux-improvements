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
            "attack": 50.0,
            "boost-amount": 10.0,
            "boost-threshold": -60.0,
            "bypass": false,
            "dry": -100.0,
            "hpf-frequency": 10.0,
            "hpf-mode": "off",
            "input-gain": 0.0,
            "knee": -10.482109069824219,
            "lpf-frequency": 20000.0,
            "lpf-mode": "off",
            "makeup": 0.0,
            "mode": "Boosting",
            "output-gain": 0.0,
            "ratio": 2.0,
            "release": 600.0,
            "release-threshold": -100.0,
            "sidechain": {
                "lookahead": 0.0,
                "mode": "RMS",
                "preamp": 0.0,
                "reactivity": 10.0,
                "source": "Middle",
                "stereo-split-source": "Left/Right",
                "type": "Feed-forward"
            },
            "stereo-split": false,
            "threshold": -12.0,
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
            "oversampling": "Half x4(3L)",
            "release": 10.0,
            "sidechain-preamp": 0.0,
            "stereo-link": 100.0,
            "threshold": -1.0
        },
        "multiband_compressor#0": {
            "band0": {
                "attack-threshold": -30.0,
                "attack-time": 50.0,
                "boost-amount": 6.0,
                "boost-threshold": -72.0,
                "compression-mode": "Downward",
                "compressor-enable": true,
                "external-sidechain": false,
                "knee": -24.0,
                "makeup": 0.0,
                "mute": false,
                "ratio": 1.7,
                "release-threshold": -100.0,
                "release-time": 600.0,
                "sidechain-custom-highcut-filter": false,
                "sidechain-custom-lowcut-filter": false,
                "sidechain-highcut-frequency": 250.0,
                "sidechain-lookahead": 0.0,
                "sidechain-lowcut-frequency": 10.0,
                "sidechain-mode": "RMS",
                "sidechain-preamp": 0.0,
                "sidechain-reactivity": 10.0,
                "sidechain-source": "Middle",
                "solo": false,
                "stereo-split-source": "Left/Right"
            },
            "band1": {
                "attack-threshold": -30.0,
                "attack-time": 30.0,
                "boost-amount": 6.0,
                "boost-threshold": -72.0,
                "compression-mode": "Downward",
                "compressor-enable": true,
                "enable-band": true,
                "external-sidechain": false,
                "knee": -24.0,
                "makeup": 0.0,
                "mute": false,
                "ratio": 1.7,
                "release-threshold": -100.0,
                "release-time": 450.0,
                "sidechain-custom-highcut-filter": false,
                "sidechain-custom-lowcut-filter": false,
                "sidechain-highcut-frequency": 1250.0,
                "sidechain-lookahead": 0.0,
                "sidechain-lowcut-frequency": 250.0,
                "sidechain-mode": "RMS",
                "sidechain-preamp": 0.0,
                "sidechain-reactivity": 10.0,
                "sidechain-source": "Middle",
                "solo": false,
                "split-frequency": 250.0,
                "stereo-split-source": "Left/Right"
            },
            "band2": {
                "attack-threshold": -30.0,
                "attack-time": 10.0,
                "boost-amount": 6.0,
                "boost-threshold": -72.0,
                "compression-mode": "Downward",
                "compressor-enable": true,
                "enable-band": true,
                "external-sidechain": false,
                "knee": -24.0,
                "makeup": 0.0,
                "mute": false,
                "ratio": 1.7,
                "release-threshold": -100.0,
                "release-time": 250.0,
                "sidechain-custom-highcut-filter": false,
                "sidechain-custom-lowcut-filter": false,
                "sidechain-highcut-frequency": 5000.0,
                "sidechain-lookahead": 0.0,
                "sidechain-lowcut-frequency": 1250.0,
                "sidechain-mode": "RMS",
                "sidechain-preamp": 0.0,
                "sidechain-reactivity": 10.0,
                "sidechain-source": "Middle",
                "solo": false,
                "split-frequency": 1250.0,
                "stereo-split-source": "Left/Right"
            },
            "band3": {
                "attack-threshold": -30.0,
                "attack-time": 5.0,
                "boost-amount": 6.0,
                "boost-threshold": -72.0,
                "compression-mode": "Downward",
                "compressor-enable": true,
                "enable-band": true,
                "external-sidechain": false,
                "knee": -24.0,
                "makeup": 0.0,
                "mute": false,
                "ratio": 1.7,
                "release-threshold": -100.0,
                "release-time": 100.0,
                "sidechain-custom-highcut-filter": false,
                "sidechain-custom-lowcut-filter": false,
                "sidechain-highcut-frequency": 20000.0,
                "sidechain-lookahead": 0.0,
                "sidechain-lowcut-frequency": 5000.0,
                "sidechain-mode": "RMS",
                "sidechain-preamp": 0.0,
                "sidechain-reactivity": 10.0,
                "sidechain-source": "Middle",
                "solo": false,
                "split-frequency": 5000.0,
                "stereo-split-source": "Left/Right"
            },
            "band4": {
                "attack-threshold": -12.0,
                "attack-time": 20.0,
                "boost-amount": 6.0,
                "boost-threshold": -72.0,
                "compression-mode": "Downward",
                "compressor-enable": true,
                "enable-band": false,
                "external-sidechain": false,
                "knee": -6.0,
                "makeup": 0.0,
                "mute": false,
                "ratio": 1.0,
                "release-threshold": -100.0,
                "release-time": 100.0,
                "sidechain-custom-highcut-filter": false,
                "sidechain-custom-lowcut-filter": false,
                "sidechain-highcut-frequency": 8000.0,
                "sidechain-lookahead": 0.0,
                "sidechain-lowcut-frequency": 4000.0,
                "sidechain-mode": "RMS",
                "sidechain-preamp": 0.0,
                "sidechain-reactivity": 10.0,
                "sidechain-source": "Middle",
                "solo": false,
                "split-frequency": 4000.0,
                "stereo-split-source": "Left/Right"
            },
            "band5": {
                "attack-threshold": -12.0,
                "attack-time": 20.0,
                "boost-amount": 6.0,
                "boost-threshold": -72.0,
                "compression-mode": "Downward",
                "compressor-enable": true,
                "enable-band": false,
                "external-sidechain": false,
                "knee": -6.0,
                "makeup": 0.0,
                "mute": false,
                "ratio": 1.0,
                "release-threshold": -100.0,
                "release-time": 100.0,
                "sidechain-custom-highcut-filter": false,
                "sidechain-custom-lowcut-filter": false,
                "sidechain-highcut-frequency": 12000.0,
                "sidechain-lookahead": 0.0,
                "sidechain-lowcut-frequency": 8000.0,
                "sidechain-mode": "RMS",
                "sidechain-preamp": 0.0,
                "sidechain-reactivity": 10.0,
                "sidechain-source": "Middle",
                "solo": false,
                "split-frequency": 8000.0,
                "stereo-split-source": "Left/Right"
            },
            "band6": {
                "attack-threshold": -12.0,
                "attack-time": 20.0,
                "boost-amount": 6.0,
                "boost-threshold": -72.0,
                "compression-mode": "Downward",
                "compressor-enable": true,
                "enable-band": false,
                "external-sidechain": false,
                "knee": -6.0,
                "makeup": 0.0,
                "mute": false,
                "ratio": 1.0,
                "release-threshold": -100.0,
                "release-time": 100.0,
                "sidechain-custom-highcut-filter": false,
                "sidechain-custom-lowcut-filter": false,
                "sidechain-highcut-frequency": 16000.0,
                "sidechain-lookahead": 0.0,
                "sidechain-lowcut-frequency": 12000.0,
                "sidechain-mode": "RMS",
                "sidechain-preamp": 0.0,
                "sidechain-reactivity": 10.0,
                "sidechain-source": "Middle",
                "solo": false,
                "split-frequency": 12000.0,
                "stereo-split-source": "Left/Right"
            },
            "band7": {
                "attack-threshold": -12.0,
                "attack-time": 20.0,
                "boost-amount": 6.0,
                "boost-threshold": -72.0,
                "compression-mode": "Downward",
                "compressor-enable": true,
                "enable-band": false,
                "external-sidechain": false,
                "knee": -6.0,
                "makeup": 0.0,
                "mute": false,
                "ratio": 1.0,
                "release-threshold": -100.0,
                "release-time": 100.0,
                "sidechain-custom-highcut-filter": false,
                "sidechain-custom-lowcut-filter": false,
                "sidechain-highcut-frequency": 20000.0,
                "sidechain-lookahead": 0.0,
                "sidechain-lowcut-frequency": 16000.0,
                "sidechain-mode": "RMS",
                "sidechain-preamp": 0.0,
                "sidechain-reactivity": 10.0,
                "sidechain-source": "Middle",
                "solo": false,
                "split-frequency": 16000.0,
                "stereo-split-source": "Left/Right"
            },
            "bypass": false,
            "compressor-mode": "Modern",
            "dry": -100.0,
            "envelope-boost": "None",
            "input-gain": 0.0,
            "output-gain": 0.0,
            "stereo-split": false,
            "wet": 0.0
        },
        "plugins_order": [
            "compressor#2",
            "compressor#1",
            "multiband_compressor#0",
            "limiter#0"
        ]
    }
}


```
