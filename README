TepsitMediaPlayer

TepsitMediaPlayer è un’applicazione multimediale sviluppata in Python utilizzando PyQt6, progettata per offrire una gestione semplice ed efficace di contenuti audio e video.
L’interfaccia grafica è moderna, ordinata e progettata per facilitare l’uso quotidiano.

⸻

Funzionalità e Implementazione (con righe di codice)
	•	Riproduzione audio e video separata
Ogni tipo di file ha un player dedicato:
	•	Audio: self.audio_player (riga ~72) + self.audio_audio_output (riga ~73)
	•	Video: self.video_player (riga ~63) + self.video_audio_output (riga ~64) + self.video_widget (riga ~65)
	•	Supporto ai formati comuni
Video: MP4, AVI, MKV, MOV
Audio: MP3, WAV, OGG
Implementato nelle funzioni load_video_files (~riga 187) e load_audio_files (~riga 271) tramite QFileDialog e filtri.
	•	Controlli completi (Play, Pausa, Stop, Avanti, Indietro, Volume, Posizione)
Funzioni:
	•	play_pause_video (~riga 202)
	•	stop_video (~riga 209)
	•	prev_video (~riga 215)
	•	next_video (~riga 221)
	•	play_pause_audio (~riga 291)
	•	stop_audio (~riga 298)
	•	prev_audio (~riga 304)
	•	next_audio (~riga 310)
Slider sincronizzati con segnali positionChanged e durationChanged:
	•	Video: position_changed_video (~riga 227), duration_changed_video (~riga 231), set_position_video (~riga 235)
	•	Audio: position_changed_audio (~riga 316), duration_changed_audio (~riga 320), set_position_audio (~riga 324)
	•	Playlist audio e video
Liste gestite con QListWidget:
	•	Video: self.video_list (~riga 85), gestione doppio clic: video_item_double_clicked (~riga 241)
	•	Audio: self.audio_list (~riga 108), gestione doppio clic: audio_item_double_clicked (~riga 330)
	•	Salvataggio automatico dei file
Copia dei file in audio_files/ e video_files/ realizzata tramite shutil.copy dentro:
	•	load_video_files (~riga 187)
	•	load_audio_files (~riga 271)
	•	Aggiornamento interfaccia durante la riproduzione
	•	Aggiornamento label: self.label_video (~riga 69) e self.label_audio (~riga 77)
	•	Slider di avanzamento sincronizzati con i segnali dei media player come sopra.
	•	Interfaccia con colori neutri e leggibili
Implementata tramite self.setStyleSheet (~riga 21), definendo colori di sfondo, pulsanti, slider e testi.

⸻

Obiettivo del Progetto

BrightMediaPlayer nasce per fornire un player semplice, leggero e immediato, che consenta di:
	•	Ascoltare musica
	•	Guardare video
	•	Organizzare automaticamente i file multimediali
	•	Usare un’interfaccia moderna e pulita, facilmente ampliabile.

⸻

Tecnologia Utilizzata
	•	Python 3.10+
	•	PyQt6 (QtWidgets, QtMultimedia, QtGui)
	•	Gestione file: os, shutil, QFileDialog
	•	Sistema di riproduzione: QMediaPlayer + QAudioOutput
	•	Visualizzazione video: QVideoWidget

⸻

Licenza

Progetto libero e modificabile.
L’utente può adattarlo, ampliarlo o integrarlo in altri sistemi.
