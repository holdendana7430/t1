代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kiagmaer.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggkxtmgy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kocdfupm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xxipngss.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rpukjwnr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhahrlsr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hbmuhzaq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bljovpct.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wglrdwfq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2imqnzawi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uavbjcxl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fmygpvaq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mxbahzqv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zwqzuuvp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ybpjwsms.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ckgvflyw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2iufhveom.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2biifyfcy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2efwqhzdn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hbttzclb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tmdjkimz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2uphcsrtf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2anammeia.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zinpbnah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmqtqpur.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ulqunzkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeldqgks.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2crjupvod.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zmjeksrw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lfkvjalc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2toiequza.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sthmgrew.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjiotsgd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xbrfhyai.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2cuverfat.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtxxjsmg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2lfcdawbm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cxpihmif.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwmnleih.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ktrymblc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qfrqekcw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qvqkfcar.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2myxfafkw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2krgoevjv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2idedcnxb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kwggizch.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2iwbovnqi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ynetkedg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2acnojyzn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dampaqhw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kgvrcgjc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2yfcaegmq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2dpmvialh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2sldzwffq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2iqhuurdf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ahtxmhak.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2iujuxdzy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kswomgts.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vbjdktgr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2gmjwmohi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bngmphky.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzebrbnn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zkyxcjvt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wmftjycn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2prrfcekg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nmmdpsqh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ybxupjql.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pxczfukw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2izkybsqk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gpsqaacd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vxukusob.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2yymuhtws.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jvdqvvyu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rkejkmtc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vsjfeobn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2aqpazezd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2khzunbwp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ezwhnxru.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mwkoxzue.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzwqxez.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zrtvrsmv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ypngofcz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pjpcvfdl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nqfvqjti.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hgmhuhyr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fxpztuyc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hythuiec.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hhxotnfl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2etuexjzn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2uzqbjvyn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2plkakcqn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sxbnzenv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtyplzyh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2czseomyp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hsuqzvom.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dhtrrsfc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ylvmzjvv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2aeegjyfn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wbrsavco.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2guwerpgl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jervgmof.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2crtwrufq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aghsawee.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wihdpmym.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofctqexw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cxmbdwya.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2btzvehoi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aqbpalkb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mdxamqnj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ziiqfkcr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ekhyxgwu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wapmlhlg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lyjwonqi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2arwtsohy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xofvfnet.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mrkalcfz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2twhzyahw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qbblfxcb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2odtsfzfm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2vmrbgnfn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2glbtkhyq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lkevpqyl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2yubircyc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2eksmamla.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xbyanwnn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lwnnjqnt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ujmdghuz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2epaetmrj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ouevxhtj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yekjavtx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jibhaqqk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xyoqwyyl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ezhsueke.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2wnwkhkro.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vvskwded.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zheeiuxy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dbqsrnlz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lsvmkzne.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2cflepdyr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qitxbgjg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wvjezwpb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pbbjrjop.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yjeiekmp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2fnsiinqn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2fkotjuuh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wnljtxsw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cuibruvz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cegbbkib.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rsxrjsru.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2czjrjzjf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jecegfxg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wgfqguil.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ghtwuwyk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2eghpmsoj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dhfvpuns.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ghzpjvhr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gztdpigt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptwtiisv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cgqjqrxx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uaiwybbw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ucjlrvuu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wodaqoqf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uacbqyzg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dhpfyvev.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2njtinhpl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lbrptjqj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kxjsazyi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2medutpob.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2leoqnrbk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ofdmbdgf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2eygqamyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grhuqtcj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2iffjlyhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpjxrsbc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nsxpgoke.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ljphdiym.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xsubslxy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zxumopcr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qtdmifcq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2krispyws.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2lrshwjib.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bpynfrmo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zcomjgqq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2eokgzwql.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fmxgmrqr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ubtrgmbi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pacixafh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bguiwnuv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hsezpyuk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2irxrbmqz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2efouzayq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yxvnjfsz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xeczigaf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oftmnfnl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sltnzmxi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2obekkixi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yeglpucy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vfbvtbvl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2beedvrmk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dmyqeluf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jxwbmwbs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ydpacclq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2esmmbzds.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xowmtsvt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xggtzkym.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mklsclpi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rhurjqem.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhkytew.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqrhibtt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fqghzdrf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2flupmqbu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2anvwqmys.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rafuvwno.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dbfngjph.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2eednxwsm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2pposbtah.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2edfnarys.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dazpcvwu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dltrtvhf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2olxdteyk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xliwellr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oeravuuy.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jlltzcur.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jngethyt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zqelqoze.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wjatqmwh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ykmwubbv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jvmqqkiq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mnltjrdp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uxeodkad.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jabdtxya.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yxatdldp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2abnwfynx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gpjtnbfr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xahxcqya.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bsbhzsew.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2soitqpbv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2bowhtpcf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kbdaeuaz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qjrbofot.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jfpggmqv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fkakisqu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jwxiiscr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2igabhsgg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gkxmqwcz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kyclywka.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2chnntvnm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rlwxiyur.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2cnmbvotq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tjgdiveq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ickwkxqn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jkpnrkzr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eapsrigx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ibdvfnkt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2sjhwjxwj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rkqfqvpt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qrztzidq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uckaponx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tkulxgyv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ltueotjo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hcwuzcsp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rjrhlnwd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rpqsjctm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ybyjqfpe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2uggpydes.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2szvbxtcn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2plabcyog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pjwciwar.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yehkaoee.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nkjzeofp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mlnoibks.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qdcgdfxk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jfrwleid.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hhdypytn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ppezsbrf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mhfjrkjg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sotwtzoy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gczwuleb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2endxepdr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyqqzjze.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uwmztlht.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2liojiset.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2userggir.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ukjvicux.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2abpagedk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dqzlyqnp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tzmcjgui.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gjuvpmpq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hgwxiojk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2llgcjpuo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pmqpvnxt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2dijqxkab.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2tuoaifyw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rwmxsllr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpuhccvi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rkiqjvxn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2owmsxstk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vvzlkotm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vqymhgrz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2olafdnoa.html


<!-- 参考信息 -->