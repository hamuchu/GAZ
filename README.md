# GAZ
## memo
- valueの教師は、セルフプレイの最終的なスコア。policyの教師はセルフプレイに使用したモンテカルロ木探索の訪問回数
- policyの教師になるモンテカルロ木探索の訪問回数に、温度パラメータと呼ばれる N()^1/γ/ΣN()^1/γ　で1/γ乗したものをかけてあげる。そのことにより、policyの選択に変化をつけることができる。なお、γ=1のときは、訪問回数に比例して、policyの教師になる。γ=0.1の時は、１０乗されるので、より訪問回数の多い手が強調され、大きな値になる。
- 試合の時に、木探索をする時はルートノードにおいて、探索の訪問回数が多い手をベストな手として選択することになる。
## references

- https://postd.cc/alphago-zero-how-and-why-it-works/
- http://tadaoyamaoka.hatenablog.com/entry/2017/10/21/174532
- http://tadaoyamaoka.hatenablog.com/entry/2017/12/07/223710
- https://web.stanford.edu/~surag/posts/alphazero.html

## English references
- https://web.stanford.edu/~surag/posts/alphazero.html

##  Repository
- https://github.com/suragnair/alpha-zero-general
- https://github.com/junxiaosong/AlphaZero_Gomoku
