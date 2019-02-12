#
# This is the user-interface definition of a Shiny web application. You can
# run the application by clicking 'Run App' above.
#
# Find out more about building applications with Shiny here:
# 
#    http://shiny.rstudio.com/
#

library(shiny)
library(plotly)
library(ggplot2)
library(kohonen)
data(wines, package = "kohonen")
data <- as.data.frame(wines)

# Define UI for application
shinyUI(fluidPage(
  
  # Application title
  titlePanel("Display of dependence of flavonoid content on alcohol
             content in wines"),
  
  # Sow instruction
  mainPanel(
    tabsetPanel(
      tabPanel(h2("Instruction"),
               h3("This application is for viewing the dependence of"),
               h3("flavonoid content on the alcohol content in various"),
               h3("wines."),
               h3("Click the app tab."),
               h3("You must move the slider to indicate the number"),
               h3("of displayed wines."),
               h3("In addition, by hovering the mouse over a point on"),
               h3("the plot, you will get the exact characteristics of"),
               h3("this wine."),
               h3("Packeges used: shiny, plotly, ggplot2, kohonen")),
      br(),
      tabPanel(h2("Shiny Application"),
               h3("Move the slider."),
               h3("Mouse over point."),
               sliderInput("myslider", "A slider:", min = 1, max = 100, value = 10),
               plotlyOutput("myplot"))
    )
  )
))