---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: Seja bem vindo(a)!
      image:
        filename: icon23.png
      cta:
        label: '**Acesse os materiais aqui**'
        url: https://dharaavelinoalves.netlify.app/#projects
      cta_alt:
        label: Entre em contato
        url: https://dharaavelinoalves.netlify.app/#contact
      text: |-
        Este é um espaço onde compartilho um pouco sobre minhas pesquisas, scripts e tudo que envolve ciência, bioestatística e bioinformática.
        {style="text-align: justify;"}

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
  - block: about.biography
    id: about
    content:
      title: Bibliografia
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    content:
      title: Habilidades
      items:
        - name: Bioestatística
          icon: chart-line
          icon_pack: fas
        - name: Bioinformática
          icon: laptop-code
          icon_pack: fas
        - name: Genética
          icon: dna
          icon_pack: fas
  - block: experience
    content:
      title: Experiência
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Mestranda
          company: Laboratório de Sistemas de Engenharia de Saúde
          company_url: ''
          company_logo: peblogo
          location: PEB COPPE UFRJ
          date_start: '2022-08-01'
          date_end: ''
          description: |2-
              Responsabilidades:

              * Processamento de dados ômicos, com ênfase em metagenômica
              * Análise inteligente de dados 
              * Desenvolvimento de modelos para predição gênica
              * Elaboração de artigos e relatórios 
              * Apresentação em congressos e seminários
        - title: Aluna de Iniciação Científica
          company: Laboratório de Biossistemática de Anfíbios
          company_url: ''
          company_logo: uniriologo
          location: UNIRIO
          date_start: '2020-08-01'
          date_end: '2021-08-01'
          description: |2-
              Responsabilidades:

              * Classificação de anuros através de sílabas de vocalização
              * Análise bioestatística 
              * Desenvolvimento de modelos de aprendizado de máquina 
              * Elaboração de artigos e relatórios 
              * Apresentação em congressos e seminários
        - title: Aluna de Iniciação Científica
          company: Departamento de Métodos Quantitativos
          company_url: ''
          company_logo: uniriologo
          location: UNIRIO
          date_start: '2019-08-01'
          date_end: '2021-08-01'
          description: |2-
              Responsabilidades:

              * Desenvolvimento de abordagens estatísticas utilizando o Software R 
              * Análise bioestatística 
              * Desenvolvimento de modelos de aprendizado de máquina 
              * Elaboração de artigos e relatórios 
              * Apresentação em congressos e seminários
        - title: Aluna de Iniciação Científica
          company: Laboratório de Taxonomia de Poríferos
          company_url: ''
          company_logo: mnlogo
          location: Museu Nacional UFRJ
          date_start: '2019-08-01'
          date_end: '2021-08-01'
          description: |2-
              Responsabilidades:

              * Desenvolvimento de pesquisa utilizando caracteres morfológicos, moleculares e técnicas bioestatísticas para a classificação taxonômica de esponjas marinhas
              * Curadoria de coleção líquida do Filo Porifera
              * Desenvolvimento de artes digitais voltadas para divulgação científica através do Software Adobe Photoshop
              * Elaboração de artigos e relatórios 
              * Apresentação em congressos e seminários
                
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Pesquisas
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projetos
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: Todos
          tag: '*'
        - name: Bioestatística
          tag: Bioestatística
        - name: Bioinformática
          tag: Bioinformática
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Galeria
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Publicações
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Apresentações
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: contact
    id: contact
    content:
      title: Contato
      subtitle:
      text: |-
        Entre em contato comigo.
      # Contact (add or remove contact options as necessary)
      email: dharaavelino@gmail.com
      appointment_url: 'https://calendly.com/dharaavelinoalves'
      address:
        street: Av. Horácio Macedo 2030, Centro de Tecnologia, COPPE/UFRJ, Bloco H, 3° andar UFRJ - Ilha do Fundão
        city: Rio de Janeiro
        postcode: '21941-914'
        country: Brazil
        country_code: BR
      office_hours:
        - 'Segunda-feira 09:00 às 17:00'
        - 'Sexta-feira 09:00 às 17:00'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---

