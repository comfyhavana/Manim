from manim import *

class BallFalling(Scene):
    def construct(self):
       
        ball = Circle(color=BLUE, radius=0.5)
        ball.move_to(3*DOWN)  
        floor = Line(start=LEFT, end=RIGHT, color=WHITE).shift(2*DOWN)

        self.add(ball, floor)  
        self.play(ApplyMethod(ball.shift, 4*DOWN), run_time=2)

        self.wait()  


