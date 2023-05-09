package com.dc.sviluppo;

import java.util.List;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.PostMapping;
import org.springframework.web.bind.annotation.RequestBody;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class GarageController {

private GarageService garageservice;

	
	public GarageController(GarageService garageservice) {
	super();
	this.garageservice = garageservice;
}

	@GetMapping("/garage")
	Iterable<Garage> getGarage(){
		return garageservice.Findall();
	}
	 
	@PostMapping("/garage")
	Garage creaGarage(@RequestBody Garage newGarage) {
		return garageservice.creaGarage(newGarage);
	}
	
 
}

