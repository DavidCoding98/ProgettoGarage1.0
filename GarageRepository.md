package com.dc.sviluppo; 

import java.util.List;

import org.springframework.data.repository.CrudRepository;
public interface GarageRepository extends CrudRepository<Garage,Long> {
	
	public List <Garage> findBynome_Garage(String nome_Garage);
	
	//public List <Garage> findByCodice(String codice);
	//public String cercaGarage(String nome_garage);
	//public Iterable<Garage> findBynome_Garage();
}

