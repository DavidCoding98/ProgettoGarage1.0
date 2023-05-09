package com.dc.sviluppo;

import java.util.List;



public class Piano {

	private int n_piano;
	private List<Posto> posti;

	public int getN_piano() {
		return n_piano;
	}

	public void setN_piano(int n_piano) {
		this.n_piano = n_piano;
	}

	public List<Posto> getPosti() {
		return posti;
	}

	public void setPosti(List<Posto> posti) {
		this.posti = posti;
	}

	public Piano(int n_piano, List<Posto> posti) {
		super();
		this.n_piano = n_piano;
		this.posti = posti;
	}

}
