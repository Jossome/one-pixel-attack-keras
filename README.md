# Disguise Attack
An extreme attack base on the paper "One pixel attack for fooling deep neural networks".

## Demo
- Our results:
    - ![](https://github.com/Jossome/one-pixel-attack-keras/blob/master/images/1.png =250x250)
- One-pixel-attack results:
    - ![](https://github.com/Jossome/one-pixel-attack-keras/blob/master/images/one_pixel.png =250x250)

## What's new?
- Our adversarial pixel is harder or even impossible to find.
- Objective:
    - $$ L = e^{\gamma(C-1)} + \Delta $$, a soft manner.
    - where C stands for real class label, $\Delta$ stands for the difference between the pixel before and after attack.
    - $\gamma$ is a threshold to control the exponential growth rate.
- YUV color space:
    - https://en.wikipedia.org/wiki/YUV
    - The different $\Delta$ is calculated on YUV space instead of RGB space.

## TODO
- [x] Run on cifar10.
- [x] Run on basic leNet and ResNet.
- [ ] Regulation on $\Delta$.
- [ ] Run on more models.
- [ ] Run on imageNet.
