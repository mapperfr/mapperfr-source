---
title: "Comment changer d'instance Mastodon"
author: Jérémy Garniaux
type: post
date: 2023-10-31
categories:
  - carnet
tags:
  - mastodon
  - tutoriel
---

Voici en quelques mots les étapes à suivre pour changer d'instance Mastodon - et, par exemple, nous rejoindre sur https://mapstodon.space!

- Sur votre ancien compte, dans **Préférences** > **Import et export** > **Demander vos archives**. Après un moment d'attente, vous pourrez télécharger l'archive ZIP ainsi créée (vous pouvez aussi attendre de recevoir le mail qui vous indiquera que votre archive est prête). Vous l'utiliserez plus tard pour réimporter certaines données qui n'ont pas été transférées.

- Créez un nouveau compte sur l'instance que vous souhaitez rejoindre.

- Dans ce nouveau compte, ajoutez un "alias" à votre ancien compte chez Zaclys. Dans **Préférences** > **Compte** > **Déplacement depuis un compte différent** (en bas de page) > **Créer un alias de compte**, indiquez l'adresse de votre ancien compte.

![](albums/carnet/mastodon-migration/mastodon-migration-1.png)

- Depuis votre ancien compte, rendez vous dans **Préférences** > **Compte** > **Déplacement *vers* un compte différent**:

![](albums/carnet/mastodon-migration/mastodon-migration-2.png)

Une fois que ce paramètre est réglé, l'ensemble de vos abonné.es seront également abonné.es au nouveau compte (je crois qu'ils et elles restent abonné.es à l'ancien, mais ça c'est à vérifier, j'ai un doute). Pour le reste (vos abonnements, les contacts bloqués ou masqués, par exemple), il faut réimporter les données que vous aurez exportées en CSV en début d'opération.

- Pour ce faire, Rendez-vous dans **Préférences** > **Import et export** > **Import de données**, et versez ici le fichier téléchargé à la première étape. Le traitement de ce fichier peut prendre un certain temps, c'est normal si vous anciens abonnements n’apparaissent pas immédiatement. De même, si certains comptes auxquels vous étiez abonné n'acceptent pas automatiquement les nouvelles demandes d'abonnement, il faudra attendre qu'ils valident cette demande avant de les retrouver dans votre liste d'abonnements.

Vous pourrez ensuite choisir de supprimer l'ancien compte, ou de le conserver -  je vous suggère plutôt la première option pour plus de clarté par rapport à vos abonné.es. En attendant, votre ancien compte sera "grisé" et un message de redirection indiquera aux personnes le visitant que vous avez migré vers une nouvelle instance.