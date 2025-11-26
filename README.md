🎧 TepsitMediaPlayer

TepsitMediaPlayer è un’applicazione multimediale sviluppata in Python con PyQt6, progettata per offrire una gestione semplice ed efficace di contenuti audio e video.
L’interfaccia grafica è moderna, ordinata e studiata per facilitare l’uso quotidiano.

⸻

✨ Funzionalità principali
	•	🎬 Riproduzione video tramite QMediaPlayer e QVideoWidget
	•	🎵 Riproduzione audio tramite QMediaPlayer + QAudioOutput
	•	📂 Playlist separate per audio e video con navigazione avanti/indietro
	•	💾 Salvataggio automatico dei file nelle cartelle dedicate:
	•	audio_files/
	•	video_files/
	•	🎛 Controlli multimediali completi: Play, Pausa, Stop, Avanti, Indietro
	•	🎚 Slider per avanzamento e regolazione volume, aggiornati in tempo reale
	•	🖥️ Interfaccia chiara e leggibile, colori neutri
	•	🧩 Gestione dei file tramite doppio clic e aggiornamento delle label con il nome del file

⸻

🛠 Implementazione delle funzionalità

| Funzionalità                | Funzione / Classe                                     | Riga di riferimento |
|-----------------------------|------------------------------------------------------|------------------|
| Riproduzione audio           | `self.audio_player`, `self.audio_audio_output`       | 72-73            |
| Riproduzione video           | `self.video_player`, `self.video_audio_output`, `self.video_widget` | 63-65            |
| Caricamento video            | `load_video_files()`                                 | 187              |
| Caricamento audio            | `load_audio_files()`                                 | 271              |
| Play/Pausa video             | `play_pause_video()`                                 | 202              |
| Stop video                   | `stop_video()`                                       | 209              |
| Precedente/Successivo video  | `prev_video()`, `next_video()`                       | 215, 221         |
| Play/Pausa audio             | `play_pause_audio()`                                 | 291              |
| Stop audio                   | `stop_audio()`                                       | 298              |
| Precedente/Successivo audio  | `prev_audio()`, `next_audio()`                       | 304, 310         |
| Slider posizione video       | `position_changed_video()`, `duration_changed_video()`, `set_position_video()` | 227, 231, 235 |
| Slider posizione audio       | `position_changed_audio()`, `duration_changed_audio()`, `set_position_audio()` | 316, 320, 324 |
| Playlist video               | `self.video_list`, `video_item_double_clicked()`     | 85, 241          |
| Playlist audio               | `self.audio_list`, `audio_item_double_clicked()`     | 108, 330         |
| Salvataggio file             | `shutil.copy()` all’interno di `load_video_files()` e `load_audio_files()` | 187, 271 |
| Aggiornamento label e slider | Label: `self.label_video`, `self.label_audio`       | 69, 77           |
| Interfaccia grafica          | `self.setStyleSheet()`                               | 21               |


⸻

🎯 Obiettivo del progetto

BrightMediaPlayer nasce per fornire un player leggero, semplice e immediato, che permetta di:
	•	Ascoltare musica
	•	Guardare video
	•	Organizzare automaticamente i file multimediali
	•	Usare un’interfaccia moderna e pulita, facilmente ampliabile

⸻

⚙️ Tecnologia utilizzata
	•	Python 3.10+
	•	PyQt6 (QtWidgets, QtMultimedia, QtGui)
	•	Gestione file: os, shutil, QFileDialog
	•	Sistema di riproduzione: QMediaPlayer + QAudioOutput
	•	Visualizzazione video: QVideoWidget

⸻

📄 Licenza

Progetto libero e modificabile.
L’utente può adattarlo, ampliarlo o integrarlo in altri sistemi.
