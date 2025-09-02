# Qingdao University Online Judge System

[![Build Status](https://travis-ci.org/QingdaoU/OnlineJudge.svg?branch=master)](https://travis-ci.org/QingdaoU/OnlineJudge)

An open-source online judge system based on Python and Vue, suitable for programming practice and algorithm competitions.

## Demo

[https://qduoj.com](https://qduoj.com)

## Overview

This is a complete online judge system with the following features:

- Based on Docker for one-click deployment
- Separated backend and frontend with modular programming and microservices architecture
- Support for ACM/OI competition rules with real-time/non-real-time ranking
- Powerful charting and visualization capabilities
- Template problem support
- Fine-grained permission control
- Multi-language support: C, C++, Java, Python2, Python3
- Markdown and MathJax support
- Contest participant IP limitation (CIDR)

## Architecture

The system consists of several core modules:

- **Backend** (Django): The main application providing RESTful APIs
- **Frontend** (Vue): User interface with responsive design
- **Judger** (Seccomp): Secure sandbox for code execution
- **JudgeServer** (Go): Wrapper for the Judger component
- **Deployment** (Docker Compose): One-click deployment solution

## Quick Start

### Prerequisites

- Linux environment (Ubuntu 18.04 LTS recommended) or Windows with Docker tools
- Docker and Docker Compose installed

### Installation

1. Clone the deployment repository:
   ```bash
   git clone -b 2.0 https://github.com/QingdaoU/OnlineJudgeDeploy.git && cd OnlineJudgeDeploy