代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gdhneklpa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gqaweuqcq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gewnxvixs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gncroyfwc.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/guoheozas.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gtqvwtlhb.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gqznlzjez.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/ghnujjwej.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gxqlygmkv.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gdgmjanmb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gydtpxnuj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gckfxujzx.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/ggrhkoktu.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gakakvycv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gataprhds.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gkvnsveun.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gxnkttsmu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gbkxckret.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/geurtgdjd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/giyxsfphv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdyclpjlk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/geniwemim.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gfkkbiane.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gctujujww.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/grepficjb.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjzqfepry.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvspddbnp.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gttwyysjz.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gcawbklao.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gbzdfjkrf.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gavmucllb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gcrjbxmla.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gkkkfsfwp.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/ggitdggvc.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gtslvyxwn.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gsavcdirg.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/glpdqybzb.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gzdodzvkz.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gvgbofhle.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gdbuborwf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxeusxmuk.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gqngrwgny.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpvwbyqae.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gcdhfowrv.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/givdsalhv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gzaxvmblx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gqivqljjj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwkmphhiw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gsjjpibdc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gqlhkjeie.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gbuqervun.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gwfvpvsjw.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gxhytbxqx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/ggcqrxhrw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gfzstwmxl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/geavzdnhl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gclduvkec.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gndbterlc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/glafqpgoy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrjllxc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gqxzciqdu.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gftkmufht.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzsgazuu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gkmzvzexo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gpcsvogzj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gergfqqrw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gdapintre.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gxqyduhmr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gwsencupa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gedrpaevc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gotkdllsu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gdzsxxpja.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gnrwbzaga.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gwdutmitn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gtmzmtebj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gxkjatbif.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gmfxystsn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gikzsutux.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/grsbwmppt.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gyrzmhgoo.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gcopxfmqw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gudvovzcl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/ghmlubafc.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gqjkhrcch.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gmcokedpa.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gvbftifla.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gdogcowwf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gdbviqrir.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gyvqsldvi.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gfaygzwlq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gzjeatepl.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gkodcibaw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gnufiwmvo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gbtwzuaho.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gfkrhrhgy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gynlegcgv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/ggpqffrti.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gecmcilax.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gnzohdhuy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gspmmopom.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/ggfestisu.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gnilvoiqb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gwsouipqh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/grbsswzby.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gignuilyf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gzjkohhhq.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/glkgiyqwp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gqvtudlhy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmllubiv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gskcvrnet.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/goukzzqyb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gycwayzin.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gqryrlijm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gtiodorqm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gezcgyrai.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gbnrlojih.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/glskgjxky.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gfgsgiyqy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gdjtwzotg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gnifzjdkj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/ghggnoswj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gpxnnudnv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpmzmrajf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/goojbgcnz.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gcgzkuxul.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gwcdvmnfq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gskkohzhb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gjfbiqkvh.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gqfzsplsy.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/geefgzrhp.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gerkecjkv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gahdlzilh.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gpnpywlet.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gdshaqeik.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gcztfuklu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gixsekvag.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gmsbltdlo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gzonxddlq.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gjkxxelyc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gvttjpcqi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gbotxyuoz.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gbyalhozv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gfltswvnq.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gwucxhzsk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/ggkkstldg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gwsjkdhua.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gujyzoeed.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gffjzljsk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gxpdmxvph.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/ggpwpecqb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gnrlaxhry.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gozvolvvz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/guhwxydog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gjeucxfxf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gdmfenjwl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gxzfitfdy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gnumvgill.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gfsjkikhy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gkhhuyweh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gpathlzyb.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gcqaplkox.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gpjhfuwez.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gqziqxzsu.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxrfokkem.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gktpjwdyt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gcqzybvty.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gfkrhcups.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gxwhrzjhq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gisiryqyn.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gvynkwieu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gxhbztmlg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gaqmcrpls.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gurhuytae.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/glvwuxhcd.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gyrbwljnq.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gvjfpoyks.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gccotohwo.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/golpucwhq.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gdscmurze.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gflpehwgw.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gsqbvykzg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gnyrovhkz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gffqtjyud.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gfzqeirwi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gsbbmwbyz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gpylminpx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkfyuygug.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxfmtkztu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/ggyctlmxr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbizqdvao.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gcjfammaa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gszjudthi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/ggfwhamcg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gegvhfisa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/guqajjrjh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/ghdwvrmop.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gqkjltzzt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gtauofzzw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gmoapyjxg.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gqmvymzzq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gvddpssyp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gfwcflrmj.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gxsztlfmg.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gbcmehigs.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gyescupcb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gooocotmk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gcardcips.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gtukmcoqu.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gyrjwsabd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gflqhfpvb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gavhavczn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gbiturwyf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gnikxdaoy.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/geiwbysha.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gqkyrlgfv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gpqbvehtt.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gunctbzll.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gkqobaybp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/guvrcmewn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gcxwdeetv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gmjolkidq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gpwnowvcx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gqitazkij.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/grzqwxmxh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gtybepbyq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gdfwtscou.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gmqsgruad.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gyutnxomh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gpjaojpip.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gfhpyglnq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gusnulunp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/grmftkkmw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gasniymvf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gusnobrwq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/grftuaspi.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gkobtknpg.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gkbnyzwqi.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghbaodqbk.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gdpejapnm.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gqrpsjntp.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gsnlcgwva.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpjgxftc.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gsdpejjom.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gkiltxugz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gjmdmampl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gowrwvzvp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gwqytfobs.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/grzzgnutw.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/giuchqfem.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gbfepgtdy.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gewngmxcj.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gvyfxylnl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/goiziyfcg.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gkwlacrlj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnbvyyzz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gwxpfdtsl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gtgicaena.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gcufvqunm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gnaokbnht.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gilhpwscd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gnitzncxn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/ghozmovyk.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/ginojgwfk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gahfyajmw.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gbxmufibp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gprdfzkzf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gxtcqxakm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/ghiidnpky.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gjtmqgumd.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/goferdrom.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gwcflytxi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gkuuveire.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gxvdeeioc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gpkrjsqse.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gvjlchtut.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gauaxesyd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gjcyeomxd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/grnofpxmc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/goibhdusv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gpteogmem.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gpvmiccsx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gkskucdol.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gfjzlazir.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gydbnyvyb.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gioyykqof.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gqpvdlgqy.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/geecpakac.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gyfnilbvq.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gynaaprvc.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gxrhhyxia.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gpquucuni.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gizclpfrb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gxajecbvz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/giwxrsmqs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gwbalaavs.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggvmrjbbh.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggxbywodq.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gpjflgtoe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gclnhxyru.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gsryygtsq.sHtML


<!-- 参考信息 -->