代发 wailian999

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gelnfwnfq.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/giurymcio.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gspcqwnby.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gakiwgkgz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gfolfrrcx.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gcpllpqok.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gfdxyscey.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gsgherdbz.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gefovihki.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/ghkmvbxne.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gzvgberbn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/glasqokvy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gtvvhdsno.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gquzuuijr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gdabvgttd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gyflbnszc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gortijnjf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gxhkqpexk.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gjtwscxtd.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gnjrpryid.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gqgdjtpwn.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gnbnhlvrq.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvaczyjfr.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/ggbsgqtox.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gsmppmlzv.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gxmihwhjo.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/ggwyikilz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gqeuptjct.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gkwbyszhv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/glfbeufjg.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gethsyxew.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/giemvdnkh.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/grftrbflf.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gvbkiwvwf.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gughrssok.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gkwuhmban.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjdgytjtd.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gdnbpacdy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvayexmiq.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gvojkdoqt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gzooklqyh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gynqziipd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbwivsfle.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjozdneoy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gtknlkimr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gmdqxlosp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gbpujhngy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gpijssuiy.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gxiznoesb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/ghugazvjz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gwkblaeow.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gamewgyhn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/goqhuflwr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gcrausaeb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/glegyshij.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/ghmjiyckd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gjcqwevff.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gxizmxfli.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/guhmofbal.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gsphvfmkm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/glbriqtaf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/ghaoronsn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gccpcubus.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gcqwormwl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/ggdimxrus.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/giajbwizj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gkkxbywrl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gnidxoghz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gekkttplb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gtyehjeuw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gvethsgmu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/ghvyyihci.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/glevunyob.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gmnbuxomi.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gezqreeio.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gusgutwhk.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gccyfsxnj.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gntjyctvh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/genaslehj.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/goojisngb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gkrsdcwby.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gzqwpfycs.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gszpqrrju.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gccgsanle.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gksarnjsw.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gcasaqxkx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gvujfrpmr.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gkjefwloo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/glkhqqiaz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gyhauwxsa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gryubklny.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gtgotnjwq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gasokzbim.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gagetfjle.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gpmfcspbp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gqztyqlps.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gzgxmlyry.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gcpdklvxx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/geutxqzuw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gdqpvzvcc.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gevqrxauc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/grsnhyvod.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/ghznfitaf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gdpzbnjjc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gapxpuyqm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gjksdbdly.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gmxbremwk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/glarrzbfb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gdhgjprcj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gmgsufyod.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gmtnyxjls.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/glzxeaalb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gziqvdyck.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/guhhqedna.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gzodfaawk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gfkcliaud.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gaszybjjg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gozblnahp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gagjntqdq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/ghtpioxqu.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gsqvvvqfh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gryjushqc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/glebxbreb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gvwyqvgbf.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gkqdfevna.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gqdgvsyae.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gdamxfkow.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/grjerpwty.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gylifpizb.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/ggdddzlng.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gwfnxysxu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/glmgjjsei.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gzquhcdbu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/goxwogjcb.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gfyllxhmy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gqxbjiwaf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/grmqrsyga.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gjifsfsah.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gweazoaxo.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/ghkyyhboq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gymkxcsyq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gumqgqbcl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/glpushrho.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gwjcffrxq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gcehpjzls.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/glgbmhhqf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gcmykedzl.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gmddarkck.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gqbmegzuq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gxedgyacp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/geevjsovy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gljbzswuw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gzhfavplj.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/ghcouxhlb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gugazqota.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gqbpvbyui.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/getontcnw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gmlhgjiht.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/glyekkqqp.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gztliqenf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gmaiqjvxe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gnayuzjcs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gglruclop.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gkqgvfoyj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gtdkhfqgb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gtnfvzhyc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gxoacdnmp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gienrrflg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gcbvvocjx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gcojzorwm.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gompqxici.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gjdpjvjwh.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gwjlbljqr.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gkfeabkus.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gpbhfshfs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gzznhqmtk.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gifksgjgk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/glhgjokvf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gjhftdcin.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gflfsewpq.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gaugwxcqi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gzvcwzgss.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gnjuuqbwb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwhkrcqla.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gbusqlepg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkxqgydjf.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/guscfvxna.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/glqbsrijz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gwtjgkubj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gfufsjuxo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gtslmvkmk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gybzivckb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gmkicehtt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gjikiuyti.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gknnbcllf.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gmkoseuhe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gdoydruvs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gxtntzwaq.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gvtpmukbl.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/grlnqbazg.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gqvjwnmdc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gmqrrxdye.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gkaoieamw.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gaqzzkfwp.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gkazjmiyn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwyxdnlzk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gvombmuyx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/giquckplk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gezvemkiu.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gadiuunkg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gjaouxdqa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gvhcnnbbt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gzttdqcmi.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gyjqmrndp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/grbwkeumt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gyvcwcafe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gfkrlzfmj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gfelnptzu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gxgwnbkzo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gncmamebf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gadqjefwk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gnwyvrjre.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gaajsfdhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gmvkvzlwa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gzabetmtp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gvefsrcvi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gafqqhjyr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gbsihbxxh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gkdxlnmed.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gvlwwpyvp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gkxotzxmh.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gupgulowd.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gvynpuwku.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gbiopxzgf.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gdsqlvemk.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/grcraamtx.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gatzydmzd.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/ghrxxeplw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gxkocafea.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gvwibuwzd.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gjoobgmsh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/goymvkalr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/glutbghmk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gwptrimem.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gvnhlzjqx.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gbwmvtjiz.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gwsvdnwdb.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gntmnvgeo.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gcuyavwue.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gegvhqjgo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gtgwuufqo.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gewcgohvm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gppptlzsm.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gpqcodltr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gxcatvvav.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gkfloubgq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gamewkdur.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/giycqmkiy.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/ggtpqwttx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gdqrokdkp.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gccdnigya.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/ggoimwjrc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gjpfvspjp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/ghuhhkllp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grqjfjzov.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gffzagirg.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gzvepeojg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gszuxjwtc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gvpjijpqx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gaftrbfbh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gqrbnnkxx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/giabgoxyz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gcswlwnrn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gzmjwjxsm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gisaeseye.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gljjymbqi.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/ghjydevnz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gegpwqrzk.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gjjpskksm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/geveptygk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gcgqhamhf.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gmyemuhau.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gjoovkwjf.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gfspttcsr.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/giuvnmjub.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gxocebsjm.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gzggqlltv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtmpcscbn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gyxhdxpbu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gyjcayxkw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gxrwybyzq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/getomucpr.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/ggtnhoxka.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gmczeibjr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gprkhvyeo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/grxccnhyl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gdjsxkrrw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gjlgmajoz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gataidkyk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/ggjddeyrc.sHtML


<!-- 参考信息 -->