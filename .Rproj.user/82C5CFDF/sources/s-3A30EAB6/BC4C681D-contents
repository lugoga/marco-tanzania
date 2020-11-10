require(tidyverse)
require(lubridate)
require(plotly)
require(shiny)
require(shinythemes)


ui = fluidPage(
        navbarPage(title = "marcoSouth", theme = shinytheme("flatly"),
                   tabPanel(title = "Temperature",
                            sidebarLayout(
                                sidebarPanel(width = 2,
                                             selectInput(inputId = "Site",
                                                         label = "Monitoring Station",
                                                         choices = c("NUNGWI", "PEMBA", "TANGA"),
                                                         selected = "NUNGWI"),
                                             tags$img(src = "semba_zoom_logo.svg")),
                                mainPanel(
                                    fluidRow(
                                        column(width = 6, plotlyOutput(outputId = "today", width = "100%", height = 300))
                                    )
                                )
                            )),
                   tabPanel(title = "Chlorophyll"),
                   tabPanel(title = "Wind"),
                   tabPanel(title = "Air temperature"),
                   tabPanel(title = "Rainfall"),
                   tabPanel(title = "Cloud"),
                   tabPanel(title = "About",
                            sidebarLayout(
                                sidebarPanel(width = 2,
                                             tags$img(src = "climate_bangwe_mnazi.jpg")
                                ),
                                mainPanel(
                                    fluidRow(
                                        column(width = 11, 
                                               tags$div(
                                                   tags$h3("Abstract"),
                                                   "The MarCOSouth project is strongly aligned to the South African National Oceans and Coastal Information Management System (OCIMS). OCIMS has consolidated South African observational and forecasting expertise through the development of a range of services that are very similar in scope to those proposed for GMES and Africa.",
                                                   tags$br(),
                                                   tags$img(src = "bangwe_climate.jpg", width = "800px", height = "338px"),
                                                   
                                                   tags$br(),
                                                   tags$h3("Background"),tags$br(),
                                                   "Tanzania has a beautiful coastal plains, which are traversed with permanent and seasonal rivers and numerous creeks. These rivers include Pangani, Ruvu, Wami, Rufiji, Mbemkuru and Ruvuma, which discharge waters into the Indian Ocean and influence the coastal environment through creation of productive brackish water enviroment in estuaries, maintanance of deltas. tidal flats and shorelines and nourish mangroves and seagrass beds.",
                                                   tags$br(),
                                                   "The coasta is one of the country's most valuable natural resources. The coastal resources contribute significantly to the national income and provide social and economic benefits to the population. These coastal areas is characterized by a wide diversity of habitats inclduing sandy beaches, rock outcrops, coral reefs, estuarine systems, bays, extensive mangrove stands and seagrass beds. Its continental shelf is narrow with the 200 m depth contour at about 4 km from shoreline, except at the Mafia and Zanzibar Channels where the shelf width reaches up to 60 km. ",
                                                   tags$br(),
                                                   "A key value proposition of OCIMS is the powerful, scalable service development methodology; this identifies archetypal users, beneficiaries, policies, usage scenarios, as well as functional requirements.",
                                                   tags$br(),
                                                   tags$img(src = "kibirizi.jpg", width = "800px", height = "466px"),
                                                   tags$br(),
                                                   
                                                   tags$h3("Objectives"),
                                                   "The core objective of MarCoSouth is to provide new decision-making services that facilitate to promote sustainable management of marine resources and marine governance and also to stimulate regional growth of blue economy",tags$br(),
                                                   tags$h4("Specific objectives"),
                                                   "1. To improve regional capacity of decision and policy makers",tags$br(),
                                                   "2. To Further develop, implement and assess the impact of national, regional, and continental marine and maritime policies: through user focused services using earth observations and forecast data",tags$br(),
                                                   "2. Improve our understanding of climate-driven changes in coastal ecosystem and fisheries productivity.", tags$br(),
                                                   "3. Gather essential data that will help  to develop coastal and marine models and to inform local citizens, especially small-scale fishermen, of ocean conditions to promote sustainable fisheries.",
                                                   tags$br(),
                                                   
                                                   tags$h3("Focus area of the Project"),
                                                   tags$a(href = "https://en.wikipedia.org/wiki/Lake_Tanganyika", "Lake Tanganyika"), "is an African Great Lake. It is estimated to be the second largest freshwater lake in the world by volume, and the second deepest, in both cases, after only Lake Baikal in Siberia, it is also the world's longest freshwater lake. The lake is divided among four countries - Tanzania, the Democratic Republic of the Congo, Burundi, and Zambia, with Tanzania (46%) and the DRC (40%) possessing the majority of the lake. The water flows into the Congo River system and ultimately into the Atlantic Ocean.",
                                                   tags$br(),
                                                   
                                                   tags$h3("Coastal monitoring"),
                                                   "Tanzania is one of the most important countries in Africa for biodiversity, ranking high in the number of species of different living organisms. A wide range of important and values species is found in the coasta and marine enviroment. These includes and estimated 127 species of coral reefs",
                                                   
                                                   tags$br(),
                                                   tags$br(),
                                                   tags$br(),
                                                   tags$h4("Authors"),
                                                   tags$a(href = "https://semba-blog.netlify.app/", "Mr. Masumbuko Semba"), " from the Nelson Mandela African Institution of Science and Technlogy, Arusha, Tanzania",tags$br(),
                                                   "Dr. Yohanna Shaghude, Institute of Marine Sciences, Zanzibar, Tanzania",tags$br(),
                                                   "Mr. Kelvin Kamnde, Institute of Marine Sciences, Zanzibar, Tanzania",tags$br(),
                                                   "Mr. Faki Faki, Institute of Marine Sciences, Zanzibar, Tanzania",tags$br(),
                                                   "Ms. Violeth , Institute of Marine Sciences, Zanzibar, Tanzania",tags$br(),
                                                   "Ms Hellen Kizenga, Institute of Marine Sciences, Zanzibar, Tanzania",tags$br(),
                                                   "Ms. Moza Moza, Institute of Marine Sciences, Zanzibar, Tanzania",tags$br(),
                                                   tags$br(),tags$br(),tags$h4("Contact"),
                                                   "lugosemba@gmail.com",tags$br(),tags$br(),
                                                   tags$img(src = "semba_zoom_logo.svg", width = "190px", height = "194px"), tags$img(src = "semba_zoom_logo.svg", width = "190px", height = "194px")
                                               )
                                        )
                                    )
                                )
                            )
                   )
                   )
    
    
)

server = function(input, output){
    
}

shinyApp(ui = ui, 
         server = server
         )