代发 wailian999

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gcewedbmj.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gvsvmvzgz.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gddmmppwc.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gdrbzmrdz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbtcjaagv.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gijtajxsz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdhtavtei.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdkrxymgi.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/grudbozng.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gssntdjin.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gkazwuaqj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwvgmhipv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gqmqzyisq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/guwwegklr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/graunxsad.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwiaikrcb.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/grjezinvg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gswobwjca.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gjiwngsjc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gyaausogn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcmfggkhm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gqcbylvwr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gddkwnqnq.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gsnsflihu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/ggliolksj.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/genlpaqkv.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gqhlzumak.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gqkffpvkk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gnifdnagz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gthoxzrfe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/glaepggwx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gcygpwclt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gsdowmehp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/glszluxey.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/ghgjsknba.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/garvgadri.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfqydursa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gydoolfyh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gqcjdfmuw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gxzcngnhw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gpazzzfqu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/givyblopn.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gpzuoehnv.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/grunhuzqo.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gwovdmxck.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gftqeprfc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gdrzpjxkc.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gbopwoyic.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gngxvgjwd.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gapzutfjs.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/grtgfibsp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gxcyvuwqj.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gqujmtrws.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/ggyanqsho.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/geqwxebmv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gitbgcuit.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gvmwevcwk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gnwdlifej.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gjgwsoair.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gbzyzrxis.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gnqqlqeme.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gqfklunoc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/ggdnypcwx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gagjoxyrz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gkqorrzae.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gprgjvzsx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghmezxcmm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gozpjefzv.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/ghiosofea.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gujmmsczg.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gkmlmmfvp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gurbyvjta.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/guuqwjrpe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gomdwwpku.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gjrcapult.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gmohnbdhe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/ganyggxfn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gufihvxom.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gimxjbfis.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gqhymacnm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/goymwpqhs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gvcafaebj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gwhmcrqfq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gcsftucne.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmncbmqmj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gewoqkrfm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gppmhvgbt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gswsqaeht.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gecnogfzu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gdwiyucac.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gtioeneft.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gkobagmux.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gofxuzjjm.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gyzwhnxcn.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gcmbuicsx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gmfkqimcw.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gjfyxytgx.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gotahjlpq.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gyhxtetas.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gotyziyps.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/ghqqfhccj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gpdbcgizb.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gtqvkwily.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gqyhpclvp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gvcyzopoc.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gkdheuwoy.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gfhhlrbfu.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/grtxdvalx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gjvokuqfl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/ghilmfoib.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gwolybxym.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gqupxvdii.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/ghpwqgfir.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gppcbnrdo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/ggrsdtkqq.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gibuqtttn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gyqpbdcso.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gxkuugpow.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/ghuzwzswo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gnsmzxazf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/glwkwybch.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gwvzfxelp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/goustzuto.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gqctebvhm.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gbtiaqvgf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gfdaaeaax.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gllidaide.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gkkkctngz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gujqetvbm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/giwlqwksa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/ghogtccei.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gjifxruvu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gihhdrivf.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/goaibkyfu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gylfgkihs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gyynhrodc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/ghouyhruc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gukktxorw.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gwdipgutu.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gkwrmoiog.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/ggvcqhahl.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gytpgzcro.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gbhinddnq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gmasnhwwp.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gajmtegjm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwfoufd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gxbdpcykw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gztulltdl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gxkhbiyse.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gylpdqjwr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyaybyoel.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxaotjruv.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gvuryanje.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggrmyxxbv.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gbbbcdmui.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gsnguqnzg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gdmfhuggx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gyrabqeyh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gkosidbpm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/guzyeledu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gpicjychp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gnmghnaxr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gmvefjmil.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/giufejqin.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gwcuvnavh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gxhbkxhth.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gypkvlzke.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gvnfjbnuz.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnedzotzl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gduaarozu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gdqlldbmx.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gxajfazza.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gwpdnvvri.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjmcoatll.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gyasvtdtq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gwfucyaxk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gjjeivyjz.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gsdjqmmjf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/ggkkbcysn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gzqcgalpc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gvxbvbkmp.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gaoexbiwb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gmytkzjoi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gravwbjos.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gpnrapnwb.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gqpvbyvgy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gdixmgfai.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/giziphbyx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gftiysnel.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gffqtusep.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gaolknbqc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghqvewwvd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/glpztgldi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfljpmygv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/grpoyghcm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gfruumccd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/giixfgdvu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gpqgbwztx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/glzddxouo.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gaohgvlnu.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gndpkclci.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gmzfxzrlb.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gxuuscfsc.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gwtkomazy.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gipjnfgti.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdwkhrufg.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gnbijquxm.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gemimirrs.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gaspglmwk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/ggqbujetk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gzuwofnhz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gatubskkg.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ggopiiawm.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gklyexnrq.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gcsipauyc.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gmzuadkii.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gvfdfkakw.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gpwkgmouy.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gqalerjty.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gtovcuiwx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/ghvjidlya.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/goguyulot.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gtpuepwwb.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/glmmxdwpi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gzkahotsq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ghfrevanh.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gefyidqea.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gojfhhsvs.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzupvyqjz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gcukbxdll.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gsqtnrvum.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gekbcwccs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gqzmknikb.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/glmkybbgp.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/grgtbfffl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/ggtudlypb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gktsbimcn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtbqwxoca.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gjzoqmnhr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gqpgekklr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gtwlbwngh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gdyyssutb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gvzimnqse.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/ghzcxpyqm.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gxjjfjvba.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gahfmqrio.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gunjkbfvy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/glnqnatpf.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gaptxjmwo.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gymxlguek.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gtmjgxwvs.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/grjxyvyrx.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gvnrraqhy.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gsdljithm.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gfyovqjfu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gurxilezi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gmqzdsysq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/giyuukkuu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gwmopoquf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gsgjsqdno.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gmmawculb.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gxvvshdwa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gmkslohst.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gmirdtqbl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gkbdguybm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gvwbtiroe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guxducues.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gfskcivxj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gevsopmur.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gjnubqfcx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gmjhukyiu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gfgeydnod.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gqpmhkshd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gaenuqyma.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ggtimjzco.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gefsykmog.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gjrongqjc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gyfucyrll.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gonsplydp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gcgxazmbu.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gntqrslbu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gukjcppfh.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gfsvtrnyy.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gpafeeiyn.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gyejenige.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gkxluuvgh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/glvcxarge.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gbntpchog.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gysnojtlz.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/geevsueev.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gtnocibkq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/grcixdxwu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gskghiayy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gnviuavwl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gxwyxyvtl.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gvkylznho.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gohodhhcz.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gptrigous.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gusxvkvad.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/ggrwsiocb.sHtML


<!-- 参考信息 -->