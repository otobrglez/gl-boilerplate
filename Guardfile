# https://gist.github.com/1610551

guard 'compass' do
  # watch('^src/(.*)\.s[ac]ss')
  watch %r{(.*)\.s[ac]ss$}
end

guard 'coffeescript', :input => 'src/coffeescripts', :output => 'public/javascripts'

guard 'livereload', :apply_js_live => true, :apply_css_live => true do
  watch %r{public/javascripts/.*\.js}
  watch %r{public/stylesheets/.*\.css}
  watch %r{public/*\.html}

  #watch(%r{app/views/.+\.(erb|haml|slim)$})
  #watch(%r{app/helpers/.+\.rb})
  watch %r{public/.+\.(css|js|html)}

  watch %r{src/.+\.(css|js|html|haml)}

  #watch(%r{config/locales/.+\.yml})
  # Rails Assets Pipeline
  #watch(%r{(app|vendor)/assets/\w+/(.+\.(css|js|html)).*})  { |m| "/assets/#{m[2]}" }
end

guard 'haml', :input => 'src', :output => 'public' do
  watch(/^.+(\.html\.haml)/)
end
