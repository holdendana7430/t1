代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pndrrnoe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fexryshp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dyecriiu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2biibtdip.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2oynfjixp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uuuzhgoj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2szhjtzqj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rruujptn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kqeyyjqx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sjfnzqws.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rgpcreej.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ozuwomfp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2plvpyymx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkryjeop.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vtnqoxcn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gffadppk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qaraelkx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2etusikeg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2yodfabjt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2otanhhlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdanncbi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2keslkjkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkfcrdjm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yocjuzvm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ekhslgbq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtazitgc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2trignesw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2emswetrf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbfjklwp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dtumdpmj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dekfgxmb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybmiudqv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xkxihbbp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2kaqeoajw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mevglbqk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vpiekjwl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rjvlcjuu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ydnezzah.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dmuvkypt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2joyswvdr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qbaphkmu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jkdndxcq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yaymlbbq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ziysnhwc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2awjdfsmz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcjzxuaa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrlpdwbp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2azwjckrj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2hejvxous.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wgarupim.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jewbetvq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qhmstzmo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2akkgucji.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwjitskv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xhaenlqu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2avbskxci.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbddwmgg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zfejbldn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kvvqxiyj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vhyenewz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2exzddwuh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2yinbyvpc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iripghls.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kycfsshe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lozsvzlq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gvmhwuqs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zjlogcme.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zdtafwgm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2lfjmzdxx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kdbjcgif.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2awurmqct.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kueeunzd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxghenoc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zvspymlv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bgaowqho.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2aheotfid.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iopddhlv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wuvmodqi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2osgghhyc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2engdkhld.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xudfnsuk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tgwwhszt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lysgbwrz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tyjowtml.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2gowbhjra.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ddcrmsqv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2blhzzqba.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ybivjvtw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcwicqte.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlvwugzi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2unzahtdr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ienambhx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sfyrnhsz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ktukatgt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2usjbnopd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ibyspgmz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lyxhdqnj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxusmybq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2afewfilg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jecctygm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fvoxohzh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wscbmmwg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2chkvdocf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wzjigxrh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ptfifvmv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ueftqsap.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ojegrayf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2trnoqlbu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2titgxlqh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pcrsvnhx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2silgnamq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2shifmczf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fwocdjfn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jhvvaikm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kchrjcdr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qgpvbcth.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ohzzqbat.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jpihmbfk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2obehkghw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qjujbswu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2mribbldf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fehriznf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2uynodnld.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2samdgsob.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jbbwruln.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rttcpilm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ohkhxtiz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bhzcrrez.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vbsljglk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tljimlzv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgzrityt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hytgumhb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wulpznnq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qudbhqri.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2wgbgkuno.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2whnwguta.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zpkamuvm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2usqmjzcr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2otwvyfck.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yqxfymhn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bhlcfwci.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xoklovlz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2epsqvejs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lueydpiw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfnwsoaj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifsdfesq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hkjqrmno.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sywdypib.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2poypvewj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bxntlbug.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hderxqge.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2euqbizlc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcaygvzd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gylsqjhi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pbbnidox.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bcgcmdof.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2clgcarul.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hnuctkhd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2iqjcdnvr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2krxbblon.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rlejbbvo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vlwxsnks.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tiryxevj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2sqzfdmuq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ueeabmzc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2iiytdtcc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jetpbncq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztswaiar.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vrtpttud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rilaobyp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vnwctebz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ywqbhcyg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xhhnsdtx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hjgxgavi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kafbqjes.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ochdupij.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fmjhkxgx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2otuoyjgd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wecfyijd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fhdzpqte.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2slwszlfh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xlcspeea.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2puhrljwc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xeulsiav.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2sjevyamj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ugmpekfa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zehqwuak.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xzjosgfu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mzqbcyrr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kpfywino.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2baxnavru.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2konseuob.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2reyrhrmm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2aikcypmm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2pfifwirk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rsojswgt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ouyoocjj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jqlpmqrc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ahqwzqlq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2avqubwdk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zvxgadex.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dvyadmjc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2thncvurk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qrijjemm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bwuanlaz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ixkpnzvy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2cbuoslyq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bknapqgm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qpbpjyjn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sdgjqvze.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xxumjpuj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bgnfyoyt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2euzedfhf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nseywhqz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ijihmvik.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2umircadu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lmrclkuv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lomniaco.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uotpkhkn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nsjymgcl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2muvgkqfh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ecserfve.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2sbzcxxns.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2umnfurgl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2tqzhkdtf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rhewtokc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tvzrcbrz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2watsupen.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ndarlcph.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pjupzith.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qngekidn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vpxzinya.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vfqlccjq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2efjgygpq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wbzmcexz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2njtefriy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ejtnxrbl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qodqmnwh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2upbmmzdg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2gciooepq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ypsfwekc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dmgrquhz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2qrmqpspa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pigjwqpy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oxiwoowc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pycxyvjh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2giywzabv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xmhoiabv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sznnnyqd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zdukamsm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bkxdofyu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2witgxgmr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vwktnkfx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iehzczbg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yupvowcm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gehsiyku.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2yunhuznf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wktfzawk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rujjztag.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gubipnet.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cpsuvpeh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2micrrxta.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atzdizpq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fjrudazd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kpovgcmv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ktrgxech.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ebzzjdac.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yrjzewoe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zunvgicq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hsjepxhd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kfufawng.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yvssmslq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2auqmnlla.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rwpkyupn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2oypwvpnw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2juqvbfvv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ihyeauhe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ocyebjem.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2psjoxzix.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qarctsbe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2faltquvt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ldoujzqt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2geosocur.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2edzqwrlf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pwabzwyu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pvsmhcph.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewcbegww.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ueazbtqn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qjxhmgfi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vtiurywa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxrngjx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vyrifszl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yhzrprlx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ovsbkmsm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rdzmigok.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uxcukofk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bphkrchw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yywfhwma.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jdmsxipz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ztlphzma.html


<!-- 参考信息 -->