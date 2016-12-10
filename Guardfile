guard :shell do
  watch %r{^(Rakefile|.+\.md)$} do |m|
      puts ">>> #{m[0]} changed"                                                    
      puts `rake`                                                                   
      puts ">>> Done!" 
  end
end
