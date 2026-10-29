代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/ginodnsjl.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gkrektgxq.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gncvkupgd.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/grtljznnk.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gfpxlixvx.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gkrtyxxvf.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gkfzvihdm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/glzkksitj.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gpoaadzvd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gwgmdrqlr.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/ghywdqgzf.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gvibvsmqi.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gxkqhspin.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/grbkqqmua.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gxntslehp.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gvurchgoi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyscioctu.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gysieldvh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gholcndqp.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gfarfswqn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gmkidompc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsjdevrjo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/getxdcouk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdzehyeos.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gjphyhbmi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gkpnjtpdz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gtdprsotu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcgeumgfu.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gsjxjdqhb.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gykvqinne.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/grqiwtjxt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/ginnwgais.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gyzkcyyql.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gdcngvvvo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/geqpiurqd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gmwcghgyx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gonrxhnqk.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggxwtthvf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gcajhfsly.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gjoqchfum.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gmzreskyi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gfgytggdm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gdehprsnr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gdtxzpmbp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gvvxxvnqu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gwzthbdnz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gfzxutpdp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gsqaccvdg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gkluxfoba.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/glpnrktme.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/ghofbfvsm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gdgchdcof.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gwdjiqipp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gykmjspcm.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/geguoisie.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gfsfqzarl.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gtywqvyzx.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gunuaxbpf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/ggtryvyit.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/garpzhpzl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gcpamxoyi.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gzhiovylh.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gwukjbqxa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gesfktiwv.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gmpxjfkzk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gaimlyltd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gqcephmdi.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gfqqhyilb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gnqmifqwl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gegoenrni.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gnrbsewoz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gfbrccgzo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ggpeobzxo.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gjzkbwhtb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/ggqxieysu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gcaijczfx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gkevtohvs.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtptxwid.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gigwotokf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gvsarqrwx.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gwklcclen.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gdmqgpjci.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gygwvnmme.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gcnsswxqi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gusglrggc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gnafxqqhm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/ghmdrckpo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gutawinhi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gnvmsjusr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gxsmuzbne.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ghxoktkhp.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/goowegogo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gewupuaqg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gmhljhoty.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gxatumxrd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gsemkjdcu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/ghioumubm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/giidmwvtj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gbeheiroi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gbtfaptzs.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gphrujojd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gyicntfjk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gosahuddi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gzdqqovce.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gwoczqaib.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/goorlycdw.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/ghjidivxa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gjfojpggi.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gswqvxtqz.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gkhwelhnc.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gqmhochor.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gvulrrzgz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gbnkmoihe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gkmsajftt.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/guxjvddpo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/grhcbjahb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gpawopjqw.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gvdejpbyo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gnkwhocmt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gqfaxhlvs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gzamkhylx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/glyleumwo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/ghnibsrqz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gnuzrgcjx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gwlttjhbl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gzlprugde.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gwubhsbzr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gvobscntk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gaexeyijx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/ggzrokuom.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/geqkznxke.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gceeegrci.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gklsanubq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gspzdnqwx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gfhntelqb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gfmucdtou.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gixmhnnhu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gkcwqsauh.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gczpqffcn.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gdxmmynko.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/grwxoqvbp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gavcjunmv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gyezrebli.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gxcxnvlrj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gpnhaekqu.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gckocuzsm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gjzwhjydf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gcdwbphph.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gmtsqdqcu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gwacgjakn.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gguibhoit.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gqkfyjppr.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gybixvhvd.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gntcrcfbt.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gimtiwgze.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/guuqcecor.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gepefkdoh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/grfqpuxrv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gksnxhbre.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gxjydrnrm.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/ggjuyrbtr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/geexyomat.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gigyqnuuw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqavaodzd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/guvfmcbck.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbepzdtsk.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/ghbyqxnia.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/glbmolppc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/grucvjkaf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gasttmvgp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gobnsaewb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gfcajqfyq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gsdqshxzt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gduhdiwcl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gyuemsdsd.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gqgtzprit.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/ghqwqryzn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gcnjkgmgo.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gxkvuuwzl.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gynojvulk.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gmfylneln.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gpcidsxju.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gnabqphsm.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gcqmkouqu.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gbmthlyaz.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gsailkvmu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gfmaorzvm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gutyxylzk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gfsvcpcxs.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gcmuawikl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gtpmddmzm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gobzqtksz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gqxrkhrhx.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/ggfoppzfm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/guwfczeqt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/grefvjkrn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gcqmbbipm.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gpxtawfmu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gnjvhfqce.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gvbzvnqrm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gdrzcefjj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/girynahxm.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gkcnnhwax.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gyhzzitso.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gnzqzlfof.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gkvzfyosy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gsgiotyjn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gibcxpnru.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gsiqvovce.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gxwnmmwpy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gfqsfbjav.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/giebscrqf.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gvujtcgob.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gzulvdoqg.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gasgezbtb.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gqwkntcvk.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gtwmwboss.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gsomsjbvj.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gsrcbbhmq.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gneacnqzc.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gvejpzezg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/glstdljbr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gjlmlsktn.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gpqozojfv.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gkaffiyua.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdtutprqb.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gyjunfqdv.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gdnqzutaq.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gbdrwmgoe.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/giukwnhzr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtizyanb.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gzczfiesa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gmsfaqwok.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gpxrsskmc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/ggvzownhz.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/ggwyifxhg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gvbydhybb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gvwmraczo.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gasuklktb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gdgosupab.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gqrcpnwzs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gqgojhacw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/ggwxmhlyl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/giicdexcw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gygxzptkr.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gqerpqeih.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gmznkmiow.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gwfmykneo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gehmjsgap.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gjroonidt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gtgtjakdg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gdxcxjftm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gjdgzuobp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gbvpfohrs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gqcdlapxc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gklntlvhw.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gzivbxedz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gxdqwhprl.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwlblfozm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gytumlsdh.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/giuhnxjyj.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/ghkixxugl.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gzzxvtogk.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gldisdsvy.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gssqalutn.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gihhuczpt.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/ggbjorzho.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjmizuqfc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gpfusjdwe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gcwbkxprz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gtvygabtm.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/grvncsqfs.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gretpgnpe.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gnmpgrgxn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gjsffqsjg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gbezytnnv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gicxawnve.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gjqqhtowo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gemysydoi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gaqjphpqc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gsnfupdrt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gwmnecxmq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/giteeyyht.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gpxhjkshe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gvcwftjsz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gxwhegtog.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gnayevcof.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gupfkkwzr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gxnykahja.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gevrlgkwk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gadyjtroc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gdxquwvxj.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gcntsmcoe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gyrctgyay.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gvtwibbgb.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gnzypqgta.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gwknsesxe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gjjpicxop.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/ggpbmfltk.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gxpqacine.sHtML


<!-- 参考信息 -->