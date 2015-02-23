# Calculatrice
Calculatrice
/**
* \file source.cpp
* \brief Calculatrice
* \author Guillaume Rodien
* \version 2.0
* \date 23 Fevrier 2015
*/

#include <stdio.h>
#include <inttypes.h>
using namespace std;

int main()
{
	int operateur, type; /* Déclaration des variables 

	/**
	* \param    operande
	* \brief       Pour le choix de l'operande
	* \details    L'user choisi un operande parmis celles disponibles.
	*/

	printf("Quelle operation voulez-vous faire ?\n 1- Addition\n 2- Soustraction\n 3- Multiplication\n 4- Division\n 5- Modulo\n");
	scanf("%d", &operateur); /* Récupération du choix de l'user */

	if (operateur == 1) /* Si il choisi de faire une addition */
	{
		/**
		* \param    type
		* \brief       Le choix du type de variable.
		* \details    L'user choisi le type de ces variables.
		*/

		printf("Quel type :\n 1- Int32\n 2- Int64\n 3- Double\n 4- Float\n ");
		scanf("%d", &type); /* Récupération du choix fait par l'user */


		/**
		* \param    operandeA
		* \brief       Chiffre n°1
		* \details    Premier chiffre que l'user va saisir
		*/

		/**
		* \param    operandeB
		* \brief       Chiffre n°2
		* \details    Deuxieme chiffre que l'user va saisir
		*/

		/**
		* \param    resultat
		* \brief       resultat de l'operation
		* \details    Variable ou est stocker le resultat de l'operation par les deux chiffres données par l'user.
		*/

		if (type == 1) /* Cette solution sera choisi si l'user prend le type 1 soit int 32 */
		{
			int32_t operandeA, operandeB, resultat; /* Déclaration des variables en int32_t */
			printf("Premier chiffre : ");
			scanf("%li", &operandeA);

			printf("Deuxieme chiffre : ");
			scanf("%li", &operandeB);

			resultat = operandeA + operandeB;
			printf("Le resultat est : %I32i\n", resultat);
		}
		else
		{
			if (type == 2) /* Cette solution sera choisi si l'user prend le type 2  soit int 64 */
			{
				int64_t operandeA, operandeB, resultat; /* Déclaration des variables en int64_t */
				printf("Premier chiffre : ");
				scanf("%I64i", &operandeA);

				printf("Deuxieme chiffre : ");
				scanf("%I64i", &operandeB);

				resultat = operandeA + operandeB;
				printf("Le resultat est : %I64i\n", resultat);
			}
			else
			{
				if (type == 3) /* Cette solution sera choisi si l'user prend le type 3 soit double */
				{
					double operandeA, operandeB, resultat; /* Déclaration des variables en double */
					printf("Premier chiffre : ");
					scanf("%lf", &operandeA);

					printf("Deuxieme chiffre : ");
					scanf("%lf", &operandeB);

					resultat = operandeA + operandeB;
					printf("Le resultat est : %lf\n", resultat);
				}
				else
				{
					if (type == 4) /* Cette solution sera choisi si l'user prend le type 4 soit un float */
					{
						float operandeA, operandeB, resultat; /* Déclaration des variables en float */
						printf("Premier chiffre : ");
						scanf("%lf", &operandeA);

						printf("Deuxieme chiffre : ");
						scanf("%lf", &operandeB);

						resultat = operandeA + operandeB;
						printf("Le resultat est : %lf\n", resultat);
					}
					
				}
			}
		}
	}
	else
	{
		if (operateur == 2) /* Si l'user choisi de faire une soustraction */
		{
			printf("Quel type :\n 1- Int32\n 2- Int64\n 3- Double\n 4- Float\n ");
			scanf("%d", &type);

			if (type == 1) /* Cette solution sera choisi si l'user prend le type 1 soit int 32 */
			{
				int32_t operandeA, operandeB, resultat; /* Déclaration des variables en int32_t */
				printf("Premier chiffre : ");
				scanf("%li", &operandeA);

				printf("Deuxieme chiffre : ");
				scanf("%li", &operandeB);

				resultat = operandeA - operandeB;
				printf("Le resultat est : %I32i\n", resultat);
			}
			else
			{
				if (type == 2) /* Cette solution sera choisi si l'user prend le type 2 soit int 64 */
				{
					int64_t operandeA, operandeB, resultat; /* Déclaration des variables en int64_t */
					printf("Premier chiffre : ");
					scanf("%I64i", &operandeA);

					printf("Deuxieme chiffre : ");
					scanf("%I64i", &operandeB);

					resultat = operandeA - operandeB;
					printf("Le resultat est : %I64i\n", resultat);
				}
				else
				{
					if (type == 3) /* Cette solution sera choisi si l'user prend le type 3 soit  double */
					{
						double operandeA, operandeB, resultat; /* Déclaration des variables en double */
						printf("Premier chiffre : ");
						scanf("%lf", &operandeA);

						printf("Deuxieme chiffre : ");
						scanf("%lf", &operandeB);

						resultat = operandeA - operandeB;
						printf("Le resultat est : %lf\n", resultat);
					}
					else
					{
						if (type == 4) /* Cette solution sera choisi si l'user prend le type 4 soit float */
						{
							float operandeA, operandeB, resultat; /* Déclaration des variables en float */
							printf("Premier chiffre : ");
							scanf("%lf", &operandeA);

							printf("Deuxieme chiffre : ");
							scanf("%lf", &operandeB);

							resultat = operandeA - operandeB;
							printf("Le resultat est : %lf\n", resultat);
						}
						
					}
				}
			}
		}
		else
		{
			if (operateur == 3) /* Si l'user choisi de faire une multiplication */
			{
				printf("Quel type :\n 1- Int32\n 2- Int64\n 3- Double\n 4- Float\n ");
				scanf("%d", &type);

				if (type == 1) /* Cette solution sera choisi si l'user prend le type 1 soit int 32*/
				{
					int32_t operandeA, operandeB, resultat; /* Déclaration des variables en int32_t */
					printf("Premier chiffre : ");
					scanf("%li", &operandeA);

					printf("Deuxieme chiffre : ");
					scanf("%li", &operandeB);

					resultat = operandeA*operandeB;
					printf("Le resultat est : %I32i\n", resultat);
				}
				else
				{
					if (type == 2) /* Cette solution sera choisi si l'user prend le type 2 soit int 64 */
					{
						int64_t operandeA, operandeB, resultat; /* Déclaration des variables en int64_t */
						printf("Premier chiffre : ");
						scanf("%I64i", &operandeA);

						printf("Deuxieme chiffre : ");
						scanf("%I64i", &operandeB);

						resultat = operandeA*operandeB;
						printf("Le resultat est : %I64i\n", resultat);
					}
					else
					{
						if (type == 3) /* Cette solution sera choisi si l'user prend le type 3 soit double */
						{
							double operandeA, operandeB, resultat; /* Déclaration des variables en double */
							printf("Premier chiffre : ");
							scanf("%lf", &operandeA);

							printf("Deuxieme chiffre : ");
							scanf("%lf", &operandeB);

							resultat = operandeA*operandeB;
							printf("Le resultat est : %lf\n", resultat);
						}
						else
						{
							if (type == 4) /* Cette solution sera choisi si l'user prend le type 4 soit float*/
							{
								float operandeA, operandeB, resultat; /* Déclaration des variables en float */
								printf("Premier chiffre : ");
								scanf("%lf", &operandeA);

								printf("Deuxieme chiffre : ");
								scanf("%lf", &operandeB);

								resultat = operandeA*operandeB;
								printf("Le resultat est : %lf\n", resultat);
							}
							
						}
					}
				}
			}
			else
			{
				if (operateur == 4) /* Si l'user choisi de faire une division */
				{
					printf("Quel type :\n 1- Int32\n 2- Int64\n 3- Double\n 4- Float\n ");
					scanf("%d", &type);

					if (type == 1) /* Cette solution sera choisi si l'user prend le type 1 soit int 32*/
					{
						int32_t operandeA, operandeB, resultat; /* Déclaration des variables en int32_t */
						printf("Premier chiffre : ");
						scanf("%li", &operandeA);

						printf("Deuxieme chiffre : ");
						scanf("%li", &operandeB);

						resultat = operandeA / operandeB;
						printf("Le resultat est : %I32i\n", resultat);
					}
					else
					{
						if (type == 2) /* Cette solution sera choisi si l'user prend le type 2 soit int 64*/
						{
							int64_t operandeA, operandeB, resultat; /* Déclaration des variables en int64_t */
							printf("Premier chiffre : ");
							scanf("%I64i", &operandeA);

							printf("Deuxieme chiffre : ");
							scanf("%I64i", &operandeB);

							resultat = operandeA / operandeB;
							printf("Le resultat est : %I64i\n", resultat);
						}
						else
						{
							if (type == 3) /* Cette solution sera choisi si l'user prend le type 3 soit double*/
							{
								double operandeA, operandeB, resultat; /* Déclaration des variables en double */
								printf("Premier chiffre : ");
								scanf("%lf", &operandeA);

								printf("Deuxieme chiffre : ");
								scanf("%lf", &operandeB);

								resultat = operandeA / operandeB;
								printf("Le resultat est : %lf\n", resultat);
							}
							else
							{
								if (type == 4) /* Cette solution sera choisi si l'user prend le type 4 soit int 64 */
								{
									float operandeA, operandeB, resultat; /* Déclaration des variables en float */
									printf("Premier chiffre : ");
									scanf("%lf", &operandeA);

									printf("Deuxieme chiffre : ");
									scanf("%lf", &operandeB);

									resultat = operandeA / operandeB;
									printf("Le resultat est : %lf\n", resultat);
								}
								else /* Erreur dans la saisie, le programme s'arrête */
								{
									printf("Erreur dans la saisie, il fallait saisir un chiffres a gauche du type\n");
								}
							}
						}
					}
				}

				// Calcul par modulo
				else
				{
					if (operateur == 5) /* Si l'user choisi de faire un modulo */
					{
						printf("Quel type :\n 1- Int32\n 2- Int64\n ");
						scanf("%d", &type);

						if (type == 1) /* Cette solution sera choisi si l'user prend le type 1 soit int 32 */
						{
							int32_t operandeA, operandeB, resultat; /* Déclaration des variables en int32_t */
							printf("Premier chiffre : ");
							scanf("%li", &operandeA);

							printf("Deuxieme chiffre : ");
							scanf("%li", &operandeB);

							resultat = operandeA%operandeB;
							printf("Le resultat est : %I32i\n", resultat);
						}
						else
						{
							if (type == 2) /* Cette solution sera choisi si l'user prend le type 2 soit int 64 */
							{
								int64_t operandeA, operandeB, resultat; /* Déclaration des variables en int64_t */
								printf("Premier chiffre : ");
								scanf("%I64i", &operandeA);

								printf("Deuxieme chiffre : ");
								scanf("%I64i", &operandeB);

								resultat = operandeA%operandeB;
								printf("Le resultat est : %I64i\n", resultat);
							}
							
						}
					}
					
				}
			}
		}

		return 0;
	}
}
