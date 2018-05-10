# TensorBoardColab

A library make TensorBoard working in Colab Google 

## Install
    pip install tensorboardcolab
In Colab Google Jupyter, for auto install and ensure using latest version of TensorBoardColab, please add "!pip install -U tensorboardcolab" at the first line of Jupyter cell

## Import
    from tensorboardcolab import *

## Initialization
    tbc=TensorBoardColab()

## Add to Keras callback
    model.fit(x,y,epochs=100000,callbacks=[TensorBoardColabCallback(tbc)])

## Save picture to TensorBoard
    tbc.save_image(title="test_title", image=image)

## Save a value to graph of TensorBoard
    tbc.save_value("graph_name", "line_name", epoch, value)

## Thanks
ngrok !