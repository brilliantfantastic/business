desc "Converts a markdown document to the specified format"
task :convert, [:document] do |t, args|
  require "launchy"
  require "pandoc-ruby"

  path = Pathname.new(args[:document])
  output_path = "output/#{path.basename.to_s.gsub(path.extname, ".pdf")}"

  file = File.join(File.dirname(__FILE__), args[:document])
  converter = PandocRuby.new([file],
                             { from: :markdown, to: :latex, o: output_path },
                             :smart, :preserve_tabs)
  converter.convert

  Launchy.open output_path
end
