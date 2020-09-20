# Ivan Guzikov

## My contacts

* [telegram](http://t.me/gooanq)  
* [E-mail](mailto:rawzyxhz@gmail.com)  
* [GitHub](https://github.com/gooanq)

## Summary

I am interested in programming. I have been studing in for four years at the university. Now I want to begin serious studing of web technologies and become web developer. I have some basic knowledge and i hope it will help me to reach my goal.

## Skills

During my studies at the university i got some skills at:
* C# and WinForms
* C++
* OOP
* SQL (postgreSQL and MySQL)

Also have basic skills at: 
* HTML 
* CSS
* JavaScript and TypeScript

## Code example

My latest university project: Game in 15

```C#
private void CreateField()
        {
            Random rand = new Random();
            playField = new NumberBox[HORIZONTAL, VERTICAL];
            Size size = new Size(BOXSIZE, BOXSIZE);
            List<int> numbers = new List<int>();
            for (int i = 0; i < EMPTY; i++)
                numbers.Add(i);



            int xStart = 10;
            int yStart = 10;
            int space = 10;
            int x = xStart, y = yStart;

            for (int i = 0; i < VERTICAL; i++)
            {
                for (int j = 0; j < HORIZONTAL; j++)
                {
                    int number = rand.Next(0, numbers.Count);
                    int value = numbers[number] + 1;
                    var numberBox = new NumberBox(i, j, value, size);
                    numbers.RemoveAt(number);
                    numberBox.Location = new Point(x, y);


                    this.Controls.Add(numberBox);
                    playField[i, j] = numberBox;
                    numberBox.Show();
                    x = x + space + BOXSIZE;

                    if (value == EMPTY) continue;


                    numberBox.Click += (sender, e) =>
                    {
                        if (chosen != null)
                            chosen.BackColor = Color.GreenYellow;
                        numberBox.BackColor = Color.Orange;
                        chosen = numberBox;
                    };

                }
                x = xStart;
                y = y + BOXSIZE + space;
            }

            timer.Start();
        }
```

## Experience

I got some experience in programming by doing labs and course project at the university. [Here my last](https://github.com/gooanq/Game15) I am searching for new experience in web-developing now.

