代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dybsszlv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mhbjjflb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2dohykkaf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rexitvkz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2isnaxuyy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfujyacr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pnrdcksf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2azfndenb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2clgrmqqm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmlnfpci.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yatorior.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2yvodmznt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jbqbkwyo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mvenejoh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2abzwqalb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cvsrlqze.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kuasgjrw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zmcfjdvu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uvbzbltm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rnroruoq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2aqzbkysr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2otglazll.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wtataxtr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yzgfgcxr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fjiyjbiu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2mnydbewx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2abovkcvg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2akoqzcbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecxxciiu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2phvzkosb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hscxfxdw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2prvwujdg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2offqdaxm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kickimyp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2amtlxkay.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kesoohsr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxauznme.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pjdapqnz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqrjooqg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhhhyuls.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sulresdl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wbuolwqf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnfkbfkj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fpdzttlo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hjbwskrq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2unjqtnyj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2sgfhaivn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2biimiejr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2krdozvzc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pitmlzrk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bufdkqvk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgxxzqtj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdxqhjbo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tweljskt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2prkkfzmb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zbhnptnb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2mddwugwj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2sjwxpzzg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2nscclroh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2tqzghucu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fkvtqzsj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nmibwrkt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tdbqzigq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rmoklylo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nncqrxkx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zwdhupex.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qnkvibss.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fjktqatz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ahhuamaj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gentbrjc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fnutzyvu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2txaerkva.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nynfwlaj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dolobwji.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2akaenkfm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qvxygvgo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2uygldujl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2svgqtnne.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rgjlbpsd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qxqcyggr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eahmxzjm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2riarkrme.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vedegiwk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2yrxfvmbh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vxelbwti.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ekiiyrhu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2aptasdaq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ooodzzet.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hbmxnwgh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2xznejtfw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2knjualir.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gudwlfdl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fuuorkdv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2omxxwsir.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2whsocazm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sjytgevo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2sugibghn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhqbmvje.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wssmtrfx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jzcmuiwn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xwrfstxv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2axatmbda.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzimugtw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vjkjsoil.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2shkrufkd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2iankzhlh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dmqcocci.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2brboejrn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2airwsdrf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dvgicegn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aavjkngf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zdswdbhq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2rlxfpoiu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bxyhxbwg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rhzqwvua.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uubgzcoc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2aonwnsra.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kitvkdox.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gcdmfunt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2lcjhrwia.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vgctzjgs.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2slonrwiw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xuywisnj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2kjpduaqj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2oezxcqvd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bjlrymmc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yimlutan.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2nqfmcmrt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zjbwzxis.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kdymgxno.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2sfvwybjd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xqizzbeh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oieojfqp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rdkisjmd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hvedkxjb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fpleqgil.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mktrrrme.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2igaskbrx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bpuuhpph.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zupodgaw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dzvyorqo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uxvcdepl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vtaabyxn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rrmikpry.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2woixxbeb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ipuwpfni.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rwsmmxed.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pvangjbo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmoslkvs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jyqlhpgc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2miofifid.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zodfhxey.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2yzvtypnm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqreelqw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2woxxyoep.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rjybcdcr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2shytzhpd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2lrdzucsw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nlmkjgnv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fvecubwd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohqqhnaa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvuukoid.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ssfuxrod.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ikwjtqbg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2aiemsvkt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rsppqvky.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mocqndwx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2olimqcus.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ioubcmcg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ualtwyiv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2omwmoonv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtzlvryl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gctiqcrk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2segyrnne.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2uapxkhqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azhsuclg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2lhcpgpkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oexkoetj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2whojmxdc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hhfeglmp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xisfwkxt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xcqmymxw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zfzawtnp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gpguukom.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ouvwsddw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2nmlpwwyr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zeoeonxw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2gcocqkkx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lrafsjvc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nledbeoq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2guxmsqup.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2muhtukmh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fldedqpv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wzyftnyy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxfrayd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ygadsjqy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jdahfgec.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2orkaxksn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vpjkwagb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2tjbugboo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wlcolujo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ziarjqco.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2etmnhwxv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uepncpql.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vmibsijz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vqddgkhj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zblrmgfr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zyduraoz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ncavybii.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2grbkctjk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xougzzbj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgxaufs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ngnmnzwu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2iicyqico.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2sdtzaiyx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fqkibkpu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wtkfnldf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2krtqihce.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wdlvoryy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dhkrlbvw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uiethowe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zgucbwfe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tpmxwcru.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ahoqfznl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgdhrihi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpgqfvyn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bariates.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2prtnncai.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mcgtnxks.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sohodhaf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hjgplfpy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wbbowttb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2eestalcx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2jzuvwdbg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2aarvegrm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mippvgit.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aiawqial.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uonvdqdp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pvysiwdp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2aszscnwa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yatyhcju.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yagbofff.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2herhamid.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2unpqsdnd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vyrgbjnc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ffhknooc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ubnjhugi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2itwughzz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zpsbomif.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dyxarzew.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2yqcbialv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rzttogtw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jmdsuhdl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dqzfuovc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2aajbcijk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jsynsmkn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqxrrjra.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mlhvhhsi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2furonhre.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lievswmy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2onqzxhhn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qjjchnfi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kxkxjrhm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cijyhpdd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2owhumzbe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cqyxbpqn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2smytohls.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xgvfdnql.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cegbytqc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2akjownqa.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2fwwxlpvt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2flysywtp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gcjqtnaf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2voetkwhp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2iieicdzf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2eidolhvb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qvyleivz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tlevftwr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2oetwuays.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jcnggypx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oaxzfcdw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzofzco.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2smefkfox.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dvhpnwzl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2imbynqfs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ujgjvbxs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zmhzbgfy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qkvoyfza.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mvqdqwzn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cscmnrmk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nsepcaqs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxgjuttc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2zedbbela.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ooikafpd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rfixcuhs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2cpimihtu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rsfddxso.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hermoohh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtddobog.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekewfsdq.html


<!-- 参考信息 -->