# SDivergence.mq5

SDivergence is a custom indicator developed by the Forex Robot Easy Team. It is an adaptive strategy indicator that detects regular and hidden divergences in the market. The indicator can be used to identify potential trading opportunities and generate trading signals.

## How it Works

The SDivergence indicator calculates regular and hidden divergences based on the selected oscillator. Regular divergences occur when the price makes higher highs or lower lows, but the oscillator fails to confirm these higher highs or lower lows. Hidden divergences, on the other hand, occur when the price makes higher highs or lower lows, and the oscillator confirms these higher highs or lower lows.

The indicator has the following customizable parameters:
- `selectedOscillator`: Specifies the oscillator to use for divergence calculation. The default oscillator is MACD.
- `rdThreshold`: Specifies the threshold for regular divergences. The default value is 0.0001.
- `hdThreshold`: Specifies the threshold for hidden divergences. The default value is 0.0002.
- `enableRD`: Enables or disables regular divergences. The default value is true.
- `enableHD`: Enables or disables hidden divergences. The default value is true.

The indicator generates two buffers:
- `rdBuffer`: Contains the values for regular divergences.
- `hdBuffer`: Contains the values for hidden divergences.

The indicator also sets labels for the buffers:
- `Regular Divergence`: Label for the regular divergence buffer.
- `Hidden Divergence`: Label for the hidden divergence buffer.

## Indicator Initialization

The `OnInit()` function is responsible for initializing the indicator. It resizes the buffers to hold one value and sets the indicator buffers and labels.

## Indicator Calculation

The `OnCalculate()` function is called for each new tick in the market. It calculates regular and hidden divergences based on the selected oscillator and the provided price data. The calculated divergences are stored in the respective buffers.

## Regular Divergence Calculation

The `CalculateRegularDivergences()` function is responsible for calculating regular divergences. The specific calculation logic is not provided in the code and should be implemented separately.

## Hidden Divergence Calculation

The `CalculateHiddenDivergences()` function is responsible for calculating hidden divergences. The specific calculation logic is not provided in the code and should be implemented separately.

## Expert Advisor Start Function

The `OnStart()` function is the main logic of the trading robot. It can be customized to use the generated divergences for trading decisions and execution.

## Product Description

SDivergence is an adaptive strategy indicator developed by the Forex Robot Easy Team. It is designed to detect regular and hidden divergences in the market, which can be used to identify potential trading opportunities.

Regular divergences occur when the price makes higher highs or lower lows, but the indicator fails to confirm these movements. Hidden divergences, on the other hand, occur when the price makes higher highs or lower lows, and the indicator confirms these movements.

The SDivergence indicator is highly customizable, allowing traders to select the oscillator for divergence calculation and set threshold values for regular and hidden divergences. Traders can enable or disable regular and hidden divergences based on their trading preferences.

Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that demonstrates how the indicator works. To find the official developer of this product, please refer to the MQL5 community.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/sdivergence-forex-software-adaptive-strategy-indicator-review/).
