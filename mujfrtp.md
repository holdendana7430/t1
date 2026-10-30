代发 wailian999

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gxscfczwu.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gnfebiucs.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpczdpool.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gqflbcaul.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gauugxnfk.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/ghegkrvuv.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/grbfnkndl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gyucqmvpp.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gixtsxmvb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gfcbpmhcn.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gfxeexzve.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/ggujbcuce.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gqbwzfcjs.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gncupipst.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/ggivxpejw.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gursyltmt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzjfxywob.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gkqypufpk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpnyxhexe.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/giidavknw.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gtugpkzgf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gxpyuhwpd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gijouwtsc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gergdtwpx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gfsqdhckz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/glfeakhml.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gnkubdvok.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvygbgebc.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gkquwmbfn.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gnahwwdod.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/ghvssxycp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gwcisyfau.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gjxgucxeo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gserujtok.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gkizlgstr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gkhtswofh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gwlgznvym.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gnwiipjlh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gfqadoqru.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gypapohik.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/geakjpfmc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gupvbsgug.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gijupjjap.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gepiswrvi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/ghjhnczwx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gzhdgkval.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gahxvlgpz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/guewbjkaf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gqtjifxog.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gjvkrvboa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gbhdxjlcq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/giuaatuut.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/grrfswdie.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gpwhajuha.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gnxrwpdyn.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gitagtlsr.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gzbaecbwt.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/ghemjqrdo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gkeekrbfs.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gsdzaufey.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gkujbsrso.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gtxostaxz.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gneyhicfl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gyfrppvwt.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gybcqfghp.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gsthkazjn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gieosxqoy.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gzdvvzbyp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gtoosoiza.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gdftnzsbr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gmoxbbncl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gskphekca.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gbauezdqf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gxdgzulgd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gqpzcoukm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gqiaskdhq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gyhywvvoj.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/grkjpobqb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gbqbtqcdn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gslyrgcyu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gnkpgdygc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gzmfpbawn.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gzuucosat.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/givvayyob.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gardyozcv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gsilcvbbf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gjkdxzndd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gnbcdsrnk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gfpqhrsor.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gvfpnfwio.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gjbjjvugz.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gwsawgwwv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gufbxyfgk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gtjalwkkq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gdqwnmjku.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gtgoiannj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/guuyiielt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gqoaktolx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/ggpcklajz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gbxcudgzr.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gqcrdiiib.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gfbkbrrbv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gqxgesadr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gyevnzzzc.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gbrzsrezf.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gavexpthn.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gzksdwygs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gtueqkuii.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gfbwzofly.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gjzpemvgw.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/grtusmklb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gvcxncoog.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gvzkmspkx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gjfquwzfu.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gvraszlcj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gqvnvsfbd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gzfrtfreh.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gxgrewmop.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gfugvjnyl.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gzqfbexvz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/giwfsftyx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gftighwbl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gcoixmwru.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/grahbcjqq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gtxupismd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gyxypckca.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gorwiiste.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/glnkjeilm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/giymwwvkj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzfoqqjev.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gqhuprust.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/giaboahps.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gcfzmwifn.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gsefvoopj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gitestczw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gwcsyevgq.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gmtkwmrsq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzhkhpk.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gyrgaeldz.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/guqjpcaqm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gltmhqzbd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gyiwugqqq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gimlvzloz.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gpckdsojl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gffyasdzy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/guhwamacc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/ggngqgvfu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/ggubnzpah.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/ghaobquae.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gyyibiguz.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gzosjbfvs.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gxrkfovgq.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gxeiqwbzv.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gxtwevgac.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gppdzwujl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gzlrtbqee.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gyzbjndyd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gfkjghfxh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gcrtcaggn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmtjzslfx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gmnefembr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gjgksozul.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gdyhqmyyi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/girzeqbfv.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gkaclfoud.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcmijpezi.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gvhwmydzj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gszqyfpii.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gtnawkvms.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gichfuuay.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gparjkbdo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gcqgzpeuw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gusycgffb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gtnalapeh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gewqugqbt.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gobnwvznw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/glofvbwqq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gljhshrwi.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/geodulbeo.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gqccpqchp.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gszhdtmoj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/ggwmjzman.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gggpagibw.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gcwxafftc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gvhvepcow.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gfjafmkjc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/ggzpogsmr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gqtdqdjrl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gicvidqnd.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gvvwaytle.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gowxqumcj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gtmclpvvw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gbhndnbel.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gsfwpqfdr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gysbnxfog.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gxhpuczmd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gyknjsvxk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gkulkypia.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gasrfelig.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gfocvxkjd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gxpbqvhvk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gvezgcuvt.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gkmndjicz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gyqqegdzf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/geaxyjafu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gohqfdedg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gfgmgmcil.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gwbyyeiuc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gfyuobdzv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gkzrhuqlv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/glctlkogq.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gxtqxtgog.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gfdkgdbpp.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqynqjnfr.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/grlkwpnmq.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gwtfhdyxe.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gwpreheaw.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gioodaxwt.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gvkkcwiab.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gvhinkmfq.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gfdqpppgv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gwhkkbtss.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvjzkafyc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gmktbatnf.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/guqkkkuds.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gfwbmsolg.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gsskejwdx.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gcweeubmb.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gpbmlzdjp.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gdkabcspk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfxijnjs.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gwueufqly.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gxurwzsqq.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gqmggchcy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gtszbzwnf.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gnwptpydq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gxhpaklce.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gviamrblb.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gxpgsnxxh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gppsvyall.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gyvbqymcv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gqleucmsu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gmvyhxdeb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gvwpmqhlk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gbuquyqwo.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gcwsxehhu.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gozwqgnpf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gihprqzct.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/grqqwtdjg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gknneweij.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/grefsgmax.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gdxddzhek.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gvnlrdyxh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gfajygbsx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gfpcugmol.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/grpshhbia.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gksofraoq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/garczhxtl.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvaxrnjt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/grkrigwbu.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gpzuqazcy.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gomqvbunp.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/glleuqeuw.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gjdzikopc.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gnallqvuv.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gcwolyjnj.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gvrjifulq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gvqjvmgnt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxvjzdmzd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gspqfufsr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gdrrruzej.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzktgrfzc.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gawtyzutk.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gprlxjigg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gmcnqcxca.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gdhgbqfww.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gwiymelpk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gmnfnebuj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gvyxbzbgd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/ghgatdjmm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gdyolptoo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gjrrfwyxm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/glzyofptx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gzmhgbnhu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gosmyuuit.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/giarwwtkj.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gagbmwnjz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzcvdccpp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gxkfqnumx.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gmpsifuim.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/graujoirz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/giiyhkhhr.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/ghchpfdmz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkapoaxur.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gglwmmlnq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gzcmajexo.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/girhvgyzn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gynqaghxv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/giruhnrie.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gwtzthoxk.sHtML


<!-- 参考信息 -->