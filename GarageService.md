package com.dc.sviluppo;


import java.util.List;

import org.springframework.web.bind.annotation.RequestBody;

public class GarageService {

	private GarageRepository garagerepository;
	
	

	public GarageService(GarageRepository garagerepository) {
		super();
		this.garagerepository = garagerepository;
	}


	Garage creaGarage( Garage newGarage) {
		return garagerepository.save(newGarage);
	}
	
	Iterable <Garage>  Findall() {
		return garagerepository.findAll();
		
	}
	
	public String cerca_nome_garage(String nome_garage) {
		Iterable<Garage> all= garagerepository.findAll();
		
		for( Garage garage :all) {
			if (nome_garage.equals(garage.getNome_Garage())) {
				break;
			
			}
		}
		return nome_garage;
	}
	
}
	
	
	//List <Garage> findByName(){
		//return (List<Garage>) garagerepository.findBynome_Garage();}

		




