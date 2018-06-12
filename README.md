# vokitoki

Ta repozitorij je namenjen izdelavi seminarske naloge pri predmetu Brezžična in mobilna omrežja.

Uporabljena je bila koda iz vaj, kateri sva dodala nekatere funkcionalnosti.

## Zajemanje zvoka
Zvok sva zajemala z AudioRecord-om. Parametri za inicializacijo:
+ RECORDER_SAMPLERATE = 8000
+ RECORDER_CHANNELS = AudioFormat.CHANNEL_IN_MONO
+ PLAYER_CHANNELS = AudioFormat.CHANNEL_OUT_MONO
+ RECORDER_AUDIO_ENCODING = AudioFormat.ENCODING_PCM_16BIT
+ bufferSize = AudioRecord.getMinBufferSize(RECORDER_SAMPLERATE, RECORDER_CHANNELS, RECORDER_AUDIO_ENCODING)

## Predvajanje zvoka
Zvok sva predvajala z uporabo AudioTrack-a. Parametri za inicializacijo:
+ RECORDER_SAMPLERATE = 8000
+ RECORDER_CHANNELS = AudioFormat.CHANNEL_IN_MONO
+ PLAYER_CHANNELS = AudioFormat.CHANNEL_OUT_MONO
+ RECORDER_AUDIO_ENCODING = AudioFormat.ENCODING_PCM_16BIT
+ bufferSize = AudioRecord.getMinBufferSize(RECORDER_SAMPLERATE, RECORDER_CHANNELS, RECORDER_AUDIO_ENCODING)

## Pošiljanje zvoka
Ko se napravi povežeta, se pokaže gumb, ki ob držanju snema zvok in ga sproti pošilja povezani napravi. Uporabila sva socket, ki je bil uporabljen v prvotni kodi. Možnost izboljšave bi bila uporaba DatagramSocket-a.

___

Avtor izvorne kode/mentor: Mattia Petroni

Avtorja walkie-talkie-ja: Domen Rek in Gregor Kerševan
