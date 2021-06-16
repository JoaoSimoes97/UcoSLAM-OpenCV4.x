//////////////////////////////////////////
//	LOCATION OF THE FOLDER		//
//////////////////////////////////////////
	place this folder at "~/", it is suposed to look like "~/ucoslam"
//////////////////////////////////////////
//		EXAMPLES		//
//////////////////////////////////////////
	////////////
	// CREATE //
	////////////
		./ucoslam_monocular ~/ucoslam_files/00/cam0.mp4 ~/ucoslam_files/00/cam0.yml -voc ~/ucoslam_files/orb.fbow -out ~/ucoslam_files/mapas/nomeDoMapa -params ~/ucoslam_files/myparams.yml
	////////////
	// UPDATE //
	////////////
		./ucoslam_monocular ~/ucoslam_files/00/cam0.mp4 ~/ucoslam_files/00/cam0.yml -voc ~/ucoslam_files/orb.fbow -map ~/ucoslam_files/mapas/nomeDoMapa.map -params ~/ucoslam_files/myparams.yml
	////////////////
	// TRACK_ONLY //
	////////////////
		./ucoslam_monocular ~/ucoslam_files/00/cam0.mp4 ~/ucoslam_files/00/cam0.yml -voc ~/ucoslam_files/orb.fbow -map ~/ucoslam_files/mapas/nomeDoMapa.map -params ~/ucoslam_files/myparams.yml -noMapUpdate
	//////////////////////////////////
	// TRACK_ONLY WITH VIDEO OUTPUT //
	//////////////////////////////////
		./ucoslam_monocular ~/ucoslam_files/video1/cam0.mp4 ~/ucoslam_files/video1/cam0.yml -voc ~/ucoslam_files/orb.fbow -params ~/ucoslam_files/myparams.yml -map world.map -noMapUpdate -outvideo outvideo.mp4
