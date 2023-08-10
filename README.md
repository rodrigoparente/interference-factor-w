# Wireless Channel Assignment in Smart Home

This repository is part of the paper: [Wireless Channel Assignment in Smart Home](https://ieeexplore.ieee.org/abstract/document/8538545), published at the IEEE Symposium on Computers and Communications. In this work, we present a channel assigner using a Mixed Integer Linear Program (MILP) model that minimizes the interference suffered by devices that uses Wi-Fi, Zigbee, and Bluetooth technology in the Wireless Home Network (WHN).

## Interference Factor *w*

 The [table](./interference-factor-w.pdf) maps the interference between the Wi-Fi, Zigbee, and Bluetooth channels. The variable <img src="http://latex.codecogs.com/gif.latex?%5Clarge%20w%5E%7Bz%2Cm%7D" /> is the interference factor that the channel *m* cause on the channel *z*. This value is given in percent and is the ratio of how much of the frequency range *m* uses to communicate is superimposed over *z*.

 The value of *w* in the [table](./interference-factor-w.pdf) is used to calculate the interference a device suffer and is part of the formula:

 ![equation](http://latex.codecogs.com/gif.latex?%5Clarge%20I_%7Bi%2Cj%7D%5E%7Bz%2Cm%7D%20%3D%20%5Cfrac%7Bw%5E%7Bz%2Cm%7D%20%5Ctimes%20P_%7Bj%7D%5E%7Bm%7D%7D%7BPL%28d_%7Bi%2Cj%7D%29%7D)

The [table](./interference-factor-w.pdf) should be read as follows: The cell value line *m* and column *z* represents the amount (in percentage) that the channel represented by the line *m* overlaps the channel represented by the column *z*.

### Reference

If you re-use this work, please cite:

```
@inproceedings{da2018wireless,
  title={Wireless channel assignment in smart home},
  author={da Ponte, Francisco RP and de Almeida, K{\'\i}lvia LA and Gomes, Rafael L and Celestino, Joaquim and Pereira, Walisson F and da Fonseca, Nelson LS},
  booktitle={2018 IEEE Symposium on Computers and Communications (ISCC)},
  pages={00480--00485},
  year={2018},
  organization={IEEE}
}
```

## License

This project is [GNU GPLv3 licensed](./LICENSE).