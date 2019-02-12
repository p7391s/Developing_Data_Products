#
# This is the server logic of a Shiny web application. You can run the 
# application by clicking 'Run App' above.
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

# Define server for application
shinyServer(function(input, output, session) {
  
  dat <- reactive(data[1:input$myslider,])
  
  output$myplot <- renderPlotly({
    g <- ggplot(dat(), aes(alcohol, flavonoids)) +
      geom_point(color = "red")
    g <- ggplotly(g)
    g
 
  })
  
})