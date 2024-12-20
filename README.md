I am doing a C++ Hacksprint project. I am going to use the Qt to build an image app with the theme of Waves.

QUESTIONS
1. How does your application fit the project theme? - The application visually represents the theme of "waves" by dynamically drawing sinusoidal wave patterns, which are a fundamental representation of many types of waves, such as sound waves, light waves, and water waves. The interactive sliders allow users to adjust the frequency and amplitude of the wave, providing a visual and intuitive connection to the theme.
2. At a high level, what is your application? - The application is a wave visualizer built with Qt. It uses a custom drawing widget to render sinusoidal wave patterns in real-time. Users can control the appearance of the wave through sliders that adjust its frequency and amplitude. This application serves as a basic demonstration of wave behavior and interaction.
3. How did you design your application? - Architecture: The class MainWindow serves as the main container for the user interface. It includes components like sliders, labels and so on.
The custom class DrawingWidget serves as an area of drawing the sinusoid. Interaction: Slider that user can use for changing the value of frequency or amplitude that directly influence the sinusoid.
Design: The class QGradient provides possibility to draw the backgrount color to gradient and QPen to draw a dash line that helps to keep the center of drawing area.
4. Flowchart your application Start -> Initialize Application: creating mainwindow that contains all of compenents and initializing other components -> Displaying the whole application -> User interaction: userAdjust sliders → Emit signals to WaveWidget. WaveWidget updates frequency/amplitude -> Render sinusoid -> End
5. Explain particularly challenging pieces of your application - Updating the wave in real-time while ensuring smooth rendering was challenging. It required a good understanding of the paintEvent lifecycle and efficient use of QPainter
6. Summary of your learning takeaways -> Learning how to use Qt - Custom Drawing in Qt: Learned how to implement custom widgets with QWidget and override paintEvent for rendering dynamic visuals. Mathematical Visualization: Understood how mathematical functions (like sine) can be translated into graphical representations. UI Design in Qt: Practiced creating a structured GUI with sliders and dynamically updating widgets. Also I created the project on a PC that uses Linux and ended up getting a new laptop, a Mac, so figuring out how to transfer the project to my Mac and have it work the same.


![IMG-64a58df3c4f44df31e7b78a010593f3c-V](https://github.com/user-attachments/assets/f0d95323-63bb-4c93-8cf3-746d827dd97f)
