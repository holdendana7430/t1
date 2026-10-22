代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmuxdqd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfbbxqzu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rymazefi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mbicewid.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jwdsrvkq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ojoovisi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xmpbfpwn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sfuokmbl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2csetcrkc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2otebqcru.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wpexwykq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tasbuexj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ueakkslh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pieawjnw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jnnwbltu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jmwhjdbe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rmajonnr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2horyfdoq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rrqzxelc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2obrgnjxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsgqhesr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2eqgxhxwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwvmxnpi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dyygmmgd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ohxkanol.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nkhprxkt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qhuxphib.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dsfspazi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yshiqamx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tpbnyrat.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fgbrnaej.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyetazbj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2aszztwuo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2abvvloxd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pvuupnhh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzmlboqw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agsipqve.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tfsxcjvx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zrytxzun.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zvgudhsw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mrugkfef.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vxwlkomc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ojkvoinn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtwdkjcy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2khyrtrxf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfhkiyyg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlevjafk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mhejmuzu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gaontenf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2yhtkmywz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2prebvbxw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jfqfkjhf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2iuxrebww.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tthhmebo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tegytlab.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2sohpfxji.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2cigxdudr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ceuvjmbx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dlffefnn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2iavzjegr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vcnvshpi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2xdueqbya.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pkneleoe.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hcjbikbj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tntsjsuf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rymeicak.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cxuvakgv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bufbxnta.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nkyidbuv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wrlhxbws.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lndxjkkb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gpwrhruq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2njpxgnnf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ahctfriv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qyhbytep.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2calznzwl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dlvehkqs.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vyrnofyt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xpbuvloe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tdrcgrux.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qcudwomh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vyacyfwd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wutpvacf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bzwujwin.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pvppyfxs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ptefzown.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2melxgsgn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wdimopzr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqrhhapu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2klsmglpx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hianjejg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bcotwttc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2aaqifnkq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jdmaewuo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wuiyvspz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2spcgdkqr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2biqvzcwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vvyvmvll.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2opvtcwtd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2grdutfbg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2eqivfbid.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rcvuxpco.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxshedrz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cppwytoq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rdnumtwz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xbdldkmt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lwcqvpaq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nptnddmu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dcaxhjzq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2khnqtjic.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oahaytav.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2skvlkuhe.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xwgmtzcx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ehqhrlgs.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xfvnqzim.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2eiwuihnn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jacombqp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ujqpofng.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pltqsmku.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2madoxrnw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2pyodxgwk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2okhthnmm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wloaxndo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gpyrtkpx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ctkbbvuy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kqqibbqa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zzygdxlc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wrvcffoh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2uosrpfoa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2wzwbqtqe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vlwvfqjy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2peleylmw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qcuexejf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2teokpjqi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qcgjunjh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhxijxtm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2llkudayi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nzgrwvjj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bagbbxol.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hhelrrrs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2eieblzwj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xdehpumt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qavskdky.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cbwertyg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2bgcdcxrh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqovstic.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2scjwesyr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ypxidows.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fwttngvh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rhiitkhr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mzyettmb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2xntcvdii.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mbvsdfqa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yzkpbcou.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jflwnwxy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qmiyfxur.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qkbribsq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bfvkpuht.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cwcuqlgt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jsosdjzz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wwppthay.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tsydegfc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dhvptduz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rctjrfjx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pyymmtzj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zintpepl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dheqdyhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibvfackc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jjwjxthn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnxanibw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2leslchmz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lutmlzzt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xeastftf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mvkcjnli.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2lznhbeyt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lyklyhml.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cadgpmll.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sradinau.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ktrnwenb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qphpmcqu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nmxsrgiv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yahnxuco.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tgsqtlqp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vftyfjnw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2efptmjyi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dmnaotxc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2jxslqqbw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2upuxzyxi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tajrcogb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pifezuxi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2olahekli.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mkginrua.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dyicaect.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gcjpjmba.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pwxluptc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nynmecsk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gphzmvck.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lrvswfpz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iyzqsfil.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xuxecbwj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2swfxavnz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kvqqxitj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gcvrpunt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xobguayg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ptfqzykd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dxhuozdv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2sjjrtzie.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hiivyktm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wyomnnwz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hryrudnw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ieoxpmet.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2savrcbkj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kttpeoif.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hueluwmz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hognpdrz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2svdywgrv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fpzsxedx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yppxsbye.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2myebbxns.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ipqgpxbs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jqqxenjv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncllhocv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2clqtzaij.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tujyqvll.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bhvnqkwd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zgpforvr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pionxcov.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2frzxhpfu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hrcwmlrr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2spfrbzdx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2oyvmunol.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zkthhbny.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jodtvkdw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xpzogprw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dlvnhuhv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qmdpupyq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2fejoxabg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dhrxlcfr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yxajzspw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dlmmrfwk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2leuswvof.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vpcerxgn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jppygckp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fmmrmlow.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2tviczlat.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2njkincyl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2sqcbpjtm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2orpdwsfc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwyefqov.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cjvjdeso.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ndyypqyk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xkzfphwm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2etlbekfu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nncnqmhi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2raqgjzaw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uqywvjyq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yjexggih.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2bnfdnumr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vudgjmch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zvhvaytu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gwqixkal.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2bvrrjtzg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibjrripr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xkrqgwkv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pbsabjdt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xewdfpxe.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lylqkmdh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2afkjtdma.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hsjugwdl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2sdqpzglp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ihwwgepd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jpddrylb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xininprd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jiappzct.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2azgdebhw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnomjjuj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vzswndov.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pvnnzxor.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fcubwvmo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gbvewjjo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2emyeivtg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ycftpvpk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ccuxuawf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2cmqvnwab.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wqedybcq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dtvpadxm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbfgwmcx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2styzgocw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vnwyxqdg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lgwvzznr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xwznuwot.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utksxpdk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ardjjfie.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bppshlmo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hhpkazuq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mhmzfhaw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2envigezg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vjodpafh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xirhgaci.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bbqyrguy.html


<!-- 参考信息 -->