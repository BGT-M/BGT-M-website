---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
        大图挖掘
        研究组
      image:
        filename: welcome.jpg
      text: |
        <br>
        你好，这里是大图挖掘组
#         The **Wowchemy Research Group** has been a center of excellence for Artificial Intelligence research, teaching, and practice since its founding in 2016.
  
  - block: collection
    id: Publications
    content:
      title: Publications
      text: |-
        {{% callout note %}}
        🔍 Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: false
      offset: 0
      order: desc
    design:
      columns: '2'
      view: Citation
      
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      count: 5
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
      
  - block: portfolio
    id: projects
    content:
      title: 开源项目
      filters:
        folders:
         - post
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: 图方向
          tag: 'graph'
        - name: 大模型方向
          tag: 'LLMs'
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase 
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false



  - block: people
    id: peoples
    content:
      title: Meet the Team
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          - Principal Investigators
          - Researchers
          - Grad Students
          - Administration
          - Visitors
          - Alumni
      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: true
      show_role: true
      show_social: true



  - block: accomplishments
    id: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: '获奖'
      id: accomplishments
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      items:
        - certificate_url: 
          date_end: ''
          date_start: '2021-12-01'
          description: ''
          organization: THU
          organization_url: 
          title: 进步奖
#          url: ''
        - certificate_url: 
          date_end: ''
          date_start: '2023-10-01'
          description: '' 
          organization: THU
          organization_url: 
          title: 'Best paper'
          url: ''
        - certificate_url: 
          date_end: ''
          date_start: '2022-02-01'
          description: '' 
          organization: microsoft
          organization_url: https://openi.org.cn/
          title: 微软学者
          url: ''


      
  - block: tag_cloud
    id: Topics
    content:
      title: 词云
    design:
      columns: '1'
      background:
        gradient_start: '#eef2f3'
        gradient_end: '#eef2f3'
        gradient_angle: 180
        text_color_light: false
        
  - block: markdown
    content:
      text:
        |-
        <div style="display: flex; justify-content: center; align-items: center;">
          <img src="ucas.png" style="width: 15%; height: auto; margin: 0 5%;" alt="UCAS">
          <img src="UCAS_.png" style="width: 35%; height: auto; margin: 0 5%;" alt="UCAS Long">
          <img src="ict.png" style="width: 15%; height: auto; margin: 0 5%;" alt="ICT">
        </div>
    design:
      columns: '1'
      background:
        gradient_start: '#eef2f3'
        gradient_end: '#f7f7f7'
        gradient_angle: 180
        text_color_light: true
---