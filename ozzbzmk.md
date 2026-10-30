代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gygqgkdls.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/goyhqshkt.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gsjawycuw.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gmkjyvwht.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gcplxkdpa.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gxeecsjwd.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkztrgzhm.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gawlfcjnh.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gawopapll.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gmtppeclc.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gsoqymsmt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gwxncdjbe.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gktpcmjyo.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/ggphngzpp.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gknwmilay.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/grptzakup.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gjwkcywqd.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gtrsakuvv.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gtqkstuny.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gransrswp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gddtwpzbx.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gikrihnqj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmlsikord.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/grrotiefx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gxpzegmzw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggznxcboy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtnikoshw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtnzoaecu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubkcqfph.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/grwjindqg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gbemjijoo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gnlnfdzhu.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gxodyuwmk.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gqdyfepfm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggzhghltu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/ghvjzbabr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbnrhsnny.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gcqjnumtc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gilrqrhvw.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gbxjfdhav.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/ghnidjjjw.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gikxmgiaj.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/ggnlgaxkf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gzxnmuuum.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gueuftomq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gwzwdutay.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gcskgxpju.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/ghlgkamus.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gcirijoxx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gkubezovi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gedkqpubq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/ghtpumint.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/ghmilpjkg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gojbtmros.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gsjtpwonl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gsiabighf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gvfkcvdek.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gijsjlvvg.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gnrfvzvct.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gkkevoluo.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gxcuibnrk.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gqugwtpah.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gmguskogq.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gcaybcdek.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gocmnydeq.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gzkqzjvtp.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gsibtclre.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gyzzpjybz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gtwnuuaze.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gvugxhnvm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gaaicvpzk.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gjcdbhmtn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gepbwzzex.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gktlplbya.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gmnemlxgi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gavibofvh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gkrqkglpz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gxgjumswr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gdwjxvjdu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gflkvrhps.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gouslupuk.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gkqeiengk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/guabyfbkq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/ghfkllahm.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gtaypzxnz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gxvneuoaj.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gdovopglz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gyjldolra.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gslgdpejb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gfsimdmjt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/grgsvwdni.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/guesizgez.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gikbxsubo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gnamwbocv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gxxthfbvc.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gddosusts.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gjkccepna.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gectjnqdc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gjckubiqb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gnllsamlu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gurymmxeu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/grpijbllp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggoqlocne.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/geklyqtmx.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gzzuwmxmb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gzjieqygr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gmxkotjyj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gzupykwjr.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gypjqyeyd.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gspkapmyi.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gszynxhzx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gorbzoedk.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/ggdvxdtxg.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gqaboyopf.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gmqkscifv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gahlyzdfb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gozhaagfp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gpiweonkk.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gmdhuutwr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/ghrfzhzzo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gbhkauzjz.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gqzdzjlmg.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gsrcjiaux.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/geiinybvx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/ggmmjbpno.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gzsnekxkn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gxcaevfnl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gkbqypaeo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gdwgadarq.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/ghphekjuy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/geioxmqpw.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gfvqqabfv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gbepfowgx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gnectyjqt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gfpxofkxw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gahhkruyd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gpugpwdqk.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/ghgvnzozl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/glnvhqebu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gqrxtjbqw.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gufbyperx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gqjefskbs.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/genlyjwdp.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gtrepwokf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/glodfnbdd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gopltunyk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gwgnkheig.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gbwcporpe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gmbjgdbwy.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gnecyobos.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gysmnwnfp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/grqnfksto.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gomeeofbl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gxhtbetkn.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/ghqxiavix.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gpbupipzf.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/ggkauitvv.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gvngnqcmn.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/ghfhkjcxm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gjubxruvb.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/grkzyqbev.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gmorsdjsi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvlkfie.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gacxmsofm.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/grqjbghiy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/grgtwqfwn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/glutwplya.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsuintsog.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/ggumxhjqo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzdwyibjr.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gozhzicmi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gzkoyeeiz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gfrhtzosd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gtbvaqoms.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/guhuqhsrx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/goavyougn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/guzennmrt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gtogzcday.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gspobyrlh.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gckpcmxgz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gtbuzgqrl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gysmppsow.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gkjtbwpeg.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/geqhbmqdy.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gczvsosau.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/glhwdwfms.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gtjyaexcg.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gjorattae.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gezvzxbwj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwdunlpjb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/ghfrbnxfy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gccheovye.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/geawvjlft.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gwaiolovl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gajrkqcaf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gcieedqfq.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gojirzuye.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/guaepgrgu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gpmfcsbzn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gobqvfggx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gcfvxjqvw.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gufltmsef.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gqzybubew.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gxfbhhvlo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gvzxbqipn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gnbncxmeo.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gmukjvjes.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gcumddaba.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gnjojtzvr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gsyyvqadm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gyuoqoomu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gjvcyjcvg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gpnyikcex.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/goiddhhpw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gnnkfxxyj.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/glqooswog.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gjnmgigky.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gdghbyhlf.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gsortqdey.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gnwhnuoss.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gbkhrkcfn.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyxmtvjtg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gcggixbqb.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gbhgcbkel.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gddgnlmlz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gfimglbcv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gquwracdp.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gnurlvsfi.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gwkcqdkis.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gqgklgmhi.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gqdckenbq.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gbmwknjiv.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gqpgcgibr.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gpgzlwqkf.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gjriidutw.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gclyauato.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gzbbfdfae.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gpeysqyal.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gcnkspysc.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gwehtojmz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gjmgzsdgv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gdrqvtbky.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gclocgicv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/ghxacotlr.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwpztowjl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/grkowjbil.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gkqndzxmi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gjwchkzgu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gbiujstaw.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gyifkokxt.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/ggovzhalr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gbukztwup.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gdrttbtwb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gltbmonjm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gkiicvopi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gkrphnzmd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/ghsqlnumc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/grwqbnrsl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gfedcjdsw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/getwlibbt.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gdzsqsqzq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gnmcptzhv.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gtjieilxc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gmbsojyme.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gvrtqpnev.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gjcxzefrs.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gdybdtgol.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/grrjrmors.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gfkknjlti.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gnyfrpuov.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gavtbxqcp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gifwitskb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/grcewabie.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gdxxdtbrn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gxafztbhy.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdcuawcmq.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gsrlzmuna.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gwjuphabi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gmhsmevun.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gnndfujor.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gwfkecacj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gscjzijjw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gonbxtgnp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcvasgqw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gmnambiuo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gvyckckld.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gmznigfzy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/golswacvz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gqujfyhhg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gfmzblraa.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gutkjoxzw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gvuwmedrg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gtdpiixim.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gfsinvhii.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbcicmgck.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gryafgaaz.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/govtcgxww.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gopnyfdlw.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/ghxvcprmp.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gtlrwyoql.sHtML


<!-- 参考信息 -->