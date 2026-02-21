# LSTM Financial Time Series

Minimal PyTorch implementation of an LSTM for financial time series forecasting.

## Goal

Understand the structure of sequence modeling on financial returns and compare an LSTM against simple statistical baselines.

## Problem Setup

Given daily log-returns:

r₁, r₂, ..., r_T

We build supervised samples using rolling windows of length L:

Input:
X_t = [r_t, ..., r_{t+L-1}]

Target:
y_t = r_{t+L}

Number of samples:
N = T − L

Tensor shapes (univariate case):

X → (N, L, 1)  
y → (N, 1)

## Pipeline

1. Download data  
2. Compute log-returns  
3. Temporal train/test split  
4. Window construction  
5. Baseline comparison  
6. LSTM training  

## Status

Project initialized. Data pipeline in progress.