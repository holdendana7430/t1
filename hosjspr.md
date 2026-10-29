代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/geggnwvcr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gwqaoitkk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gspeeghbc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gvxvkiugn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gdbjawuhh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gkzozkzlm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gawurpvye.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/ganvgephy.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gqehlhkfi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gppeypybc.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gtuiwpemg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gpmqjemgf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gkyqgszxv.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/grqnuohoq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gvfpifeny.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gawlhslsf.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gqzoqjmwk.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gdwuquool.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gsrcptzsk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gkbjrxdax.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gpapzchnl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gowbqgsnm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gcessyfbg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/ghxylwnds.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gjnfqlthp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gclzvqkvv.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gqxuatetg.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gigsomtpd.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/ghjvflajv.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gabstsfkq.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gcjkcgved.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gnmjciexa.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gxtlyuwur.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gqdyzdtwo.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpucfuegr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gopjryvsx.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/ghjpdspay.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gzoxbvxae.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gjedgaqrq.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gztyauuvj.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gxnsulyep.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/glwuuiydq.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gxcvcdsgo.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/grwlrklpq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grqzijrfx.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gbvznqkyf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggjmsxcnk.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gxpgpvzae.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gvcthvlme.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvztyrqdk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gxlqquuww.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ghevmunzp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/glryibcop.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gbvundbmt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gwoeklvpt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gawcjitch.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gdbxbigew.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gklfokzbw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gbhxridjf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gexjlbsth.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gpscsxhcf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gosynknnd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gflljqhov.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gvumughyp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gwbuekrya.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gkfzjzozd.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gaktpetqa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gnezeibqc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gbqyrltiu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gwjyqjbhj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gqdfmdvoq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gneqqfchd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gtebjsflx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gkignzekc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gftubtxtj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/grschxhvu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gzaaayjmc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gubsomehe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gyzsftmey.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gbgworhne.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gysbnskot.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gurpiflqx.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gdocupknm.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gvzvgxoea.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/grfgnblhr.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gdmdltjvy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gfiitebeu.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/ginzdrvkl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gsxedtctu.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/grijkrxim.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gtdumxzev.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/glvxxqtjo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gzwhofkla.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gcxvzieyb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gbusnswny.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gaxfoovgk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gwaopkgks.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gwtdysvbh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gpafgkzpq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gmgncanxu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gdmogudzm.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/ghsfhgrga.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gmkjliukd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gymuywlgv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gfxriuats.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gerhbnhag.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gcneabycd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gmknlrmnm.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gfpheicyk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/grllanovm.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gbflkaoet.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gbqejhcyv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gqwybhspw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gyduzypbc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/genwvclvy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/ghdxpyecp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gnmgpidqf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsznmfxoo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gpntxlyvd.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gdrdrvysf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtdlozdjn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdcawjmm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gntczisbz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/guonideqe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gxuzfvslr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gkylvlwsq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpwplsjko.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/ghbsnhoek.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gtgqjcejw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gacyvyqpj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gvxmtwgnr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gnbvixbwl.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gvqjwekcu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gjmwkxopj.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gzdsqihrw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/geyysppra.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gjfnefdvg.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gjxgzrjfy.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gxfssameh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gsvcvqcww.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gqaloivpy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/giuqmuofk.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gbfgdtvtx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gfewcrsej.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/geibyxkpq.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gjotfpbpp.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gpnlrafnk.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gljzilyjo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gnzuqbqrj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gqwzraahk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gtgdbhzzx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gfmvckged.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gzxrmgkgs.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gxepiobqd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gcrfiseas.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/goccdiybi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gguaxgjux.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gmsybwkgs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gakytdtoq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gvsombgdk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gxhoywbjp.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/geohjalql.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gimrhldca.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gggbtzhda.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/grrbsmilm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gqrjrruce.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/grrcfabzw.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gczpzqtec.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/glegkiqkg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gzyuloohv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/glagegxnr.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gbbgiblwr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/ghvtwosby.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gwwsancfx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/ggzwpriiw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gcdhavcwz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbmrstdas.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gcizcwoei.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/guyvxdvhn.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gyvfcbiqa.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/glydtnsio.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/guvrpwvbn.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/guznfuvzq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/ghcvphzip.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gcnaaokcp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gjlxahyqm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/ghthsogni.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/grytdmucp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gflylgkfd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/giikzczcl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gjtlwoojd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guipxtddl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gqbjereea.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyreemqzb.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gclnbfayw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gtrbtlgdd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gcujnjbcg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gmscegtbd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/ghzuoqalz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gbqazbmcd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gqfkgbpkj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/ghrwkbogy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gfejpscbx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gejtrfumq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gqpaxfmxe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gjyhsbwot.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gkqwyawon.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gmearvbdb.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gmigbfsun.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gqjpuehyc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gbnhlvadx.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/glsyjxnpk.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gczcxrtcy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkfiymill.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/grtdflcnw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gqrklhpgr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gwvcgzphi.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gtdnyvotg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gcrorwodw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gqmjunavo.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gapbvcohl.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gnzbmsgzo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gcvcnnkln.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gcuykalti.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gfoqkewzi.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gxozxjngq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/geojskyzr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/grnjpdidy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gfcxmfwrk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gvoxpxiha.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gudpfdxqu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gqtizmfle.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gzjimsgxi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/guowbqtvm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gplawndyu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/glvxqznob.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/giivqnuia.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ggtqwksra.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gelserkdg.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqedxdyyr.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gdxblbfgh.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gydupkjmv.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gzqivukjb.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ganyppnmd.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gxqbygmkm.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghfiulexh.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/goilzpsli.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/grfkcoarh.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/geicjbmhj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gpegcrxtj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gpwiegjyh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gpysnkokf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/guocuszqx.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gdmjvfewa.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gbkctyshp.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gymhwsixy.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/glcjyzlop.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gcpkyvwzk.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/ginwubezc.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/glayaqluw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gcalxhycc.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gwjvgbgeg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gdxpgjjiy.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/guybxxmsd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gkutvthmb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gfldknesn.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gwrkzlbxr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gxcoafztu.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gqhhirsua.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gdwqbfcal.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gbrczdizk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gpidwuzcq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkgyldmqo.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gmajapbuo.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/ggtgiuwgy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gxthwuvix.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gbqexpres.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ghrrzsnxx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/ghbnrjseu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gwjmzkjkw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gzinklqyz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gfegjrlkt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gsmfnfcou.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/grpqyammo.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gmpqjywkf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gxcirywuy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggeoxoahs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gzrxblavw.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gpujfiukk.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gjwjmuoww.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gvckelmwv.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gehwnabvs.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gqnyzpuzf.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gihiuupyu.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/grnsxmvjn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/ghdbxybwj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gwcnhbyje.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gdlgdufyk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/ggnpbktcv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/geackmigo.sHtML


<!-- 参考信息 -->