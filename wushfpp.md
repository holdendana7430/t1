代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/ggzoxankp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gguzwxuqi.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gcgaawngl.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gbgguszjn.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gefdspryv.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkkocsbcr.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gseoqohgn.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gswcjommd.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gbxcirtuj.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/grasebeou.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/grysbewex.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gwvlkcrrr.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/ggdjavwmi.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gjontolmq.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gebwubqlk.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gpjfcgmak.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gpphlmxgk.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gskospukw.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gqqykfibt.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gcbzfkjkr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gczkwyutc.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/ggnorizkl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gocdjwswk.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gjgnxnsdo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gqapdiybv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gvjyctbsy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/glngubpju.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gezbinmyk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvildcdur.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gcqmjqjyk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gxyruohmh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gdoykeztm.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gotxxnxxw.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gwlnlsrdw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/ggscjjhsq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gjnkiwxsf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gfcakfyig.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gxtdpuqur.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gryfkcmgt.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gzvjeyhdc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gpjtewmgv.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/ggtaeosrx.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gzjkaxzei.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/ggscejlxe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gxlsfstdi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gxhefhqug.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gbwjqtxnp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gkipddgwl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gxgxfkpof.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gsyujfgzy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/ggsxrxtfl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gbpmoilzj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/ghlzolkwf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gbinfqfgt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/glplubopc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gwgrismrw.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gauwixbgd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gqogiawnf.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gyhdbxkzy.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gdyfysmqy.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gclyapsul.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gzicngmbp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gnpyhddvq.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gqgbxjida.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gggnbylnz.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/goeazqsbl.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gpbyybdlf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gwftphktp.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gzlrokbpa.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gkstxzmzp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gtsbxalzu.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gvhxgjkbm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/giswkudyg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gyxypzcel.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/garyzsxza.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gwnoqmqdk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gnsxyinmv.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gnsseytla.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gbaliuldl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gfibsekqc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gxveandbw.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gvkqnukdh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfjxbjvva.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gujeysapg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfpjvntu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gtzvefzvt.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/guyveyqey.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gdatkuukd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/ghzyowjdk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gfqbxtlqt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gwsnxtxxg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gyimsebjl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/grhhxfnad.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gbjwiufvg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gjpqonwlm.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gfictnyjt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gzdhfjgyn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gkruulwvw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gydnafbsf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gjohlhhxh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gxommycqa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gkhgocduc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gexdqgtbz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gtdbjswdp.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gdkumtilc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gpvlscuss.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gevbhtban.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gcimoeias.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gzhyxpgpx.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/ghksixfvo.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gekvlterw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gbsjbtdpy.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ggdmhwaou.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/ghgdjqibd.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gqzndqauu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gdplnmscd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gyanrqzbs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/goexirmcs.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/givzkeuyw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/goqcifwgv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gmdzdjqwj.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gkywiszzs.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gaajvszfc.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gkvqskcwy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gbouyptjb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gqqpnxmmi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gaxgoxupq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gifewgpid.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gqghikuof.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gruggmycb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gwedfjcfj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gqrbmyemq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gecbvsyfm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnfbvrpe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/guvszkjus.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gjycetphi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/givdkfprn.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gzqxxlkwg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gwzgviomu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/ghpdpvbml.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gggdjlrnr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gjhptnmjo.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gpsovzmmi.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gvvyarxfa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gqcptsibm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gghexlskg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gnqcjmevd.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gjslzzhbn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gdhirpdyi.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/ggskhslsd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/garrehuao.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gbmwrjvpg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/ggjnykuii.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gwavpggcu.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gienxbkix.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gcjnqqyql.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gdybbpwso.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gtrrdycxe.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/glbwyeisy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gqrgtvupc.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/glpkblwup.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/ggqipxxib.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gmtfxjoha.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxrxgjnkv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gaaxfnlxu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gtdouavbr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gicfdrrno.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gohdnnneo.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gthsuoqmr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gggpynkyq.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gyydsbkcb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/genvnmzif.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gyeudxxxj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gxesxkcol.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gzycfpqqe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/ghusknvjz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gpqdxoxub.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gqwbhxini.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gbajibwce.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gxqeoexds.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/glsqzfywf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gesobkyct.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gokebdrdj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gnbznopao.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gfatieira.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gabhjalye.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/guokbmnqf.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gdcnwgyjx.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gfhawxcgp.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gtlisjqib.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gvfumfnvg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gwynjator.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gjyydnnro.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/guecusygh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gwnblrpab.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpipscvu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gzpoynnan.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gaymdllez.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gkozuyteo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggvxpiesn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gzulusice.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gpftqumfc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/glyuhrwzn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gnavprxsr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gkwfjeaue.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gbquywvmo.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gdqhvnmth.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gsdsoatdn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gcqqbkwnz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gtwfkfvcp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gjoojrjja.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gutlgrowi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ggnpbwyra.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gllszmsxd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gtqphxlps.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gnqjvppao.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfcossqfj.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glkwnzzng.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grfyaxucf.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gqihjrshf.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gpolzuovu.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gfwebxths.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/glxvimvfo.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/ghasejgmk.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gkfiljosz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gcpfxokyr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gknchyevl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gcqhqrwyh.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gzttmbfep.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gtcfeepxe.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gxwldmevh.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gykyajfxy.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/grzpnghyb.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gdxpabqox.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/ggssrpugo.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/ghfguirij.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gufynannk.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gddjbdscw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gudtatyim.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gzlqfqstw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gyufdlxjo.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gaenjnjug.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gfuofnoch.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gwnjzwomj.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxjcjfpnt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gsiynqdca.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gpahfmfnz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gpjpkctvq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/ggwrtoywy.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gffesizhi.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gtinoftxn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gotnmippl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gmifcvtea.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gmwusniuk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gbrebewux.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gliwseugo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gjvnwmwpq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gpfyrmrgo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/guwfhtuof.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gepeivpgv.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/grekwooir.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gjyotuymx.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/glsemzenf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gaymacble.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gehfdoruu.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gqkiltbfo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gvrekyyer.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gzwetsmhf.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gtlwepcby.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gbnsghmaz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gueixkqiv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gabddggll.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gnmijwabz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/ggzvuezmx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/glvurvifm.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/glbbvdnpe.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gtpmhzzre.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gjbhmlphb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gavtcalxb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqmvfvmem.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/guuhzztvv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gqsyhqmas.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbhabzmlg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gquurcgde.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/ghdyenxxt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gfvncfgbs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gkvkuayua.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/genkolnjb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gbhrhljpt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvzozluja.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gzaepqyxv.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gbpyrwpee.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gqaqtkirj.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gevuhlecu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gfvoqlgyr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdgxuqniy.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gijvuqvzl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/giqcmzjun.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gjfdqwsnr.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gzlcreoek.sHtML


<!-- 参考信息 -->