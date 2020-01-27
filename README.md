# Blackjack
import org.apache.commons.lang3.ArrayUtils;

import java.util.ArrayList;
import java.util.Arrays;
import java.util.Collections;
import java.util.List;
import java.util.Scanner;

public class Cards {

	static int[] value;
//make the deck of cards
	static List<String> list = new ArrayList<String>(100);
	{

		list.add("TWO-Koupa");
		list.add("TWO-Mpastouni");
		list.add("TWO-Trifilli");
		list.add("TWO-Karo");
		list.add("THREE-Koupa");
		list.add("THREE-Mpastouni");
		list.add("THREE-Trifilli");
		list.add("THREE-Karo");
		list.add("FOUR-Koupa");
		list.add("FOUR-Mpastouni");
		list.add("FOUR-Trifilli");
		list.add("FOUR-Karo");
		list.add("FIVE-Koupa");
		list.add("FIVE-Mpastouni");
		list.add("FIVE-Trifilli");
		list.add("FIVE-Karo");
		list.add("SIX-Koupa");
		list.add("SIX-Mpastouni");
		list.add("SIX-Trifilli");
		list.add("SIX-Karo");
		list.add("SEVEN-Koupa");
		list.add("SEVEN-Mpastouni");
		list.add("SEVEN-Trifilli");
		list.add("SEVEN-Karo");
		list.add("EIGHT-Koupa");
		list.add("EIGHT-Mpastouni");
		list.add("EIGHT-Trifilli");
		list.add("EIGHT-Karo");
		list.add("NINE-Koupa");
		list.add("NINE-Mpastouni");
		list.add("NINE-Trifilli");
		list.add("NINE-Karo");
		list.add("TEN-Koupa");
		list.add("TEN-Mpastouni");
		list.add("TEN-Trifilli");
		list.add("TEN-Karo");
		list.add("Dama-Koupa");
		list.add("Dama-Mpastouni");
		list.add("Dama-Trifilli");
		list.add("Dama-Karo");
		list.add("Vales-Koupa");
		list.add("Vales-Mpastouni");
		list.add("Vales-Trifilli");
		list.add("Vales-Karo");
		list.add("Rigas-Koupa");
		list.add("Rigas-Mpastouni");
		list.add("Rigas-Trifilli");
		list.add("Rigas-Karo");
		list.add("ACE-Koupa");
		list.add("ACE-Mpastouni");
		list.add("ACE-Trifilli");
		list.add("ACE-Karo");

	}

	public void shuffleCards() {

		Collections.shuffle(list);

	}

	public int getValue(ArrayList<String> cardsPlayer, int valuePlayer, List<String> list) {
		

		Player pl = new Player("");

		System.out.println(cardsPlayer);
		for (int i = 0; i < cardsPlayer.size(); i++) {

			if (cardsPlayer.get(i).equals("Dama-Koupa") || cardsPlayer.get(i).equals("Dama-Mpastouni")
					|| cardsPlayer.get(i).equals("Dama-Trifilli") || cardsPlayer.get(i).equals("Dama-Karo")
					|| cardsPlayer.get(i).equals("Vales-Mpastouni") || cardsPlayer.get(i).equals("Vales-Trifilli")
					|| cardsPlayer.get(i).equals("Vales-Karo") || cardsPlayer.get(i).equals("Vales-Koupa")
					|| cardsPlayer.get(i).equals("Rigas-Mpastouni") || cardsPlayer.get(i).equals("Rigas-Trifilli")
					|| cardsPlayer.get(i).equals("Rigas-Karo") || cardsPlayer.get(i).equals("Rigas-Koupa")) {

				value = ArrayUtils.add(value, 10);

			}

			else if (cardsPlayer.get(i).equals("TWO-Mpastouni") || cardsPlayer.get(i).equals("TWO-Trifilli")
					|| cardsPlayer.get(i).equals("TWO-Karo") || cardsPlayer.get(i).equals("TWO-Koupa")) {
				value = ArrayUtils.add(value, 2);

			}

			else if (cardsPlayer.get(i).equals("THREE-Mpastouni") || cardsPlayer.get(i).equals("THREE-Trifilli")
					|| cardsPlayer.get(i).equals("THREE-Karo") || cardsPlayer.get(i).equals("THREE-Koupa")) {
				value = ArrayUtils.add(value, 3);

			}

			else if (cardsPlayer.get(i).equals("FOUR-Mpastouni") || cardsPlayer.get(i).equals("FOUR-Koupa")
					|| cardsPlayer.get(i).equals("FOUR-Trifilli") || cardsPlayer.get(i).equals("FOUR-Karo")) {
				value = ArrayUtils.add(value, 4);

			}

			else if (cardsPlayer.get(i).equals("FIVE-Mpastouni") || cardsPlayer.get(i).equals("FIVE-Trifilli")
					|| cardsPlayer.get(i).equals("FIVE-Koupa") || cardsPlayer.get(i).equals("FIVE-Karo")) {
				value = ArrayUtils.add(value, 5);

			} else if (cardsPlayer.get(i).equals("SIX-Mpastouni") || cardsPlayer.get(i).equals("SIX-Trifilli")
					|| cardsPlayer.get(i).equals("SIX-Koupa") || cardsPlayer.get(i).equals("SIX-Karo")) {
				value = ArrayUtils.add(value, 6);

			}

			else if (cardsPlayer.get(i).equals("SEVEN-Mpastouni") || cardsPlayer.get(i).equals("SEVEN-Trifilli")
					|| cardsPlayer.get(i).equals("SEVEN-Koupa") || cardsPlayer.get(i).equals("SEVEN-Karo")) {
				value = ArrayUtils.add(value, 7);

			}

			else if (cardsPlayer.get(i).equals("EIGHT-Mpastouni")
					|| cardsPlayer.get(i).equals("EIGHT-Trifilli") | cardsPlayer.get(i).equals("EIGHT-Koupa")
					|| cardsPlayer.get(i).equals("EIGHT-Karo")) {
				value = ArrayUtils.add(value, 8);

			}

			else if (cardsPlayer.get(i).equals("NINE-Mpastouni") || cardsPlayer.get(i).equals("NINE-Trifilli")
					|| cardsPlayer.get(i).equals("NINE-Koupa") || cardsPlayer.get(i).equals("NINE-Karo")) {
				value = ArrayUtils.add(value, 9);

			}

			else if (cardsPlayer.get(i).equals("TEN-Mpastouni") || cardsPlayer.get(i).equals("TEN-Trifilli")
					|| cardsPlayer.get(i).equals("TEN-Koupa") || cardsPlayer.get(i).equals("TEN-Karo")) {
				value = ArrayUtils.add(value, 10);

			}

			else if (cardsPlayer.get(i).equals("ACE-Mpastouni") || cardsPlayer.get(i).equals("ACE-Trifilli")
					|| cardsPlayer.get(i).equals("ACE-Koupa") || cardsPlayer.get(i).equals("ACE-Karo")) {
				Scanner input = new Scanner(System.in);
				int answer;
				do {
					System.out.println(pl.name + "Do you want Your Ace to have value of 1 or 11");
					answer = input.nextInt();
				} while (!(answer == 1 || answer == 11));
				if (answer == 1) {
					value = ArrayUtils.add(value, 1);

				} else if (answer == 11) {
					value = ArrayUtils.add(value, 11);

				}

			}

		}
//calculation of current value
		valuePlayer = Arrays.stream(value).sum();

		value = null;
		return valuePlayer;

	}

}












	





