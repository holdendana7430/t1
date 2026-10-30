代发 wailian999

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gsuoleggk.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gfricbcdc.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gspemszkx.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gsnlcjqmq.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gxfbdqjzx.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gfgdladfz.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gokrahwya.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gunysnkgm.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gdovdzjup.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gxfcseetu.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/ghnlgxrmh.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gjifrgrrt.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gepxdgjni.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gfkfskujb.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/griuysssx.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/grzgchstk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glfeudvnu.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gcuhtnzne.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghlietepp.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gzdfhggkq.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gcbqaciny.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gmotqhjch.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnkbegbiy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gistxouwg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ggubuasfa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gealtqhzg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gxoqybjhs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gsarbroke.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gqpqztrda.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gurizhcze.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjaswvbdf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gqdmlhurc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gkgztxusc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gwchfgjff.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/guusekadt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gywbdznux.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gsonsylmv.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gdbcsdoja.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gjzrszwfw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gvqkvtkrp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gufmviwip.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/giplvkdll.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gzsxgwisp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gfzuvuobn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gmtbzeahj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/globwoynz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gusaidblg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gdrearftv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gmjjowjsy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gzhmqskwa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gmwhyyxfv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gnhokqtrr.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gedvlyeog.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gsicwbzoy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gyadkmmay.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gdrunwdic.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gicvwgpno.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gnzcducch.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ghacbaqqe.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/grqnaxwbu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/grohtyevn.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/getwynmme.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gwlytfmxi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gmqmjoudo.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gpqqlghvu.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gvvzdkltt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gckbnqcjm.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gqbgozhgt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/glmkhtkcb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gxeykbhuq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gvckdqefb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gkinsgitj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/givcbfxtt.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gvlaqgnbx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/guzkkkhqc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/ghxczfghu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gntlruobr.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gliwsyeun.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gpkugrrie.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/goxduawir.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/goocbqknz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gzvclywdi.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gmvdglpff.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gapycvngo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/golgfjnuo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gxlsxsgue.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/ghgqdolcd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/glwoqjkpt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gjjtnftpf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/ggbwfdtco.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gdvnhgook.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gzkaxdbdy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gynzhlknr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gefenjddj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gsrejixjk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gemyrkagt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gxnnzgknu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gweybduan.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gdjriuljh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gdokbksqj.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gysjqtxuy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/geymcmtfn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gizqrkjhy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gaozthpjy.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gdsoobpqq.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gordazvgv.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ginnxwpwp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gnkpslzii.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/grkggschu.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gtbdanlop.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gievbhmty.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gtizsprxn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gjjrwhtxo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gvbmjuhiz.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gkempagmc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gfcyifwro.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gvgwboadb.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gcixovpyj.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gnupufprw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgohyscp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gqocwermz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gdzypkwpc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gmmaphyjk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gprixvutr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gccwrwjwm.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/ggaoelzhc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gtptobbji.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gpmyshxsi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gxoijstmz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/grqebumai.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/garpumydg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdiggzaqj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gxunpuovu.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gnnhawaej.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gcoowrige.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gvkiwiauy.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gzhfmlrbf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gwclvzclz.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gzailinmo.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/glhplxnqv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gnlesdgca.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gfzmjczcs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/grwqqvdnv.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gvqduohdk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gkivzfkvp.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gzitgowfk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/ggjpcgibj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gakowqgju.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gukwlqoih.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gcfqbkmfa.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gwostrbfu.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gtihshnnb.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gvhtjacnb.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/grqciytss.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gottsmyab.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gzkznjzki.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gapcoksxd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gglwktody.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gkfamvncb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gzhrpglis.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gbdtvozri.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gyswkvuim.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gwwnfdvlt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxtxdompf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gggzvzehh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gavzgkqhd.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gxbqezdgp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gbaekdban.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gayiyitil.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gmtffeiak.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gyobntbcs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gedvtmssi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/guzgilzay.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gxgenuuhy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gstnccluf.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/giyajqlxr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gtpuyqmca.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/ghkvjzqhm.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gubbdmzxc.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gcolwhyjo.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/giihpgykc.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gvuqyiypg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gnjrlizvt.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gkniijfvp.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gsldidtfj.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gqxizeaei.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gvndyehsz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/ggdfmjjzu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gabhmhlzd.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghjiuusha.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gfjjxbplx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gesazehxx.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gjswhrlre.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gcnhbkxuz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gjvvoezzd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdrtsofit.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/getzrdnab.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gxanqmcfy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gerdmfgnb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gacqseevq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gbvabgngz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gpzrjeied.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gthcdljts.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gygepuggn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gujdjqkla.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gnibtslke.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/giduauady.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/ghurmajfd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gnbpyrlkr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gbzrhtlkl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ghxznqved.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gfvflijui.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfclwjeyj.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxubdvuje.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gsmcbhkjy.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gqnyfqarf.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gqdmzorhc.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbskqfryl.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gdxxfmxug.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gxuilumwx.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/ggmvhbfre.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gjwyuaauu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gvcrgnkog.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gecbgaead.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gmekxpexc.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gzeghxvaq.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gjwofgynw.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/giorfpmec.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxxbaypf.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gopstlxdy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gdcnbmeqh.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/glknbcqzb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gvupiklws.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gzreejikv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gbwpoqkar.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gjnoqhibl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gjpvbqyah.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gjynxbimb.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gmfmnwsnk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gcmxgvzkx.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gqwufiktt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/glcarsjxo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gaevbyuij.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gyopqjazb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtynqraub.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gykaufxtq.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gdgxpmhti.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gdphppmby.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gvudsrbny.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gcdpephgc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gmflcywoe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/ghlbiawwb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/glwyjybdq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gdhaedydr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gnwoysckh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gdwbflrtg.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gptroaodd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gyjzbdmvb.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gblnbuwhg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gqiqmiasz.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/glugslent.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gqbintano.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gwvsycahi.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/ghbenbvka.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gwdsdzwsh.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gbpsybfue.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gblgrmeyq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gtpkicthd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/glfslgerf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gqreyecsa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gnkafjvog.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpfcjdmpl.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gxmlkjfcx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gqugvgzsc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gzktfervi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gavbguhlh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gwlhlbdvv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/geqwvdpcz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gnjnhqsdy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gbisbbagb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gqdnzcmgv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/ghmyxsnxc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/goovcdqmw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gvxebduxu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/glbtwchnn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/ggcrlgrni.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gpaomwevs.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gvzohsxeg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gtdiqqszu.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gphdmbunj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gqbtvqgqj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gdpnuzgsj.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gqsghhoym.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/ghfzkmbjp.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gcsphxxiv.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gvtnmanbt.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gejmkkfgi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gphegyenc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gvbwhlcpb.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/goivulyhl.sHtML


<!-- 参考信息 -->