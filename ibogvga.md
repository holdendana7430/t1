代发 wailian999

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/guxsahdaw.sHtML

Ruby: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfghhlb.sHtML

C#:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasftgmjb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gottyefsx.sHtML

Py:   if not data: return
来源：http://wap.fanxiaobao.xyz/Article/details/gwkirsgyn.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbglumfsb.sHtML

JS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gwnvkkegt.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxmgcugm.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqpybhsg.sHtML

Go:   if data == nil { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/geqgihcrp.sHtML

Ruby: return if data.nil?
来源：http://read.share.fanxiaobao.xyz/Article/details/guvnfxmdp.sHtML

C#:   if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gemogoksd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsasbxhdr.sHtML

C. 函数与作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gpubkwebl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdpehwfnx.sHtML

[C01] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/goyuplggj.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gebxddezl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazgkdkyl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gspgfnist.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjjqovun.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/giilcmxyq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gvjnxjbbj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/gyxwxmyhi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbswbqaws.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiikexfq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgcfurcp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmxbuorwj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/glrntwvot.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbrycixx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gehvgsfwv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gviciipag.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gktaywckx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlfqdgec.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/galfhlwcr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoiiwlzu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyrmbfyss.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gttlowvgs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxjcshpy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gojbwdcfs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnmkmuqo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gevfilgxx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fanxiaobao.xyz/Article/details/gpoyqrswz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gknxskvbg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gidpofphv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpeeaxsw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnybpgqun.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gsijgewrc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gjmcrqaqq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjaaqbng.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gywyagxsk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfsmqjjm.sHtML

[C05] 返回多个值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgitmbfy.sHtML

Py:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gousezkwg.sHtML

PHP:  return [$a, $b];
来源：http://blog.fanxiaobao.xyz/Article/details/ghbxwawxw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlknupgg.sHtML

TS:   return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/glglfyqzf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrdvrqor.sHtML

Go:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwreubju.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkricnev.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fanxiaobao.xyz/Article/details/gthktivrq.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gzwwqcakl.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnpvqfff.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmojuczp.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gjpjxvlrr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmuolktq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiekrvmk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gvdfdaokt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gzyetvowt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gazxiljdj.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gnnlgkrab.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffiyydog.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/glzykruqx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fanxiaobao.xyz/Article/details/ghhwulqwe.sHtML

TS:   arr.map(String)
来源：http://blog.fanxiaobao.xyz/Article/details/gdmnjdjqi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbdlrffe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fanxiaobao.xyz/Article/details/gnabnqhdh.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fanxiaobao.xyz/Article/details/gilbqmden.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdxrzsyi.sHtML

[C08] 闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/grqtpsjtd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/golcejnpm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/guuzjpsuf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaxdvqmv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gudrzzdva.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fanxiaobao.xyz/Article/details/gvzazrflw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhtafmhr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fanxiaobao.xyz/Article/details/gwglknkjq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwdtnqgg.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/gqnhaamlj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gspxyoxly.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gggrztgie.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gxfljwrvp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrdbbjm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grbriqrkn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fanxiaobao.xyz/Article/details/giguimlmg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtxpqvbja.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gchrgahmj.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrbpzihq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnqxafgd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqqctiks.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gajqtyawn.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gydznscxk.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmxnltmw.sHtML

Go:   花括号块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzwlnwqd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fanxiaobao.xyz/Article/details/gqgepoltn.sHtML

C#:   块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmlttumi.sHtML

[C11] 模块导入与导出
来源：http://wap.fanxiaobao.xyz/Article/details/ggfntwzec.sHtML

Py:   from module import func
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheuwpcct.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fanxiaobao.xyz/Article/details/gmfaxglxu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gnijljerb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/giahdesyf.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/grtwgqoup.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxhoattx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/gruwcxroi.sHtML

C#:   using System.Text;
来源：http://wap.fanxiaobao.xyz/Article/details/gzdcglrnk.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxstdwaz.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fanxiaobao.xyz/Article/details/gmoybzegw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fanxiaobao.xyz/Article/details/gyojayole.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkzodsit.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gwfhbpgoz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwyjzywx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fanxiaobao.xyz/Article/details/gltpfgwkh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqqkjpjy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgioxdii.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpmuymun.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gqwysirwt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdrbnxve.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fanxiaobao.xyz/Article/details/gecgrwjxh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/guuqhzltn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guhbzuuwa.sHtML

Go:   func add(a, b int) int
来源：http://blog.fanxiaobao.xyz/Article/details/gjtumxjvg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutxqsbgr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goelutcmn.sHtML

[C14] 泛型函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrlfgqxj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsynctgx.sHtML

PHP:  // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghttvaslb.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gyygjtpbg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqysitona.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghktltdmo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fanxiaobao.xyz/Article/details/gjcvjozih.sHtML

Ruby: # 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/guepcrpss.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fanxiaobao.xyz/Article/details/ggkldxfjd.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahgrvtms.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjussknas.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnddxmqec.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrqknfrq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbgdtqkv.sHtML

Java: // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/gzpnugagf.sHtML

Go:   // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griuhdxyn.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocefllxx.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlzndhga.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaxopbdw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gfardvxyq.sHtML

PHP:  // 无重载
来源：http://blog.fanxiaobao.xyz/Article/details/gwhxqblcn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmmnxvep.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gdercpikm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/goggmqmcp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzhbgbgs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtukkvqcm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gohnkmpbr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goocvsvyk.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdcmgjks.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlxylnkv.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyesgqcng.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fanxiaobao.xyz/Article/details/gqqijarwo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmckpqjf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmftsjtid.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgkkixyk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmrhkmps.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgndyvcq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/gvrcacdbk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fanxiaobao.xyz/Article/details/gragbxjss.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gnresucsi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbwtolwt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqryvkhw.sHtML

JS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gafgwiqac.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkanlpgf.sHtML

Java: list.add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gxrpaaswo.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gfcxszozr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrhaykfp.sHtML

C#:   list.Add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmxksepk.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcqcfvkr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzfkxour.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzallpxr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpvpvqoq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gmwaykeqx.sHtML

Java: list.add(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhkkwtxs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gaobpkqkg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqorkudrc.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gkijlohdw.sHtML

[D04] 删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/goaxlfkqr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/guqhyadwz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfcyppes.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjaneych.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gmahqykrb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbkxhdhv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsluehnm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrmrckhw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/gkbsqgsoh.sHtML

[D05] 访问与修改元素
来源：http://blog.fanxiaobao.xyz/Article/details/gzutzixbl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/grkicqyvy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gsfmjxdgo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gxrqnzaac.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gafpnyqcl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fanxiaobao.xyz/Article/details/gbfgdqqvs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmmgbmrn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gmslgjysd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gkczzbiaz.sHtML

[D06] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gkpzncsbi.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gektdfxrq.sHtML

PHP:  count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/guwtdbhuq.sHtML

JS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/ghcfweccq.sHtML

TS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/glruxjfhe.sHtML

Java: list.size();
来源：http://m.share.fanxiaobao.xyz/Article/details/guaakfwgi.sHtML

Go:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gjtptrjvf.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/glrszbmrj.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/gassumpqu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gposforbr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fanxiaobao.xyz/Article/details/gkzwdoywk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyatzgow.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gpntkundv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyfrfxmd.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gbzfbmqgi.sHtML

Go:   arr[1:4]
来源：http://wap.fanxiaobao.xyz/Article/details/gpjwazjjx.sHtML

Ruby: arr[1, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/gpumpjrkg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmddhrtu.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gepuojnkh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrcnuqel.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fanxiaobao.xyz/Article/details/gzouyimrk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkacwyamb.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/gswmffffi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gloezbzrp.sHtML

Go:   append(a, b...)
来源：http://3g.fanxiaobao.xyz/Article/details/gkevgukyc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxqczons.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/geeunibci.sHtML

[D09] 排序（升序）
来源：http://3g.fanxiaobao.xyz/Article/details/gfhuqthpk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gqhgazfsg.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/geeoevwfi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzikceyk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhdzlevw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsesjzno.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gsuubnlxv.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvybyqjx.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczttvsix.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fanxiaobao.xyz/Article/details/gomuvvgzl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gpvxnibhv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghauslraz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/gykehxhed.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnpwtzpk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbkdigog.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fanxiaobao.xyz/Article/details/gewqrhdtw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fanxiaobao.xyz/Article/details/gwfskbofs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqkuuath.sHtML

[D11] 反转数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gwefhslsx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxztkzowh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaudjtcx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkqpabha.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxyhcdsx.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxrbjrpe.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhfhutsi.sHtML

Ruby: arr.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gvezemeuk.sHtML

C#:   list.Reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gxhwchszb.sHtML

[D12] 查找元素下标
来源：http://m.share.fanxiaobao.xyz/Article/details/gszxflnph.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gmokuydvy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gctwsnlna.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozwcihca.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrthtzrq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fanxiaobao.xyz/Article/details/gsrvzjcuo.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/glxkszlhn.sHtML

Ruby: arr.index(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gwhykmcyz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevreuxkl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoyxddqf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gownezoev.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfankxmoa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvcegkue.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/grygtlllu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gdxqcuczl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fanxiaobao.xyz/Article/details/gdycsdaho.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqvdtdsj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gmnzsziuj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fanxiaobao.xyz/Article/details/gxdnwztzt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjckhust.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhqpffbm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpoonqpqy.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjayubjtp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuvzlvds.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/gsmoywmhv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzybdtwv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gnamtomxr.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmasqyjoq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gasndtxnm.sHtML

PHP:  array_unique($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gyztfiehk.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzhvdpcb.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnqzgqpv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fanxiaobao.xyz/Article/details/geaxurvup.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwqgayck.sHtML

Ruby: arr.uniq
来源：http://blog.fanxiaobao.xyz/Article/details/gybcjfslm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gbpnzncjg.sHtML

[D16] 求和与平均值
来源：http://wap.fanxiaobao.xyz/Article/details/giicauyeq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gurngxddf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gccvkcyfz.sHtML


<!-- 参考信息 -->