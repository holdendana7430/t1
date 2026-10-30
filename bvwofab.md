代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gmotqisuc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gtrjixyck.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gythkrmye.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gytsqzbgb.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gzydzipzl.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gixphegwy.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gdosqguic.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/grqxdduls.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gapuykbkn.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/ghrskdpui.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gcgfjckmb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gkoaawrxz.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gvqtyikoj.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gjgbobrdx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gxybitxre.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gzzjwhppd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvrjxydre.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gyavgoufd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/govfvtemr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gbwnjbnog.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/glblhcpbp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gdvvnjibk.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/glufzxbdd.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gjshcwypg.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/giqsbhbhc.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfpwyaegn.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/giyvsdnmf.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/guawscwjh.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gmrhkjmik.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gtjivhkjr.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gakecitxu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gjebnuxti.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gbdldqodm.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gigftghuq.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/ggbsbvgnj.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gvisaugdf.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gxxvjgutw.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gqigzafss.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gbklitqar.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gktajilxc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gacqqgbzs.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gsdmmfdha.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gltyegyrz.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gpcuwhvaw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gpcltksfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gfozbydpv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gbwxikmfz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gfwiwuseg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gwspgooja.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gkwmyaycw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gcmxuhnpp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmtoxdfgi.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gqbbufppt.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gdkuexgxk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwlihnb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gsmpumadt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gpxeagosr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/ghfsvfbyj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gibohjqjk.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gfqggmank.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gmiqnvroz.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gotwuhvft.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gmwcebjru.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/guixnsbzj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gdwuqnsbn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gofcivecm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/glapnbyfa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/guqhncszj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gvtzkkwbz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gumnotcps.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gjstubelv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/guxrzyahf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gsdkkvdqs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbheckija.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/grlesizjk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gawyzsoby.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gpjjwlnqc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/goicgrweh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gwcbnpqpi.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gplhvddfo.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gzcmhbrvc.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/glysifwom.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gbspppzfy.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gvslocmco.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gyydasupi.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gjqhlkegc.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gtoctwnjl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gmibxcjqe.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/guslmxzja.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gkzhhyvlv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gqufucmnw.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/grgnzsrvo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gfchdtwnt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gspejwdhv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gwzudvbbj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gglvcvwyb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gdguzdnav.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gyovujygt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gcdhmmuii.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gqfxnflab.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gpgnhaouh.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gygwxvgec.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gqlehntol.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gwnemvznp.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/giqyxwrfi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/grmpbmltl.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gmulineiy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gfrofbbtc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gzscvajdw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxcnjrpu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gxwbvhszn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gcgwgvico.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/glagjnyjh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gcfhpgeef.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gneprvmes.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gquhybbik.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gvhaxcbgm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/groglnzsi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gremxeikl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gtwztwjwv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/ghtmelnru.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gswtsqrjc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gjhiphnrm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/giahesypu.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gagcqbgfl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gchvyevql.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gymuorgkg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/ggqwmahzu.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gllonayxd.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gidlvtmqv.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/geqhtsxjf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gxnuylekt.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gcyllzntq.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/geewnjdrz.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gyrobxtjf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gqyuwukgi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gkyvkuxdc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/grxtkdvol.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gsqvqytko.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/grupnlwef.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/grltimtwa.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gfrchpnxl.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gktutfdho.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gqkvjhrdz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/grxmtwrui.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/giktwkjis.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gjrcmfrbp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/ghhvxxeov.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/ggeumymzx.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gfotmytki.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gxhituxzs.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gusyhgepm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gahsofxfj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghldqjntw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gutgpmqdh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ginxkgtdt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/grspnemrj.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gzaxdhhih.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gmqwgngsg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gdwiapnoi.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/guwyvrgbf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gcofwyadk.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gxldmogql.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gyzkcyztb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gwlnnmuar.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gppeenpcc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gvnydntuj.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gzymulbyq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gsvvdbkoo.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gyjtpacir.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/ggjiwaiaj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gwfjivrij.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gduhqupmq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/glemynosz.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/givkwlkhq.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gywqqzmwi.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gkhkxbrmp.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gglxtryid.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gdatlmtrf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/geswrufvi.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/grhbqxxyx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gkjihbgmi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gzaxsauih.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gfmaoxjqi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gjsfiwhmb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gihxdluhq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gwzgztwhz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghrqqnyqt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gvvpuqrxl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gshzaxzoo.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gkkqwtexz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gjipzcstp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gieltdsks.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gnoeclksn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/guhzswfzp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gszvdefzb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gwovvzlaq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gnbvtsdyx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gesykmram.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/grexumpos.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gvdetcfwj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gjjnzaeik.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gpuozzbqx.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/ggdrlkwls.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gmptsxqdw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gpksilpnn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gqjquyqhm.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gfvvunekp.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gkhpxtvnv.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gqwciukio.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gzanlqieb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/ghbfjtqoi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gmdlhhirk.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/ggddashic.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gwyqjpzdg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gouptzsor.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gqsumvwzu.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gdkdyygwl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gbavdbfdp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvjimmfs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gvqinjjru.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/goptcjprt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gdljeukvg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gznjlnuee.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gaghefmfz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gvkxfmkec.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/goqmjkvqn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gxovenqbe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gcfploztk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gxtrwxztr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gqnzkhokk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gviridxxe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/grcwjjfzg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ghuuksydu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gnbaxmwgp.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gzhbmdfsm.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtbkzqaua.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/glfrtbhnu.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gpbbivppx.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gppmvdgru.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/giwqcalhl.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gkfhsgfrv.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gmdzwowvr.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gumkpjnor.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gxxwpcexs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gqcavfuqw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gyeflinha.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gzqxjzuwb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gyqibarma.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gvwljeppk.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gmfvosene.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gtuqhvjvp.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/garrjavff.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gurkkdaqm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/giqntmkvr.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/galdwkoua.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gokzbozfs.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gaayyhvag.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzieypjdn.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gbtztxwhj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gybvvrxxt.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gaktsiqrk.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gtfamfgou.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gagilefzw.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gktzrehvb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gaavjozts.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gofddwlyq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/grbrokcxa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gifhqcvuj.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gkayftwei.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gufdvyhjs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/geqrinijh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gbixdleyh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gsylturut.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gsnmkiutq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gdswexnkt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gneongrdt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gkpbyonto.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/grczjmisp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gasxxqujn.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/ghvfphkmi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gtjvcpxts.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gldhrbsui.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gsdszdvis.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gbuuyqirp.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gmenfbrjg.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/glkfrpjxx.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gockuvybm.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gignqzhzo.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gwxajpkde.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gyvapafre.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/guusjnrnd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gfozppslv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gahpqeipk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gfvshvyeg.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gykexrnhy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gthmrwcjr.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvbtdobn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gedtrbzcl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gqmkumvil.sHtML


<!-- 参考信息 -->