# Typewriter-Textview
How to do text writing animation? 
In Android Development we do not have the option to use any other custom font in our default TextView in an xml layout file, except from the default Roboto font.

And the choices that Android gives us are limited, by letting us set only normal, sans, serif or monospace fonts, which are usually not enough, especially when we want to customise our application.

In this example we are going to make a custom Android TextView that can change its font, by customising its attributes from the xml.

Usage 
========

How to Include an External .aar File Using Gradle?

Step 1. File -> New -> New Module -> Import .jar/.aar and import your .aar.

Step 2. Then in your project’s build.gradle (the one under ‘app’) add the following:

Step 3: dependencies { compile project(‘:Name-of-the-Project’) }

Step 4: Clean Build after all the above steps


In XML
========

        <Nithinchalakkal.TypeWriterEffect
        android:id="@+id/tv"
        android:layout_width="wrap_content"
        android:layout_height="50dp"
        android:text=""
        android:textColor="@color/colorAccent"
        android:textSize="23sp"
        />


In Activity
============

      TypeWriterEffect typeWriter;
			typeWriter= (TypeWriterEffect) findViewById(R.id.tv);
			typeWriter.TypeWriterEffect(MainActivity.this,
			"I Just Implimented The Typing effect",
			100,
			FontFamily.Montserrat_UltraLight_0,false,true);
          
