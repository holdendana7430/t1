代发 wailian999

Py:   def add(a, b): return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gdzlxrfea.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/guxbqrgml.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/goasumqrr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gznvcwyry.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grhezhtdv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrqlxuod.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fanxiaobao.xyz/Article/details/gkijmmzmz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtofebwpq.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbwedbrd.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fanxiaobao.xyz/Article/details/gcswigwns.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzdonweqg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxomtaeht.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepqiooni.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fanxiaobao.xyz/Article/details/gnatbkkfa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbkfthjow.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpbfbljw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbnjycpf.sHtML

[C03] 可变参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgdpwzda.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvryzxgra.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyuqnsyi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzwtjfyxp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/goougywak.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gexnlpjbj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwbkzuqk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fanxiaobao.xyz/Article/details/goukhgkhy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxqockok.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwpcqcrx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggljuurzh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifaptfbm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gaefvyezp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbrfzpho.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqldwvio.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyupmpvuf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmsxmjeyd.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/giprykhyy.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/gpjxbjgiz.sHtML

Py:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfzovqje.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvwkocrz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/glhdnfdgg.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbubpjfm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdwiwttv.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcomgfdf.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gpfeuyfwf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/gntyqduyd.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gexnrsakj.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fanxiaobao.xyz/Article/details/gihvwwsju.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmntwatqf.sHtML

JS:   const square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gycumocws.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gtjecrfds.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxddgbwzs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gfjhbyvpt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/galbivgqc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gteznyiae.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fanxiaobao.xyz/Article/details/gndvigyjx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtktguxuc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gahhrnlac.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpjvjsru.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpwsjsyi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhgzqauc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtwclxiz.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnakpjllz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxsxcfho.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijlbtbre.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfepqzkva.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glbmkunrq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grlucmdyu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geqamhdtk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxkxticf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvdypjha.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gevvfgnow.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyakkxfh.sHtML

[C09] 递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrbnxwpg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqqnawaz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/goqyksmjq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gsexxwhvj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/getrqacqk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/geakyuybb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gakjlzxvm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkziztxhz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvzuttoh.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/graspojgf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/gwweuersi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/gosunwqnk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gdfdcoraw.sHtML

TS:   同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/guepndnkp.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gapglzlbc.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/glqhunkxy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdydopgl.sHtML

C#:   块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gczoprzub.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcqaturs.sHtML

Py:   from module import func
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkmbyqdx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gigogwhwc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyeslntw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfzqriqh.sHtML

Java: import java.util.List;
来源：http://blog.fanxiaobao.xyz/Article/details/ghifumtry.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrfvmvil.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fanxiaobao.xyz/Article/details/gvspjfvde.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gekthjlxl.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/gbwyppvlz.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/grffvgfzd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fanxiaobao.xyz/Article/details/gmufvfurx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/garxkbxgd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/ggutkkkft.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fanxiaobao.xyz/Article/details/gknqzowox.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gtmtelaws.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fanxiaobao.xyz/Article/details/gmlgjwxkb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqxciqggw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fanxiaobao.xyz/Article/details/geceymfns.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gsamkgopc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqxrkuniy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcxzhblg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhfhukbn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskozzcko.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajmwoqpr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhhddlpv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fanxiaobao.xyz/Article/details/gcplrfzxs.sHtML

[C14] 泛型函数
来源：http://baike.fanxiaobao.xyz/Article/details/gosfuvrqk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/gzohcouwh.sHtML

PHP:  // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxhehsti.sHtML

JS:   // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlpxydvc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gifdgikaf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gsugdoutd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fanxiaobao.xyz/Article/details/gcsffcccw.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gcmpxtqaz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fanxiaobao.xyz/Article/details/gyjfhqvvd.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fanxiaobao.xyz/Article/details/gooljmbwl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fanxiaobao.xyz/Article/details/gdvsivqyg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gailjqcrv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ggyauhaxo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztohskth.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfgaqsjb.sHtML

Go:   // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggylbwywg.sHtML

Ruby: a, b = pair
来源：http://3g.fanxiaobao.xyz/Article/details/gcefwgpbr.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gcxzhfuji.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fanxiaobao.xyz/Article/details/gifqlwsyp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gfsurwuqy.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmkhfefj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fanxiaobao.xyz/Article/details/grxkxcmoi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/ggahwreec.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmyvqhyyx.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/gwvxbevwu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatdcmshe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbffyfag.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbtidoktn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuccgrkt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmmugjvy.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gaalhnwnu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fanxiaobao.xyz/Article/details/gbattqmcf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyvwzanv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzflntnjw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsfwxpos.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fanxiaobao.xyz/Article/details/gylxhnunk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqanmnfpo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/girjjcqwp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fanxiaobao.xyz/Article/details/gckswkzeh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/glvxpzlyn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/grwqfzabl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gskzaitic.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ggsuyepis.sHtML

TS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpxmfoxb.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gclahotax.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnckxnwxs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fanxiaobao.xyz/Article/details/gvqlhjtbv.sHtML

C#:   list.Add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpkubtjc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvrgzecu.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/ghzbfskpc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fanxiaobao.xyz/Article/details/grcczxygs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fanxiaobao.xyz/Article/details/glxxrrgvm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gmztunlla.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gosbjmbfv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gggytxfsc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fanxiaobao.xyz/Article/details/gitumzptl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwvvudtl.sHtML

[D04] 删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkbeufle.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqujxelt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyxqxtun.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fanxiaobao.xyz/Article/details/gegudoqwq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gqfutpqbi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkmvavwa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fanxiaobao.xyz/Article/details/gdajkiiol.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjpiljul.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/geavwkuin.sHtML

[D05] 访问与修改元素
来源：http://blog.fanxiaobao.xyz/Article/details/gmlrvbsqk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gzqldvsrs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gadoquwrj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gvcnpwfxz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fanxiaobao.xyz/Article/details/gzpylvveg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehphbtet.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdqjgafu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscbyqvhi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/grbzwrvdm.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbijmlioo.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gejzldogp.sHtML

PHP:  count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/grbtyygit.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gavguehdp.sHtML

TS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/gljobeagw.sHtML

Java: list.size();
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlwyjayy.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/guckiyxbv.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/ggujjeqap.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnnftiri.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpekrrtbw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fanxiaobao.xyz/Article/details/gkobntcwn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzuapbiq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbgynvwi.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/grpfvmfez.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gacjmrcjt.sHtML

Go:   arr[1:4]
来源：http://3g.fanxiaobao.xyz/Article/details/glemlhuyy.sHtML

Ruby: arr[1, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/gzbprtnyt.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gzhitxtnx.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdksbervr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrswctys.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvyaaazo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/glfbldffc.sHtML

TS:   [...a, ...b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnlhlqxu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gonfbvcsy.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gkmovpuqd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gnnqewqpf.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gatwtkngt.sHtML

[D09] 排序（升序）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnvqvfwv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gegviqemm.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/glrizfszv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/gvwbvpigf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdyppcur.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsfjitbc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gbcrmkfpm.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwxxkxfw.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqpgmgtu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fanxiaobao.xyz/Article/details/gubowwlbi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gdniyscmy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gloxrtybo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/geinnkzoe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvifalen.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjmhdjko.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/guipzcekq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcoibopx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/gqwisvmju.sHtML

[D11] 反转数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfisczep.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/gsalbmgpw.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gwpstelrc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfmypfry.sHtML

TS:   [...arr].reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/ghhtirzmr.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkvoljbi.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwckfmxqi.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gvybvzboc.sHtML

C#:   list.Reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoopplmg.sHtML

[D12] 查找元素下标
来源：http://baike.fanxiaobao.xyz/Article/details/gjowygxky.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgsfamql.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsalivlu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggstfiwkq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbttoecgw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fanxiaobao.xyz/Article/details/guukpikgy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpejechh.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/guxvaxjlq.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fanxiaobao.xyz/Article/details/gwyamjmag.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghseujuyq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gqjcqpmdn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/grvakidcw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/ghrovkfkj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzddason.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxotlglg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fanxiaobao.xyz/Article/details/getzvbhln.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwkihjnn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gwxfpzqad.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fanxiaobao.xyz/Article/details/ghmitczsm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geooruuzf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbzozvfp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwebvwajl.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gfrnkcdvv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gsrzmghal.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagmpucuh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gntmgaeog.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqkradvc.sHtML

[D15] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/godeqgjbz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezxxdcey.sHtML

PHP:  array_unique($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/guurroist.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gyhwrbpae.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gzyhjifxw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkznouarq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaldamts.sHtML

Ruby: arr.uniq
来源：http://blog.fanxiaobao.xyz/Article/details/grtbnvfvi.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpfadyzj.sHtML

[D16] 求和与平均值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghincxfti.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gpjknzwar.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfrmtzhb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gacmupxtr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhhasrqg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fanxiaobao.xyz/Article/details/gjnkdrlbk.sHtML

Go:   // 手写循环累加
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfbesuaq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbkcggad.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoblmcpx.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gjozzkfob.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfyamfbn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghylyffkh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtskfrmp.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmkrjahk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gtgcuhlkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/glombxfjr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fanxiaobao.xyz/Article/details/gddtywrfg.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnyjvpcw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbmogcqz.sHtML


<!-- 参考信息 -->