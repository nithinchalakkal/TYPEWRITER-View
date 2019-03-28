# Typewriter-Textview
How to do text writing animation? 

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
          
