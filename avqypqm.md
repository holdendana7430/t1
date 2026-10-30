代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gpygvhqjo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdokpao.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gscjwcjgq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gbgsvechv.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gjqcnered.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gfymfoqbj.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gfrrqsqyo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/ggbfvwknl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/girkokfni.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gmlskmlpy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gaydvlmun.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gzgtsrqgq.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gwnxbdiuz.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gmwkabunp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gxouyyccd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/grrttvlve.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gvtziglrg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gnrvkbjao.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/guzevvvzy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpcsbipkh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gckadgsvh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gwdhycdnj.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gnwzillya.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/govmvshoq.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/ggqergmkl.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gnhuwathf.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdbzorvtt.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdjlwrnkd.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gfpgmwzwf.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gpgnhqdkb.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gnotaewpd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gmeyqfpfh.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gpunfachp.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gcrfykfpy.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/grzsefirq.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gzmwcyhqm.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gtxzaqkfr.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gjpuvmelq.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gekatkpsk.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gniopiosx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grmxlpmea.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghnhjhvmk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geinnfqdu.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gcmvnddna.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gzatzyswt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gjqbyvjig.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gxszorasx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gbtzjkyiy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxjshyhgp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gjazxceyz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/guwsizfxa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gjbqmiszb.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gfsrbycpp.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gjzsscjne.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gopapjvtc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/giuvysfej.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gdetddifa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gegunqypg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gbhbqeycc.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gabkcgdip.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gclnnupin.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/guzzumsyd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gjuusnyyd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gxaqwxdkf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gyijlrnls.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gcuuedabb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gzhofctmc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gqxsvwsyp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gogtxnxoi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gdaydgwaw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gsknldymo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gqknicwtp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gljhekbrd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gqlboxork.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gtnhlnjxj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/geicjvfey.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gmbyjscba.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gghffwtsh.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gavwsyfov.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/guwrcygcn.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/govyrxspk.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gaujujmmc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gohjipfjm.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gjoddmasi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gxvjtqlcq.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/godhthnoy.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gvelorbfs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gzzapdnvj.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gnpdfysvf.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gwajvdynk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/goerzvrtp.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/glbrilsab.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gtgspyhdh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/grhajzbac.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/glgxtblrz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gmcglgmfi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/glsguknmz.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gxgtthqnv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gwlfgyvab.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/grncugnjx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/ghhncirxj.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gaimnknih.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gaghzchyy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gprwudrxc.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gamnfkohx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gqxvnpemj.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gahfkwfva.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/ggshuflyn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gwlrqznjq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gmselmuxl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gxyzrzzoh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gyuagceti.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gbzsylcrr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gmubttsor.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gumoagazm.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/geqexchzg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gnqprnmks.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gkiibkpbt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gafnzycpd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/ghnycmlwv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gezjgeltx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmrqfuffy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gsgjrswqx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gwltzjuci.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/glquxzugp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gafxfbryj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/ggktppijn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gefsuxnqo.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gnphqkzxc.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gazxvltqa.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gnuzwykyp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gomptpgpw.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gaoerxwso.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gjfsicnbx.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/goctpyfft.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/guxqztylb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gbyrlsryf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/ghloeekfh.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gfhfmncyz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gbewxblzv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gcrkfuuuu.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gawcpieji.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gepqqwopd.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/guigulxqi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gnnbclcxs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gbeyjxewb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gvqyjmthq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gkedyotww.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gygeqwyna.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gtysxrftd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gedbzqlqv.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gpjnjiuty.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/glhvmzuep.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gveuuhxxl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/grntfmkns.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gqghxanvu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gwquhenwz.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gfsnsgnmq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gmdhxnvis.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gegsatmsz.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gioncwbpp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/ggpqeimfv.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/grjqzwxlp.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gebzdeuan.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gvftiepxd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gxbphzbrs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gvlevqjte.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gojjdiazg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/ggfczedco.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gqayhjoww.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gotjtvzjn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gbwtmdwkx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/ggsinlosb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmtxykyod.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gbzkdofei.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gqohxhqze.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gymaxibzi.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/grnzbtkbc.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gahqepdha.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gbjgxcndb.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/ghvaflzbh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gyinrawrl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gaxntapkh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gbiynourn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gavgbiqyq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gvwlnrejv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gojdqxnli.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqhvbtpma.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gsizezhlk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbzodzcpm.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/guginorke.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gjzdbqbpc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gshvbgmpq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gsktcwfab.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gndswmkyd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/geaiqernk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gvjikkapw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gcjkolaom.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gcxbokbkd.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gdqxcrwgm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gjkabxwkh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gipjjytar.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gxddsogtw.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/goltqebwo.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gtvptujuc.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gfdhgacuj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gifahyecd.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gcpwkypfi.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gnmnozufq.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gpquffmya.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gtffjceyf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gqttjcpqo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gzudxsugp.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gtwcxwchd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gosetksrd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gqtzfauus.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gcxpblijo.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/glmqmrtju.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gzcwxgcsp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gxehaxkrd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/ggxluxplu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gozaztjtv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gvcnccvyz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gqceoevvs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gwypbucnj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gtpemmxyp.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gutkkqlat.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gwukiucib.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/grraztkpm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gwdzvamsv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/goghsjtiu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gozrixncu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gdawwmpuz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gcgtwsdcf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gkcugngog.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gdktdeplm.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gybdzzjqm.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gagexmedj.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gkgtoubfr.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gkzlbadus.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/ghtpifeqd.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/giqpdsuty.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gntcurwfd.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gdelyykqy.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gtflkqjkh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gldqymdai.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gfxcfgwsx.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/grkewttat.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gvnttzqjd.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gdexqqtfc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gjixftomj.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gttjhgocs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gisaoxibx.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/giktkcjky.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gnkjaioez.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gnesvdxau.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gzmnjyuly.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gyuuxawbu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/grdhdkzhd.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gghftrptt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gwxusnokt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gmcgazovd.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gukjpupvy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/grrssixyy.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gnqnhbcsd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/glqobmzyv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gnlbnfasu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gjommgrql.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gtflsjmia.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gnqzbyqkq.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gbwnoosoi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gpkedellh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gowwzzbbx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gbqtghlmh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/giuvceahj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gfrapqsal.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gnkhhaksp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gqsfjvunp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gtkkdxcnl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gwgsmmsnv.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/goawmiwgi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gqfrnssua.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gfxaylwjj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/grjxtkwsd.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gjbhnexkp.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gcqsdadcy.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gaymvqggw.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gitknimoa.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gdbtwbhnd.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gpecklgfm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gfpnlcrxz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpbyxsqfh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gjyvreefy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gsgumxeze.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gpwpgniqk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gaqhoeeez.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gtlmvnzax.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/guxpvyvlh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/guecqutbb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gmsqzsksy.sHtML


<!-- 参考信息 -->