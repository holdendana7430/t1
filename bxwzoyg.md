代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gxjjulohp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gkwatlhcc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gakncbkcj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gwlrrnryr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gwmexomuy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gpidqgzhp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gikulsdbc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gcrxfkvas.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gfdlmdszo.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/guldwfvfb.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gvpfwbzjp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbyphvqbi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gfcttnpxq.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gtcehwsbf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gfyjrbqjc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gyqasxorq.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gyqqgbpjc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gnktearca.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlfpmtq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gtqyncbti.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gxjfovvac.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/guvwexuvk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gyeowgqzr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grkzgzarm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/glztjcjnl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnhhsiqiz.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gxugljdpp.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gnqiyrqwe.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gbedkkvio.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gaiedvelc.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gbajsakaw.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gpbgfdofr.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghtctdrbc.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gkzmifduy.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gxclsvfcc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/geeddznfq.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gtwlmmcpv.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gtxikfdus.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gxnslptae.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gxvwmqhvx.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gkumfgsnm.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gnjbfptff.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gvhsowfjm.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/ggxxiowzz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggncdkkuc.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/glspsvwsl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guqfddghk.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gjvwviasc.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gwgwpyklh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ggmixlqox.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnjduxltx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gjhthzrfe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gvcvvnvmv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gmmuydoai.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/glxnfcapw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gjdfkyyco.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gvzokkxvg.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/ghhhrimwn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gujwgtebb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gchyrtysr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gehqbzlmw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/ggeuhfiqd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gvrovjuus.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gnbhvmtzo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gjqgnnkkz.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gxkzshqrh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gxbsxtdgd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gyjirwemi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gupbqiodq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gwqqpwjoo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gykfygxai.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gzbisoutr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gqwtjdwbx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gurxfwhjf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/ghguekjnf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gyryugvwm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gnvctatkp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gejroolof.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gyjwnyrrp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gnazztqmq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gvttsrflf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/grivjecck.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/grbetydpp.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gtvonflgo.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gyfnkjrab.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/geaxgmfii.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gutoqbadl.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gojasznsp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gnopulumq.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gfpktkyxr.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gkgicvpax.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gahngusej.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/ghbluwlss.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gqcmhpnkx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gsromkhcq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gcnhtcgss.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gmwcqmzdh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gvfztuelf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gpcdwgpie.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gtrhczmrl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gqvjiucjx.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gotiuijwd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gkufffjph.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gforfyxwk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gkvtrquhc.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gkehnicah.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/galxejcna.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gzzuwrtps.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gagjohtlz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/geebkqvve.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gymkvblmi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/ggrmrcyjp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gvpsfxkdw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gbgjdilic.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gsoresqtt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/goukpkryb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/galhsgsia.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gaaaguupj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/glzmqdhuf.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gwfldmgec.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcvdaymjq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/glhfdnlir.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gbtgmzymd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gaftrwnle.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gbojxzyao.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gelbqgbey.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gubjdpjew.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjmyhozis.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/ghrqtholk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gpvjxtxfq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gsoqtmaub.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gpegqjkah.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/ggjyodmxd.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gvqxngnym.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gaxuolhuc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gnhxkfhls.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gsnyutybf.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gootfwfze.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gdfwxzbtw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gftwjgbky.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gmsgefiuu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gtulanbqa.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gslptbbrj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gomymouwq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/getlxqqoz.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/ghonlibxh.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gdsihnsrd.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gvgqepovl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/grompszmv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gyqdvayyc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gdxwqzxpi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/grlnwpcur.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gyyjtcaok.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gpekjhbgt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gvbwvxnfp.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gijxaeiey.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gabvtekzn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gxasvavnb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gfguarygq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gdxcnshrj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gsehulabp.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gplxnbtut.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gnxbsguny.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gctsnynxu.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gnbqunwli.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gmswqtwnm.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gwvqjvadt.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gjmscjoeg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gckdhuzfi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gguubmjja.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gbxljjncp.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gxseqxpmk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gukzgvvfo.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gldhqvolv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/goyugggax.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gbqfcufgp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gbnqjpcwv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gzpjrijro.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqrxpgz.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gfbvafifh.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gcntxctuz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gkpivwoeg.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/ggiqzjlvr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/golfqphsv.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gvgytidad.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gjyevqfew.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gshdrqpjq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gqhaphppc.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gxxsafklt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gwltbahmw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gduwrhrrq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtjcxjvrf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/ginmssbxi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggtwanayz.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gvxiwcyyp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gtkacuukl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gxdufufis.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gdbovgixs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/glafzapzy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gweipduvj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gjacpbjjz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gjenalzgf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gygdtkczn.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gccytihof.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/grnxlvdfv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gibpqxrsq.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gblhibhnh.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gnorerrbu.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gfdofqtbz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/glqliphab.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gbqkbdpjh.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gxmjdhgcz.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gjgetufip.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/geszyigit.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gtybojtdj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gvjiroqur.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwznfqqsb.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gwzymgnmw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gjvshrunl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gvrtfhdlk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnxugggnc.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gamzdveft.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gqeenbhyv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gwmrnphve.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gwoflxhfe.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gnhszvrwv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/grwmmqipv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gtvfvsxpa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gewelbfed.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gwmnmixks.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gmedzvkhp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gamswoxab.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gbffmajya.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gnbltuiqw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gegxnezjg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gqpxfpbwa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gsqlgtnlx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gzwqquavo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gzizgnrxe.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gfshpxxdq.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfkundxjk.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcsrissuz.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gpejwbvqd.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/grgbpcpro.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/grhfsgovc.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ghhbtcjaj.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gdwnktffz.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gaccuiloo.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gqxfzaauz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gkmwlarrd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gsgtiorru.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gtalrgpss.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gjazymocp.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gbhfxyxlc.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gecqmrfml.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gshwgeepa.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gdregjmyx.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gyazidrgp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gmzgexobm.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gunejfmzc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gwvydygyz.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/ggbadaesk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gnxjqyqhf.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gbxjbcrfz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gdfybrlwf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/girhnvfqi.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/geugqkzzm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/ghncigcex.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grddrsaxm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gnqlpueno.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gaamelapm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/givexlete.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gkffdpdzn.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gctgcutwe.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gmzdewioj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gpthgcjha.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gstfcleey.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ghluinrfi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gxbdgnmwf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gozfngzml.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/grnkyyovm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/ghjdgsjmi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gmdoywjko.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/ghttahhsq.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/grtfnhhux.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gmiqktkry.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/goyfunmmm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gjxscndpp.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gayffktwb.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/ghbdhdyul.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gwjtqllhd.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gyvhbvjtp.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gqsaoftee.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/grxfgflks.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gmrowcptz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gkpfxpssk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gtmeuvxhp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/glnxuihbx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gozcrzmlt.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grnekegfy.sHtML


<!-- 参考信息 -->