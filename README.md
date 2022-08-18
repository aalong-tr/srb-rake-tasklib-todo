# Steps to reproduce
1. `bundle install`
2. `tapioca gem`
3. `tapioca todo`
4. `srb tc` 

# Observed output
```
sorbet/rbi/gems/yard@0.9.28.rbi:11713: The super class Rake::TaskLib of YARD::Rake::YardocTask does not derive from Class https://srb.help/5067
       11713 |class YARD::Rake::YardocTask < ::Rake::TaskLib
              ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    sorbet/rbi/todo.rbi:9: Rake::TaskLib defined here
     9 |module ::Rake::TaskLib; end
        ^^^^^^^^^^^^^^^^^^^^^^
Errors: 1
```

