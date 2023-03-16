# Football-League-Manager


This is a simple football league management system implemented using classes `Team`, `FootballLeague`, and `Dashboard`. The system allows you to manage teams, maintain their standings, and perform various operations like adding, removing, and updating teams' stats.

## Class Descriptions

### Team

The `Team` class represents a football team and stores the team's name, number of wins, draws, and losses, as well as the number of points. The points are recalculated every time the number of wins, draws, and losses is updated. A team is awarded 3 points for every win, 1 point for every draw, and 0 points for every loss. The class provides a human-friendly representation of the team (toString()) and supports total ordering of teams (teams are Comparable).

### FootballLeague

The `FootballLeague` class represents a football league and stores a list of `Team` objects included in the league. The list is maintained in descending order based on teams' points. The class allows teams to be inserted (adding a new team) and removed (deleting an existing team) at any point. It also allows updating a team's position in the league by updating the team's wins, draws, and losses (changes to points must be reflected in the ordering of the list). Teams can be relegated at the end of the season (i.e., the 3 teams with the least amount of points). The league table (i.e., list of teams) should be printed after every change takes place.

### Dashboard

The `Dashboard` class is responsible for creating a `FootballLeague` instance and subsequently inserting, updating, removing, and relegating teams.

## Usage

1. Clone this repository
2. Compile and run the main class (`Dashboard`)
3. Follow the prompts to insert, update, remove, or relegate teams
4. The league table will be printed after every change takes place

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository
2. Create a new branch with your feature or bug fix
3. Commit your changes and push them to your fork
4. Create a pull request to this repository

## License

This project is released under the MIT License. Please see the `LICENSE` file for more details.
