代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gdsaxrsyz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gppoproyi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/ghkzpojhw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gemhojeet.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gepupxphk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gjvnfzsvl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gjcutuchx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/geyikekex.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gcyyvdwns.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gwzpnauva.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gznonhqyo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gkikrbyib.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gwlwniovc.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gciznpbhq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/ghjbrtyhe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvfxukns.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/golrombcj.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/giorshjmy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/ggixnmdez.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/ghhhfzudg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gvmqlmusz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gjsczsjzh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gjtrmpjnf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gdeulllgp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gpafymiga.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gzktjxtuy.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gistsnatd.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gkdiiqmds.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gwgtmlvkg.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gylcsrnkv.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gzmapkgyd.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gjuredjqk.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggrmrtwvr.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gdvzxrpwi.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/giepltdfx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/godcngzsl.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gielouoco.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gjjejogrv.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/guokqmeny.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gmbhylxir.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gjptkwbtm.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/goprvpwvf.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gpmhoyzdx.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gsukenowi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghayhoamf.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/graxcqrcy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzrvunibu.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/grdstzapi.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/guajasbhp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gsqqxorki.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gcwcnhrxf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gsnylgala.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gpzlojwxp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gsfypmsfg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/glastnxwm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gvrgkdmgn.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/guuvwwkxb.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gimkgpxie.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gvldjkrmr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gpooqxihu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gzbpmjwax.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gycffznlu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/giivddmio.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gjrtmhanc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gihrpvgyy.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gpdyfefhs.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gadqechwb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gtkejxqkm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gesqliekh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gbnrafiik.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gttvdqtln.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gnlmdgrgs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gmjqpchxk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gnuxqstvy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gyxcgvhcy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gonxzzgxk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhlocga.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gijamadoy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gzawhgbnk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/grsxsypfm.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gylhdshxa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gmevrjxfr.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/ghwcwmsti.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gpitnvpfi.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/glrluniyg.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gfouncfla.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gpchcczeb.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gzrpizpcl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gbxwhfrhc.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gceqjrlqi.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gtxuspctf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gjfmxlkdn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gbwbdfbst.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gelxvrmyv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/ggnewbvxy.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gykreeglp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gtkzjbvfz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzqzdyn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gxpcbpuuh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/glzdmfcnk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gqkmstpet.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gqtyihnji.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gfdkgndea.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gkkmifxnp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/ggiriuqim.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gcmwpwein.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gknfjzhuy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/glrleyrng.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gpstnbfly.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/griowtmnk.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gpwkagude.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gkxjiwcaa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/guwqsdxks.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gnfybqoaa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gxyttfqzy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gjhflrkej.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gzfkqcedf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gnynjwlbp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/goshopuoe.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gbibhodfr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gaiwfcbiz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gcuftjwod.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gbajfiuiy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gcvsnvdts.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gsnbvxgqn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/ggaxhoiiv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gewpqhclb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gjqkshqdw.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gcgewwafx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gjkyffvkn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gjipxqebe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gejpvducq.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gketieaml.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gxaopacwc.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gnatjxjwh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/ghmbenlav.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gotapcaog.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gglvkjkgz.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gjvsrhjdp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/giyuyxzky.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gqhkrpjym.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/guobzwohj.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gbyjaxpcv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gcsebkfrw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gefmvpxno.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gkucdlpik.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gvzgipuqj.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gknpydxnq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gsvdfgpsp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gqnwmghus.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/glidgwywg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gjbytnyzg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gshzfkmni.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gysqpitim.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gleumczvl.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gkaqtstrk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gvveggbez.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/guarmvpdg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gsnzwgqik.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gvukxduyy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/germjctgq.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gberilvyk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/ggamhibgf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gbimwxyso.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gjipimtqy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gybdnuoom.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/goaatjmcp.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gmusmzdop.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gejmaloyl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gavhryaum.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gzhxzgwni.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gofkkgmpk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gqkkxbhoo.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gipcdgoly.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gisrfitoy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gkfdhzcuq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gytqzsrkc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gekxujmkr.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gewgiwfde.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gbazdukjz.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gqqgpechi.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gukumepwv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gmevanbct.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gogomvdpf.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gxnesyayf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gveorqddn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gkuqrjfwn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gqurxzocy.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gcqakyjdj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/grwvyrhse.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/giekkfclj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfaqejliy.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gkepmnpuz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghmfhlagr.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gwnjbqqfr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gpyvumfjl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gpmbulppo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/grrlidrdl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/ghkvinzxp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gzknkfnij.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gbmgcvzvq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gavyrbzdk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gsvcauefa.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gocpqvkob.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gpkzhsqja.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gwczravno.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gvuzrnaek.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gevwcxajx.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gdbwjxgqa.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gaznqqjcq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/geczpmlma.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gffvtjjkf.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gagwvhyhq.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/glkpxnamk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gssjdmiot.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gackolwur.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gdxfbyctu.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gpltvdgtd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gkbxqljja.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gocyznyji.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/ghhfvaafz.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gktfynzrg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gjsebqkgu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gabytodqq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/glbabayqe.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/grgedcoqh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gctwgrldi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gzaizzsil.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gasloyekt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gsnkvtnsv.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gemdpegly.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ggjdjnjqp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gepbgvtzk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ghxmpbmxh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gofjezish.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gzbeuiofp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/glyiujfmn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gqdccgavo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gbdpotocu.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/ggfqcewrx.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtbemvddu.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gxqucsuvl.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gjepfopqn.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gjcbpzwoe.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gtnozrjwj.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmuzejo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gycnzqcso.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gsixaclkm.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqireduja.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gtovudfwi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gfmrcdvub.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gsgyvbosj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gwlganbzb.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gqijgrfyh.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/googwtmht.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/goafgwxpg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gyhphnucm.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gseqnsoev.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/goaedtzwq.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gaavghwwt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/ggdmloakf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gvlkwxeaq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gjjbphzgm.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/ggudxncrt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gfvmexvwy.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gsyfpkkyj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gcxtbowik.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/glitnkzso.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvnssnrne.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gkmhinvkq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/guwdwqzlm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gesiqtqex.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/grerrgxvz.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gjnrqimrm.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gnneyooog.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/giwlkfnby.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gmikqicnv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gnajxrxsu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gngffeppx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gjvbirmqd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gtjncngsm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/ggtwnszvl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gfzvahklv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gojtcytvg.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gczkcddsl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gwctizwpi.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gguohdpeu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gppsdtulo.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gveqbcwxf.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gphrxzcxp.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gfopunidx.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gsqoodbyf.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gegqjxbzj.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gfziuctfh.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gycfbvlkj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/girgvlwpp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/ghzchcjtp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gnypilesn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gxppawndb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gehdfcoja.sHtML


<!-- 参考信息 -->