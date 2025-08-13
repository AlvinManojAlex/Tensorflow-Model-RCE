# Tensorflow-Model-RCE

This is a PoC for creating a malicious ML model using Tensorflow.

This is done by exploiting how layers in keras work. Specifically, by using Lambda layers which allows us to wrap Python expressions as a `Layer` object.

## Installation

<strong>Required Python version: 3.8</strong>

```bash
python -m pip install -r requirements.txt
```

Better approach would be to make use of the Dockerfile since `tensorflow-cpu` has dependency issues with different platforms.

## Usage

```bash
python exploit.py 127.0.0.1 6666
```

## Acknowledgments

[Splint Gitbook](https://splint.gitbook.io/cyberblog/security-research/tensorflow-remote-code-execution-with-malicious-model)