# write-the-lyrics
In this project we've deleloped a jupyter notebook in colab to train and test a gpt-2 model fine tuned with Metallica lyrics.

We've taken all the 109 original Metallica songs, excluding _"Garage inc"_ since it's an album of covers and _"LuLu"_ since it's a colaboration with Lou Reed.

With that, we've fine-tuned a gpt-2 model to generate lyrics _Metallica-Style_. To test the model, we've taken away the last part of 10 of the songs (put away before training) and we've told the model to generate that missing part. Here we're looking for accuracy, but to avoid that the model forgots all it knows and overfits to the lyrics, we also look for some inventions that fits quite well.

Finally, the notebook can be used with no training needs to generate new lyrics, since the model can be pre-loaded if desired. The only thing the user has to do is to define a song title as a string with the format `"The sound of silence" <|endofverse|>`, where the quoted words are the title and `<endofverse>` is a special token that indicates the end of a verse. A possible output could be the following:

```
War is coming, no end 
The sun is shining clean through, no need to hide 
War is coming, war is here 
Please, please send the message 
Of no return 
War is coming, it's never ending 
Obey, obey, obey, obey 
When you feel fear or sorrow, turn your eyes 
You are no longer there, but the fear inside 
War is coming 
Pure gold reigns supreme 
Pure power whispers within 
They send darkness, but are not fear 
Dark times are upon us all 
Obey, obey, obey, obey 
When you feel fear or sorrow, turn your eyes 
You are no longer there, but the fear inside 
Obey, obey, obey, obey 
When you feel fear or sorrow, turn your eyes 
You are no longer there, but the fear inside 
Orking the shadows, but become so strong 
Men of iron rule
```
