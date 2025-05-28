# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: skasmi <skasmi@student.42.fr>              +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/02/27 17:23:32 by skasmi            #+#    #+#              #
#    Updated: 2025/05/27 21:33:33 by skasmi           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #


.PHONEY : up down re fclean

up:
	cd srcs && docker-compose up --build

down:
	cd srcs && docker-compose down

re:
	cd srcs && docker-compose down
	cd srcs && docker-compose up --build

fclean:
	docker system prune --all --force
	docker rm -f $(docker ps -aq)
	