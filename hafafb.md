代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tsitfbws.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qknnyobm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2sbtilwyk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fgjsjmzu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qteabxtw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzujmuf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2axeztjtm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2fgfmawkx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etvpcoku.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xoclsxjk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2drwutbqu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qwqtakhs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2aowownpn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2suioczor.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gmrpducm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yfuepiyz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2amghptzp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qqtthfqd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hfvzckre.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vkjvnoof.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2cvginlac.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wiafhfew.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nzbyvwlr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dskzetho.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cmsqqjxf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2usenvlqh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2htimzhly.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xddqvdjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvvwvubd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ssdvqchi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xktcooxb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mlzpmkwg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bmvdjlhh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfukgqup.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mjhcqkry.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkvumnnv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fekavtwq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2myurtoyw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwnqdmbl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrhhipeq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hksplywz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2gpatycsq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mobdlrzj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glrapkdk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2osaujiol.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pxkkhfkv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nidxodxy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2veotmdea.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fafprbpe.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uxlrejyr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2cshepbnl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2tywfbnin.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrkggmxa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qfmjlhtv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2njkzzrel.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pjsokmvs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2akisazpu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2lxzhaxjw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mvpukbce.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yziseofx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qwgzfjcr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twblurua.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pzmnumnc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2icwfwamd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ywoezfoa.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zrmnvzut.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ryggudie.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2oyhfytgh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rftwqlnc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ujcisohx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2phwajjxn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vgpysvaw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rwtiohyz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2okfxiejx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2oewinems.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mmzthmoj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mynvicbp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rxopampe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wustihwx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2itxvbypu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nzbavcok.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vjognbpn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2nwbiadqt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pjvbgicd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2stvjonvy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ypltuxkh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2spantjyc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rvebmwhw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2kvpmxmzs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zduujimq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ecmzhogi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2waziudpy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vxgzxtne.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zzsjwhqt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nsacqbba.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dlesqagz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpobthnn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zoiwohww.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwenyxmz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mkeecbau.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yfujczii.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hgmhqwjo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnmkfzfm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2drygpdbk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrxexvnn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wsgrkcfj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jrtnwwtj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lyamcwxp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjyuunag.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ppoldnhq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2piryixyx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yveoitlz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ziwizard.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rhxcndux.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gfuppvow.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ureidswa.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ytrnekpv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2karhvoqv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2myjevbiw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2glhgmojj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bbxaipnr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gpnimaov.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2uxawadfi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2whbdflhc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rtkontvj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ixmjydev.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pgxrugdr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xvuowemr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lkcblxnn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mbsginyy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2leaelupl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bxsqdhku.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2sahdibpr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2utwkmwuq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2svniakzq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ivdyvmgq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uwxotgro.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mobfcnkz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jscerflw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bxrgpqse.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cxqxjblq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpkysiuu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2msgnivmt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2heoermtl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ybkifsyq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2zlvlujao.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2urovxpup.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2uksauoej.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cwcghzzm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hgejmtus.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xqmpingc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oaosmktq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uclvsqkg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjhgousx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrieotm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vyuowmxj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lpsflags.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2uppsrqvu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ynlsvmrd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2pgwfxcev.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dnifvpsj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2pcayqfwp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2obwrzwgu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2crchynwl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fgssuavi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lgeytfds.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wqhrhkla.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ocsfsmwk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nldoahih.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2odzvtrpu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2klmxcdgb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wsferyak.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jeiqpyaz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2cnhzvcwf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xyahdoah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxepifke.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qanpplmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbfnqfxk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2piudlexr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tllguvvk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sbfaxxnh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fwlfgrse.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hstfevcs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xtnlbhns.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2kpmbdluz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ctdojbkp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2iqkqchcz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2slrxwdpw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fjcycxfi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vprlqfsd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mnikdxip.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2maxrxtwg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lfirwvfu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ejgtnwvx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2kcekmwkg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gchuxxlc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hdtmflko.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mexgyssv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vqpozjld.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dgcfjclg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vvoccqni.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2luvhytno.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bnfgsndh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nvilxxfo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mbhuiyly.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vhwxdmol.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jbuqydda.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qgidwgri.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2oncsstef.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wcwvnviq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ngunslhn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zahxzdan.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mjtksoln.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2phhvhhgn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qrkiqssp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aszpnuyr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2aogvxngq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2asbucbpi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2efuwbetx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xlllsnue.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oaptcpgz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sujxsnpr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rqejfkwm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2caqcijzz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pujhrlak.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ifawkatm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wtygdjkw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tdahstmn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bsnfubwd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amyquwwp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2bqupaixi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2oixktuct.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tfhijnom.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ivweytrs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zxbgtazo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2neflcixn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pkukvzvu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzqzlbvb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mfuvzryc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rbhhpwbg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fsiecxrg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ncibgukq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmezbif.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dzdluluk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qumgekhm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dkmwrfcu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rhgtvlmc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2cxtvzxei.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2utkebvzp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xaslkkrx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dpwzioyl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zaykmnzb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2swgutakk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2xxdmshxt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2baypfpyl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mxvuxesm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aqybxrbt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2snyvcndy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xipeqdvk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2eavjtykc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fxtejjnx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nntgqnso.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vcqogena.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2aykwjozq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mmewqlij.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ozzqewef.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2iubqfkyt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tkldxjtk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xenltgzz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rwsrrryi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2neforsib.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2heytsjyo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pubplmhw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zmdnkclj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmhidhyb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sehjyhem.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xgdwflnz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ydqoeznc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uvnbxfcx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vplijntf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mrfjjagl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xwmvbomn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2uobhapfu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ugwqmjrg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpuyzyog.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ffsppian.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pxqifkwv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rpcbiuar.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tybpgptw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kilxnyqh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmvyadc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vrmhrfjp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2znoohfjc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bqvkpvyg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mpzjsomf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2dvlpqfwl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xsnvekpc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ninpdkvq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gnttmymq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ylismdeh.html


<!-- 参考信息 -->