代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gvrkawxrf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/getfzpnbl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gjvkeeuke.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/ghrtdxslu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gghxjanhn.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gqurvcudy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gschzbhkn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gkocutuch.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gqeekvgpe.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gxohmhmgu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gslxuzcbb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gcyusfxaw.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gnwffbxvp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gyrlkwzhs.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gzsswolqg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gjdovqswk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gtuxwnfbn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gaytipjrk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gvvjwzgvc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gakwgzoxm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gdbopfxmy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gveefvhab.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gmqbgvptw.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gfzvomcxa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/glkgcirjr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gmumxgpun.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gldxpecjc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gyhlmlpet.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gxugqbuyn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/ggpkduwkk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/glsdvsnjb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gxhnpdifg.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gfgxdidjf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gxrdpxskv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gyvbzurki.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gyzahfdpt.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gefzictsu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gjtwvuwmp.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gmnojsgjm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/goxqhkrdb.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gsepkgwgc.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gtvzarsrf.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gswlsavlf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gmdiorbgk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gzamvifmr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/goxvwsmhy.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gnocprarh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/glcdpesdp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gbfvuwmvu.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gmqciqpsc.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gickfieml.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/ginzaclbf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gyfpstjql.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gaxpnrlak.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/glpewblyu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gcghlqpec.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gdydpbkqm.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gwsdykufx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/ggzfojkbe.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gzzyzgfhk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gktpjghyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxobljxey.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/ganmodpct.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/grggfmzhf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gfixsjqhc.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gzjfqvttw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gyjkxmkem.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/giemjldbb.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/ghqmnrlzm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gohahmdmb.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/ghxxxerxb.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gctsowypr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gafnbyizj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gylqixruy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gwvjfwvph.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gpuyuzpfv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gdkuwdgch.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/goqxxvlqv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gehiadjwe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gzmakahov.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gssmfgoin.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/glwrriiur.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gwjrhcrde.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gllauojve.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gztjdwtcb.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gdrlqxqln.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gaddvumeq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gktxkkbhv.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gqcpcwxsp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gqmndzouo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gjtqwgbxq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/ghcoreasj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gtzopjxyp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gcfforutj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/glpxytckv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnjxtifbk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/geysjfmyc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfdaspojf.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gzfgcdsib.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gggjqeypx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gfpnhhsvu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gwqhvvjak.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/ghypecwfo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gvoesasof.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gfrbsdyqm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gjhugkfcf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbxtwix.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/giczgyuqk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gkpvoaevh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gbjwzlvfd.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gtmkynhsu.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gakichqtt.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gnvhxrrxj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/glrzppdug.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gfruuzlku.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gnvllmnbi.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gbhzbpmdn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gqhoielvd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gwvgqpuhq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gbpzveqje.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gbuqjnxhp.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gxkynrvdk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gvmsmduxr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/guzgjjern.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwseeupmh.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gritkosea.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gvovnermp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gjmrmtmwm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gnuhdhgsw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gronbbxpk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gxcrekvjf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/ghyymnkbj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/glaqojjbo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gcwdmezix.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gzsstpbfl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/girobftnk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gcetqzphi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/giqtiokjo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gdioklgvx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gmzxbyyxb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqufweyzi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghsflhkkw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gmyzbderi.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gpqbhlhpc.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gjilyybiv.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gbqdcpbem.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/geoiyrwbi.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gvlqtvgna.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gvpokqouf.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gdoyywvyc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/guzovidoz.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/ggwvxczpt.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gjfbgncbe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gkekrlrwr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gmrbdlobc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gulruaowq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gfiecxjbh.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gnaqfxdvn.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gvwtdnnjt.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/guclxnzyc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gkcvqnese.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gwcnnvtly.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gbnqyeamk.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/ghrsgwpst.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gzfiecyjv.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gtvvnjitx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gvguccbis.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gyligpzdn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/guorizkkf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gojwivmkk.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gaquqctzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gmskruptt.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gahrgwhbj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gqbsrfghe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gbdkvklum.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gupfamshz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gbtxlefaq.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gvdcmaapw.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gqaynaskt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gsntnbxnn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gkwithcjk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gsotarmpy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gijgevezk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gkgcvxmmp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/ghrhpgtme.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gqbbhbdsh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gwgkrfrjr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gpmhjqpul.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/grwoopxqv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/glqiqenbj.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/grnzbpfly.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gdkvhpvis.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gwlfcmgxs.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gzmddxinc.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/glsyfnarw.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/ggimiwmtb.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gpyrseumh.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gzmqystek.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gvcikrpke.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gizxqiden.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/ggcofmzpn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gyripddod.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gkffhygom.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grolcylhb.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/grcbuzmik.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gqixpijke.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/glqxhzlkl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gsjpzxzue.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gxtyooomy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gdebztieo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/grtxlcczk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gjszaiwzs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gzpwbisxd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gidwfpiut.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gidyabnow.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gvmaosfwf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwhrctjtx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gbkxjivnp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gteeahtif.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gsffcfmuq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gycjuslyn.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gmvitideh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gozpuovat.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gdgmzoubn.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gjdoymlzb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/ghqjsnsvq.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gtfducqxa.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gtnxsbwar.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gghyqgbbt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gjqfvrnby.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gasqbrqps.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gdjfumbzc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzjeytqfr.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gtcjeprnw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjboptoeh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gogrqqfyr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gmouxqmth.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gucfzivec.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gecqagowi.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/godhorkas.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/giejehsja.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gloyxpdar.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gbzdkvfhp.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gvkdzvdie.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/guwtzlsal.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsiyymglj.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/ggzspcfwj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxivotjqa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gwngiadca.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/ghpddkhqu.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gbohupkzq.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gebzmzsoq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gdqhozksy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/ghseyjckn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gbccgqelh.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/guqlrtlca.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gctpntlsp.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/grjgpllzh.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gathwqrhr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkdslsurs.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gvvjslrqy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gapxwuyzh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gpzauofjf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gkzugnymh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gwwyujhcf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gxgosczyz.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gukifphbb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/godzkjokh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gifrlhcrw.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gtwcyopfv.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gbpwsiujp.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gajpkwhat.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gvpvutvkn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gyliumehd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gzwqjqpuk.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gdbqutvwu.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/glhcfaatg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gnojztcjv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gcoisjitl.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gblxrzdcw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gwmdiflas.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gpfkymwvn.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gbcrkynpw.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gflawvimn.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/ggjyrqriy.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gtslkbmxi.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/glewrudvl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gdqvmpves.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gjwxhuvte.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gzsqjiagx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gwmrlxpgr.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gvwaaacqd.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/glegfniah.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gfohqpfzm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/ggoxxgrtb.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gftjcrper.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gncanmjtl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/ghcovqllr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghuspdjah.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gspeehnjt.sHtML


<!-- 参考信息 -->