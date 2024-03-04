# Documentatios techniques de l'application mobile Frisz 
le contenu de la documentation 

```HTML {.code-block}

<div [ngClass]="{enregistreVoice: enreVoice}" class="parentFichier" *ngIf="showVoice" style="width:30rem">
			    				<span (click)="abortSendFile()" class="mdi mdi-alpha-x-circle"></span>
			    				<div>
			    					<img *ngIf="enreVoice"  src="../../../../assets/img/3.gif" alt="animation pendant l'enrégistrement du voice">
			    					<div *ngIf="!enreVoice" class="parVoice">
			    						<div id="waveform" style="width:75%, overflow: hidden;" ></div>
			    						<div class="enf2">
			    							<div class="gauche">
			    								<button *ngIf="wavesurfer && playS" (click)="playSound()" ><i class="mdi mdi-play"></i
													></button>
													<button *ngIf="wavesurfer && !playS" (click)="pauseSound()" ><i class="mdi mdi-pause"></i
													></button>
													<button *ngIf="wavesurfer" (click)="stopSound()" ><i class="mdi mdi-stop"></i
													></button>
													<button *ngIf="wavesurfer" (click)="changePlaybackSpeed(1)">x {{ playbackSpeed.toFixed(2) }}</button>
			    							</div>
			    							
												<div class="droite" >
													<strong *ngIf="wavesurfer" >{{formatTime(wavesurfer.getCurrentTime())}} / </strong>
													<strong *ngIf="wavesurfer" >{{formatTime(wavesurfer.getDuration())}}</strong>
												</div>
												
			    						</div>

			    					</div> 
			    				</div>
			    			</div>


```