package com.dc.sviluppo;

import java.util.List;



import jakarta.persistence.Column;
import jakarta.persistence.Entity;
import jakarta.persistence.GeneratedValue;
import jakarta.persistence.Id;
import jakarta.persistence.Table;

@Entity
@Table(name = "Garage")
public class Garage {

	@Column(name = "ID")
	private @Id @GeneratedValue long id;

	@Column(name = "NOME GARAGE")
	private String nome_Garage;

	@Column(name = "PIANI")
	private List<Piano> piani;

	public String getNome_Garage() {
		return nome_Garage;
	}

	public void setNome_Garage(String nome_Garage) {
		this.nome_Garage = nome_Garage;
	}

	public List<Piano> getPiani() {
		return piani;
	}

	public void setPiani(List<Piano> piani) {
		this.piani = piani;
	}

	public long getId() {
		return id;
	}

	public void setId(long id) {
		this.id = id;
	}

	public Garage(String nome_Garage, List<Piano> piani) {
		super();
		this.nome_Garage = nome_Garage;
		this.piani = piani;
	}

}
