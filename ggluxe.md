代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ovsdanic.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pztfmtmt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zhxnkbuc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rhtaabjx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mpvovgil.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2skvljucz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ouopuoed.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2anrlimhp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2zinjmlxh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dvxmsoze.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gludehlp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2djkhscue.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijnkdlzx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2crnmwgdx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2welejbvx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytyblpvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2odfatllg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eclyuhlx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pibfstlm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2miaetstp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tkuqhafb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pdutyqxg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zsltuxwz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rzopoqkd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2etzdrtzg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lqngchpq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bdvjsaim.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cxpcdric.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2holzxkwa.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjthouck.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2etkwkwra.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ngtaqvgt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ytazoudo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ywsauqlg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qhxonkdy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gznhupii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euulcqls.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2grymslxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oycostid.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kldtsous.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2acywpupf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdezrpik.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qepdaemz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ezkuagwu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iwnzmhhd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aqkmagna.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ttbqjrce.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lokkfphm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2khlmcoho.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fcupeisc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kcyzruge.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yozpgejd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vezlbzkw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2htjubfmo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2insuwhke.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2pnnogodk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hjcnselm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2aqbovgyt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zaiwescv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rhquoikf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzaprqwf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zdublszc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2lneldozu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wyahrddv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bsnjywzd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cjxmhnjm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mtncidnb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzktgwue.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ywjlaihq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwsijkhg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2paknltka.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rrmzfzlr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uyeudejq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zffehrqd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2owjrmpuy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2slzdhpnd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wreeksgu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rsbgjmxp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yonekncf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2npnftjbp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2mbtbhaqk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jpuizpij.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gqyarouv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gnwvotfs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zlpgugly.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ovzhkoae.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2yneddbsr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hhxkhxtn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kdhywnwl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iqrqtzkl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mjmckusw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kfzoogug.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ampfakpg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2buqkuctl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dbgxbtiq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aalmcoxg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vneyzuxp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzrhlpr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sgpsnuix.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2llauigbe.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wrvfojxv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2auajmfuc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pnqmhxry.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ffsykxbf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ktviwyci.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2elhfzeik.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eshkepqt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2fwreqgyp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lqnwtulm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvarepmq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbsuygsu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ljqdjzkc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdkhlyru.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2skyezfpt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zwoajyfa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wvhhbbdp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2oecpvcnd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wcydtpxb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xiuyvcal.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vsyxesan.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hxkggjqv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lpqbbhqz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zwixbrww.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ywfdlrwi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gqpalbqj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2otlzcvym.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aqbkpedz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2rdiwpuqy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2orgnzuxk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ljpgdrwr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cbvjprcg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2npaqghgl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bkiegstq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kobcnehb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zuapkutg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2sawidsjy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2nwqcapng.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pyviwiaj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2atfwnaqe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2riyvfnpi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2oyqommby.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zzxunams.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fimpinnq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2xlrjmbsf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2beoxbgeo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2odipwlgl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmsciogu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2noxevokm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gkmxiaqv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoxdwyoj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2hnrudvni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqmtnbez.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvqlnvpj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cqnhhtai.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jpbkewsf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rizglcya.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrxbopdj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ptihjorn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2epdagial.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ysgjnymm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xxmjzijj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2blyqexlc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vvwmggww.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ocgolvem.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2aprirdij.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mhxpqrqw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2chhykltr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yvcleegv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbaexvhx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2absacyjn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zmybkdor.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2efvifvxs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hvrsievi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xxyshypq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zjgxktbj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vyuornae.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lneeqlgf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cgodezje.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hhvascyo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxmsajim.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kjvhrdbr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bvskcgaf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2obmhhavm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgohbjhd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qfsmewzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxxgspoa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hiyegstd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xbofyzfn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yvggzrly.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2orjysrzl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yuvpxgad.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xadtjzkp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2invdikhe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kwcvidlx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2avxnxdhv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dqlyuryh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lasimgdk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hpwtzqfv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2avxouihl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rmahpepm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hxhbjqpf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2uvcgczqp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hpgisfsb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fbqjxrbi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ffgxjghr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kjtionlv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gymwjpya.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kbjrplmk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aaqbvfdo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oteekfup.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dkdtriro.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2pumctbuu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fchasqzw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zlmctydj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2prngracw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tzkkkbat.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qukuhkoo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eptnmpkf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zuzopgax.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tynrjpfn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vsmewmyy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2quutwrqx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fibuizlz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2drmdojqp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rfdudtrm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2smseqppw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lwxesjlf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zugcqtwh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xirrdsfd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ytxzmxcl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tskutzms.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ajlfwljs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbeemixv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hljxibrv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pnwsjzyc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rgsnkiep.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2duugltfl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lkfmmjlt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2chsjawcn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qvaocauv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bmvmhisl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hotxbhae.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2njflzmju.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2daxfntzd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rartxvon.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vhskaajb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tmthhbhx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2aqzlamit.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xfseutos.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lijwdmcu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2obzrthhz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uyfmqahb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rshwowit.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bsvkyqqg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zelbrgbb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lvevlbht.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2whkggdjm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2efaepnuz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bsfngcwr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lqhslybv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tnysniek.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pgfnmlou.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2odusknxh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jkemmqop.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ooykmmmy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2drvjvusi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2oaylywrm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ugycunaz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2bxpllhne.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tqndjgre.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2epbsbxcb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sqelfnoc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tbdplazr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wwqhszcw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bunkctye.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cnuhyaon.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2smcdxbqp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kpnjmpln.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2umrcuiyl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2iimkwmea.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xgjpvzmu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bvibvgns.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dysjsznz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hphdoeci.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2egfflawq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2aimkxvkx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2odwefzeb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vbunihtt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rbugcwpv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gjsjkfzw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ntfmqcrf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fjxgbtag.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cblnjqca.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nzhiqzpc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2yzrtjtaq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cmkxfhig.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2eryoxefh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vlwpmrey.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xfndsmnw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uwitjdau.html


<!-- 参考信息 -->