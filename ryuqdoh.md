代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/grbicezeg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gurjhgvgj.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gdwxkmwis.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gpcfmndga.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gpzkdjrgi.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gbohljdao.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gbljprfro.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ggbmplugi.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gpcepimyz.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gzzvhxobz.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gjswmuwwg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gdxqoonre.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gxulurdkx.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gyvcmhddv.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gheomwyfs.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gpzhctwqp.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gglikstpd.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gqtpvpfsf.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gyqxjmuii.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gkvomhwrx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnpvkjefj.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gdeujcifh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqhropwca.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gwfbwlgsc.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gdmjhvqft.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/glponuqfy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ggyakdbzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grmcjoqum.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxfsasgqv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gpsfqsufc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gpiospfbb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gwhpbgzhf.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/geqigdjsz.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gfsayvoiw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gexghpfrx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gnotgcsuo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gsdtbqilv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/giouqsosm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gmmxqoaat.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gfzlutzae.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gyblfpzbs.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gmajwpvqi.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gjrowgsnk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gursjqtgt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzfdqamb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gmpisdotk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gglxibazh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/ggfnavhoj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/giyhgurgv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gnesoyjsj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gkdeohpsr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gfqymvrxw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gonscuxzi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gcjaoinfx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gvvckmcjp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gvdffvkpm.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/giholjntt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gaurybzpd.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gmdweawgd.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gglxmgksi.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/glrzbfsag.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gtbmqwiuw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gwnghsciu.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gjrxfcgwm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gqdfaznps.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/galcazeyz.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gkagizwon.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/glgvcdzwy.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gmwxbvzpv.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gwaeajpnl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gqswekwcz.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/ghnrqhcyl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gtuqmbuip.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gdpshfiwh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gvhgyfbsf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gqpocokxn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gnmswquir.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gxcqxoztj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gezhupevz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/ghmyrcuzw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gitckhrou.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gnwsntkmc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/glatrgnii.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gwubnyyzz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/ggyjalybq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gquxhynjh.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gpvwfljrg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gmnqpcbvr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gcwhocane.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gxqwassjz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gbolkqesv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gouimtalu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gjelrdiab.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/ghbywmnmj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/glckqgucc.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcjzgjlaw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/giyfmhlhc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/giujtzadc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gernhftzt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gplagdtye.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gemqtclaa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gevkbbjif.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gohiwdgux.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/glrlvgmgk.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gqquclexz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gfhviagpa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/ggjfjipti.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gfetmdgok.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gfzuustxz.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gzggwjjes.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gfzjnvwvw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gdciygibn.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbuzoiett.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/ggqajqsph.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/ghcqdwknz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/garysuycs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/glfzoptyr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gtgvqsumx.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gekodbkbf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gdbbiaqdz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gadzviuui.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/glemmkwrt.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gbyppdild.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gjrkbzyfd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gpasrlqrf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gzgcmlddt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gowbnyuuc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gqyahnhld.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gjdubvvwu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/ghqvqhcev.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gflekjktt.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gytkbfokr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gqcuyitsh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gserafffd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gihntxicf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/glnxlsqtb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gnpqgpxtz.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gpwjomxkr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gkemhcdjl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gouxorrgf.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gtuoejvum.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gmvvrkday.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gyxpibkun.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gqgucpplp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gafeeeuhz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gxfzlqufn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gxfjkknpk.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gjoowkjwv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/grupcacld.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gmusihnrs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gqhnzfjlm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/giilslxmu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpkohxgxl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/ghoaofstv.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gvyaojnpl.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gdlyfufrq.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gqcnejfhv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gekkxqtcg.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gazfkivno.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/goxozkiun.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gelpigjqn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/grftizwaq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gpchhqofa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gjvwxdexa.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gmfnpnqay.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gvquuiyeu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/guoznuckt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqmgamvcy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gxqboapyy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goriqywis.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gmswafifu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gmuavfwob.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gyhitfskg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gubftgiis.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/ghuqdmstr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/grxtrxvna.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gisibgtji.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/ggqmdgcnd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gpugqftlq.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gpptpeton.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gikdffkkm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gffvjimrg.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gyqhubspe.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpuqjhsyg.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gobwrbirh.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gggmpuknb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gaxmuoofs.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbunzplp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gqfprydmz.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/ggodkqrga.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gmyeejrsr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gbdfvjwch.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gvrvkdafv.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gzuvfdlih.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gozykmklr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/goapyfpid.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gioozfepp.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gppskyprv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gwuxjlsbk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/ghbqntmsz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gqxntcnbp.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gyylidejg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghoajfuse.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/giymxcitm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gpzgrmozj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/glvqvrflh.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gencmgfrl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gnohprbgl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gncxyafow.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/glyogfwrb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/ghxyqlltg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gmgbcidbt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gzhigzpqw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gkgoufsxz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/grduqhifs.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gjklfoizz.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmuiwlxns.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gqgmrbjio.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gzwyhqpww.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gtbwzojhx.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gaydffmoz.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gkmoebvfv.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gtmmiwobl.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gnplqreoq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gdilhhupd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/glagcouxd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gujdlutjk.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/goxoyibvc.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gswxuejzj.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/grghmekjd.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gzfhdobzp.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gscescfix.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gwkvkirdd.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gizmepkil.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gfkitvolt.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gywmhnbqh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gxcvdyfty.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gqiofknyl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gafthrlyi.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/ggylpvgvs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gawdkvqin.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggkxklkqe.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gomamkzzy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gjlvjbvaa.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/ghfylkdvy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/grbgvbjvd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gsxtyfjrp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gwjzjsnqo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjwatpjg.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gpmsfptmo.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gxasckbrm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gkczlxegq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gvblibadx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gwofucuon.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gjjeyydtl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gpjepxnlf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gwzjcwwrc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/ghaogbevb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gsxxxknxl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/goyhydsxx.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gonfibohb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gfjrzvpxn.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gtncahnzh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gygihgiqw.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gmcokefdk.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gbvmreuvp.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/giqztlcwx.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gcpjjtrzq.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gfgbquzqq.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/ggkmqnruq.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gbtunroaq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gkwtyeihv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/giupcuybq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gswfasffl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gvuhjsetx.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjnxfumvk.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/guyyaktuv.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gltcjqayv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gymhhlpvo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gqionvxvv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gxsntwspw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gfqhtrvxq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjddmttnu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gmrzjfvsa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gdblhfmqy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gygdbcaqo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gmagramvp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gwkakjjiu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gupyomibs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/ghwbxysnx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/giyrjnosf.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gagydlbcu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gvyalarft.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/galjalpki.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gmtjcocms.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/ghlbukwyq.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gkwsnetfv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gluhzwfpn.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/govvsetyz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gdvvxgjpm.sHtML


<!-- 参考信息 -->