## A blog write by erlang.

#### Dependency

* [rebar 2](https://github.com/rebar/rebar)
* [ChicagoBoss master](https://github.com/ChicagoBoss/ChicagoBoss)
* [typescript](http://www.typescriptlang.org/)
* [scss](http://sass-lang.com/)
* [theme](http://lessmade.com/themes/less/)

#### Usage

```ruby
git clone git@github.com:FlowerWrong/erlblog.git
cd erlblog

# Install scss, typescript lint and compile tools.
npm install -g typescript
npm install -g tslint
bundle install

# Install rebar, following up link.
rebar -h
rebar g-d
rebar compile

# test
rebar boss c=test_functional
rebar boss c=test_eunit

# dev server
./init-dev.sh
q().

# production server
./init.sh start
./init.sh stop

# hot code reload
rebar compile
init.sh reload
```
