代发 wailian999

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fhokffmv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2olwlnabq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nybxdrxd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2orkycmzx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hbeujymj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rvcppjit.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tnuqqgnk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2cltworah.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2fgdgzmbm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zlgrwaat.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2efzflqai.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ziqdsbfa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezeseqkq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pyzlxctj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ctklydks.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2somybrvv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zynwmgct.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsycwsgp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2cnfiwfbx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kmnlatqf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rmamqfov.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yiluwxsf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zoagwxzm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hqpkjxlk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpzovavv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xasowygz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lfsbesgz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lvplctib.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hgbcznoh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fxywjrft.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xgneqgti.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2frxfswzt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bjvocdnv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tifhrpht.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xbawjqee.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nvuvqazl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whypkqhr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2cxnhlyfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iclfueni.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmpijhyd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jooihchz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lsjsqttz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuslxmvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xqathhyv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yovmfqvm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2husnpjvf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkpisylo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dslurbht.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pfelumnf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2assfpskw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2igcouhhr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ceczhtzz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hbcvelfq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2efrucjbk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymywqtad.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qytkmpwh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fcxxqzei.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2arrcsqyp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bdxzaefa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sccqwsmh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lsqwglzs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgppqmde.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qgivesan.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cnxweroc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xisdmhsw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2uuyrecww.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qgixldjz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gmvwixbi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxqdcbac.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lnrlgkak.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dutknaqy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xymdjxbt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xccrtnjl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rtmsxizt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfdmoyyr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2syfvodfj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ahkzokkw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wbbchxrn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gyesnobp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tkaxmmxy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bryajsoy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2klelkisi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nggwrpoj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2imhttpnj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iivhqoxo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zidhfqhp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tepgnthn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zkwlhgec.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rxxglvrw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ncqjngpl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2senbywjf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fcdrrmkn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxxqukuo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kmjwwlgj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zlrlmtea.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hkwcncdi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2iofrqbha.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2juskewhe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hhdfesgh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2loqstyvb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2oowsixpx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lufpxmde.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nsrxdnvy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zgwtmsme.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xzzaxiae.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bjwidecu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkbuhber.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ondnbwvi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2saymyski.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2udbvleez.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ejxuyyhn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kaxqxnqo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bqjoydwn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nyhmcteg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hsqzoxhl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mvtvifnx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vupmmfht.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jpskdkkb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2njzgknkr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2srqkkyvd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2siugokgv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bkfinshx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2myuaridl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2waykrhrn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kinwgfkh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sbpnurgc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2khfiwhno.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vhvlkmyt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qnwffaxt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2muqulypq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kwuhhpvq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gmvlocft.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2grkhvgsg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2yazftotw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2bjqpywnf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ignzvuxd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2uolzvykw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2csorsfiw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qfjgbmjt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kpmyhwki.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ydpxdkjw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sykkdvpf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jgrdxxvy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wqscsmze.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zbpcurex.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ijtpovei.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qfnugdxv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2usldlocl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hcsodlfh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nrzfqrkc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xmlspeks.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bnbtwspb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ytcdchyu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mjhnimsa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ekoohlya.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2qbziqeha.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdbuyebc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ykqirqeg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ahngtsfu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yfkfwfru.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpednkdi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjdwvakz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2geyihbox.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vroepdxj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ajbmopyw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kltlbsdr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2voiwhplc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lxihjain.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nuhjphkf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2peljisay.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vfqlsynp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qatgyaxp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hxoaavvc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mbzmcujh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zvjnnknc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xalesnob.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wrgbgzvn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ibaifcos.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bmlplpwh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dclznrxw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dpfxzmen.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wikmtuug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pczgxclv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmzvywak.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2untbvfle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2geimvxng.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mrxbiiqp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vyiutast.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wsnhtpuc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kglwlqrg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pwoiktdm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vakqzdmc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bhvmyrkk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fgpzvrqp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mqjzwujn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2kexmaxij.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xoxoqvct.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jmgjtzsn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cqmmvmso.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gyfbagdl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2biwbmdfk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ehvndacl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2cjdagveg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lhghzptx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hzddikad.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cwdiyyjt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mrnyzpkr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jvhcexxb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wcomriky.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fipkrwdh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zaebmxbv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2iudmhrvr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gypxcfpa.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2onsfnwjt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2oycelnbx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2flwxijct.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2glkamezm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2okxfefiv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2svpdatvi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lcbrpptw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jgabpcgb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmxevfvk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qjybcfxa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pwdqztgu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ruaeswou.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2odpxpulb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xgpcpjgy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2awyxulyi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2meqkdciy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xfhemqrl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fssqxsco.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2frdpllvz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gyhjmmsk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gzcqjggc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lsvfbxjs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tzqijtom.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2izsiupal.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jhnuzoym.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zfhwfidu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nvnlreuf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2rtjynhag.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pwjqdhaa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fkpvxuyt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nazrjvli.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qygonfrk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2djioifzb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2flrmnnkn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hmwhyqix.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2txofajff.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dyowobqb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2elhusagm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2iqpzanlx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dlscitxa.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2whnctezb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nhfynjew.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2axeyjpqq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wwaifcct.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvttbgrg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2likdmviy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ccjecpuf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mvdlbiah.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hmtnjlhu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2bhexuoss.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tkbgnivf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zdmvezoa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hbfohlyb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2isipfvrc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2oawgsstv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sqncbhle.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xjevbzzf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ndmiewnl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mizxipzy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qizbnysx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ynqtrgwz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qqdxfxea.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uaziffbi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hgilowgu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2alollusb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uvszhsbs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xflqjsof.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jagysfgm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lqtaiifk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dkdhomhr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xgejdroo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gfvmzauz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qnpteqoc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fsxelfhk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tkvwrlre.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ndvhhbgb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wotwmwoc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2suizvgxq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2acsnsmrc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwsjdthi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rwfrobxe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ihlusujz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oobreyym.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cnrgbhel.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aguxaten.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iodtysao.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bckrcmil.html


<!-- 参考信息 -->