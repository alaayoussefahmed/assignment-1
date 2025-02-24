w1 = 0.15
w2 = 0.2
w3 = 0.25
w4 = 0.3
w5 = 0.4
w6 = 0.45
b1 = 0.5
b2 = 0.7
input1 = 0.05
input2 = 0.1
def tanh(x):
    return (2 / (1 + 2.71828 ** (-2 * x))) - 1 
    net_h1 = w1 * input1 + w2 * input2 + b1
out_h1 = tanh(net_h1)
net_h2 = w3 * input1  + w4 * input2 + b1
out_h2 = tanh(net_h2)
net_o1 = w5 * out_h1 + w6 * out_h2 + b2
out_o1 = tanh(net_o1)
net_o2 = w5 * out_h1 + w6 * out_h2 + b2
out_o2 = tanh(net_o2)
print("Hidden Layer 1:", out_h1)
print("Hidden Layer 2:", out_h2)
print("Output Layer 1:", out_o1)
print("Output Layer 2:", out_o2)
