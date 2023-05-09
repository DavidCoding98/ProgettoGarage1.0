package com.dc.sviluppo;

public class Posto {

	private String codice;
	private boolean occupato;

	public String getCodice() {
		return codice;
	}

	public void setCodice(String codice) {
		this.codice = codice;
	}

	public boolean isOccupato() {
		return occupato;
	}

	public void setOccupato(boolean occupato) {
		this.occupato = occupato;
	}

	public Posto(String codice, boolean occupato) {
		super();
		this.codice = codice;
		this.occupato = occupato;
	}

}
