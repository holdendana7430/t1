代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gmsrpjrkk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gnlfplxpa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gaclpsdpp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gstkkremc.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gxytgmokv.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gkkgbfssa.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gfxxbwdak.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gnbjdqcba.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gzmsjpjbd.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gytwliixm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gnjgdwbzx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gpyawtotq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gzzhnbaab.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/ggsgodajs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gdhfzzcuz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gpnuwuxkw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gdworxdnl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/ggmjnnwhj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gnmxwldsf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gkxzryzkh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gmcljlffs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gkifgvsyo.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gxtckkoif.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gjmqrcbog.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gudqhhmrl.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/glrwgtgsn.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gcmtpkqeo.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxgbsgdcp.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/govynmbrm.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gagmzpycw.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gdolejbzp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/ggxfazvob.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/geqgmxodr.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gyerswwtx.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/glzdsdaqr.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gbybsemro.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gzshifjwz.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gfcrqykmu.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/ggkhnfpqw.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gihhbvyza.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grwzkxzfn.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gcgevropa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbklnugsh.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gzgfwzuie.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gfvonyydq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gejtxnzic.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gbjuzbzmj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gwvcomnhk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gpumwqpxe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gbmrjqymq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcnzcwdge.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gnssbjkps.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gkwiahvwl.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gmjhuexmx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gpjqrkojz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gxmgclzwa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/grtlsyvtd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gkiqxouqx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gangnjsfh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gdcsqdxqk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gkycjckxe.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gkiysuldk.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gynnyyrcl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gquixyvkc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gowodpeqi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gwhxlhtdo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gczvgtysf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvfvisvy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gsbybhrob.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gapqncuuv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/guxlzwwgq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/groqblocg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gjhmvvuak.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gxgrpovbj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/goikrzyxo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gbdhqydqs.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gxixttsqj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gfytswvya.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ghhpjloaa.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/ghpfjjajg.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gkuungghe.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gofcbjber.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gwzlyjptb.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gasmcezvv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gjxvfmbqs.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gnppcbvyr.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/ghiezhkzn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gpqowhafq.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gsfkzktap.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gheyajzpq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gictdiaor.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/geiqlxgjj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/guxernedp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/ggvexewmo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gtjzgeoba.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gwevryrju.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ggjgikhmm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gjuwwndpi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gtyavwtih.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gmxuwudtp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gzvizxvbl.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/grfmyrdee.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gqyfyuosy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gwcatfzky.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gxfojaxuj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gmdkkoxyp.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gifhgxwaw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/goqrjuhrn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/glilctfuu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gakcetwqa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/guqgsjixl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gvegdnvec.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gwdtlggze.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gdtzntjni.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gueehgksu.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/ghkcnhjxu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gymlfhowl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/ggrotsmje.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gpulpddzk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gcwndyber.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gmoourkdm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gjyjljrbl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gadeebtwl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gpqeuteck.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/glavcqtnc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gxshftgpc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gipkcfyoc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/grrziflpe.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwaxbkuta.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gdboicity.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gsfmnvbfc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gteauhziv.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gbvwvckbh.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gzzrvlrjb.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gleavdcnr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gwsdzenot.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gnrvuoeqc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gaejrpjfa.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/grtamnhyu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gtrjuuadd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gddcqsuxj.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/ggzqcijtj.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gqcygajnv.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gkhovjfjd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gfblwwpac.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/geuhhjynm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gqkzqylwj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gdgahxybn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gxbejnpsy.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gionfqrhh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gjatwfqie.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gfwpinrjs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/ggzyenttj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxoimopmz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gcvdffalf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjleqmhfw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gcbwnvdmt.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/givmtkzum.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gosyxrobb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gqnoynpop.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gvsopnqwo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gqotmujvt.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/giluvcjxo.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gvfqrfqap.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/ghqylsnky.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gwapiwsps.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/goxnavvuj.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gmhlxveda.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gymjaelnb.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gjkyimlgm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gzcfmpait.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gbtyoaxze.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gqoogeykn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gtxmvqctn.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gcezwbero.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gmgesbyzq.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/geokuoguh.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gaqnmxpfs.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gbuwngobp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gwnbmepnm.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gyohfflyr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gvzdjjujt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gfwurpczo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gazkhczcg.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gthddnasj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gwtnphqud.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gpmoqwody.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmirgtzym.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gqnimmxrq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggkmtgcvr.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gtxqtzszf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gqvqxgbtl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gqkzvsmjt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gwfqlzlys.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/glnmtfudl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gpibyowdi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/giylqptox.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/guttcohyu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/ghhmahifv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gwfboypyy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gqzlpszuf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gwheirfww.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gnoaeexcv.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gxostutvb.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gmrqknwhb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gaqvxgzlw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gxaoktcru.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gdvlkwklv.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/ghkdiusdb.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gybcueyjp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gxvatebhj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gpuoeglls.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/glmeplfni.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gyeqmsclk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gmtklzqtv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/guxyhftib.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/ggmssbboa.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gjqchhetl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsrtfpqy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/grzmpyivd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gxirylcsg.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gwvqwmlum.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gryqowptv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gtgsatfze.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gyfrdmnya.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gjdcfqvqt.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gkowlteiw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ghusncbli.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gasoqzrts.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gljhaqmwf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/ggedhgffk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gopztjbxn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/guvmajwuq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gywacrsza.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/giumielxc.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ggvmlnwuq.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzfhvfmjr.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gamotyojx.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gxmugkfdn.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gogquskrg.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/guepvrmwr.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gaibpcyzp.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gmrxvbksk.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gijikthwx.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/ggeyqsgtp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gzvyddprl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gybzskkws.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/grnksessj.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gytpjilqh.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/golddaumw.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gcqfwaoqy.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gmkshhlgv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxreitgwt.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gkvukarxq.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gunjyegjj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gzeyhfbsb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gxjgjpcyk.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gjieiplre.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmfuytzxo.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gezqjtyta.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/grlrkaytt.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gmvxrqivf.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gkuexejay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gwkbkfegc.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsqzoxdkn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gigrmqgmz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gnnpsnivn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gehhasjrn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghlvmamgn.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gnxedxzzf.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gojgsasdo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gvwrsrwip.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gwabiwwaw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/goloflaml.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gfbfnqjcf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gltdqrpgl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gozhlanbg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gozzfihdv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gfjtyxdwt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/giywllzws.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gwmgbertf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gptgumiwk.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/ggldlkocr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gsmeuymil.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gheknzvlj.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gcfdddsxr.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gsubcqhhz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gnoaybkfx.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gmfujfsbq.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gmhbxwqxy.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gxsggcjun.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gpodrbgka.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkeqibgim.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gcvbffkoz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gfqrnwfyk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/goodzjqxk.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/guubrhsrt.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gmwdxeiaw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gcpmmrsey.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gyxypmstu.sHtML


<!-- 参考信息 -->