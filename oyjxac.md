代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vtpflkax.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ptxdrwqt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zbacupcw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dqbckzqu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jgyocckj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xlhefndq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ohuktmdw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvzmktj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pzrmnmiz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vojuxvus.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3eszjnjvd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wgqkdfge.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3cstfkdtt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qywryjpk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cfbtnkwn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cmssrvzp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tbnmixge.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fpcahpej.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dyjvvffk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pwchshtg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3igogbxow.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwdtulxk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rexbrfvi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pbzadwlo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kezzijcy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3narfecfs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3cnutoctd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xvzwzrfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqlvetvi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ljwcpbyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3powkqbtc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ypteemss.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3okliical.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3urkkbolc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nliowckm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtsiqael.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbqpjjwp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gssvtvft.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bwacncyt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bneqfrqx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zomderun.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3nraglzmn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tcytisuy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiukdfur.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nseosjay.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3tphglcce.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qyahmbea.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3eqiresmh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3recbnvwi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zapotxmr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mfvitngk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lktxeowj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yzocueaa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3apeegxqn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3cilusvpj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mpzbiteg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3nbmpfboe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wvqydfjk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3zkpgkjxg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kkqdrcej.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jsnunajx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xgrdgagl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fapldztc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3jxvciezr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zxvynxdy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fgmjrhux.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zsqcwuun.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ggugedzh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gcnwpybg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bsmjwhae.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3syvyshjw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mieemcei.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ldpojtwv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cwiiycbd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oqqtccvn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hcjwqjpb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hkozdhpo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bhkjaiws.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jbivcjsz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hxyajdqr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hnzpdyow.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sksupimm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mdkmcjsp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ukzmbcwz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yksojbzf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3agfrfzze.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3iwwqbxiw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fjukacgh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pvttczom.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gmwhhezk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xlvdfhef.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gnfbedyu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3oqntqjcc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rlpyazcb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qwovitfd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3iqqyugal.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqqqqkrg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbuvrdkv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugopcovg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dryagvtm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmcfkxrt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fwkuejuu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yhfgikrd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mxloipkn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ntdxitdv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jbziyuql.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3goqvgvig.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uysexkwk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3syvcyazh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3eovgdenk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lmkxisgf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qxomacme.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nbcshrxd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gaiebuuf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ztjyapom.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sigfqyod.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3endvytsl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wndbgpyu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3toqcdqap.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vxgfvlen.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zjhqnuoa.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kocpoizn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3jvohdcnp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hcjyqugw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vgisbeuy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zgfkxhqu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mgxrdsvo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jdwtgwhw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vfmwzsif.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3iqfzimvj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lvhgcgvo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3hppzvurd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fshcizvl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rsthfxwk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3crujjbrd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3eufzeaxc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ctqyaenn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3yfsbvoia.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kpqjjtbn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dgiisuwf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iluwqfzc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bhrhkfow.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3uicnbsib.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fhgnulhe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3esufafhb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mzdvueme.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3uhaplklx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dajcvfwu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fxkovvkd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ecjqdqou.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ngnztkuu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vtihflop.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dfwfgkzd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3muedwhhu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vsexxkxa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eunpktmm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3usxbgkgh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3grfxzwhj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3eqxpslvj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ytgzyadp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3stkwktiw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpawfbaf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rzzbrejx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bejzlkgg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qbziqgra.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3sljbdtwi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3nklfljps.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ahrquqkl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3afetuouf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wstaxoaj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lykqetew.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mtpiltvb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ymcxecim.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3eybpgdqi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhrgzyak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfhbteph.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zkelgtyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flgovxwr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gbbcynpk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3uywcyesf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3oseuqepx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tiaiujff.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pbcnbzio.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3tfobhwpw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3sutolvor.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pzutucja.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3kzqgcjik.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bcrikfby.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3tjdbmlnd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wfgzmzrl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ioeeunfy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vushjcyy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xjrbtpck.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gqrnyxkf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3klkucydx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3eiumrzom.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rjszjcws.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iktvhbxz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ikcpqslm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ukphosdw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3udkdwerj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rwtookdn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3sienrqyv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3najxivvo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3twcjqgvr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qaedgftg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dkwtqsof.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qpzgwatt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jjnjykrz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3pqbtumkg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pmjgihtw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vsxobmnh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xjsuytvx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jeirrqce.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mewznsdp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yorhemix.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oqnvihry.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bbtjedvt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ogopcfls.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ootkjbft.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fpswpirp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3huuebhnv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3thtoxwhs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mzakhujl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sauatdpe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3trugxxfd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3khhqfcqh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qpabjyln.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gljjdjrg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ssmhxslc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yfdjbwsz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3cjxuyxyc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jvsrvcbg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qhouddrr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mcjnfnmj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lrprnuyf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ajmehtys.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hyqkcqso.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zgtbxdpj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3levrwbdu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nmhdcsff.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zblvilan.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3cuhgyasg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3giwgnbxw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vgsyobcg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3pdztbltp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sqezpmrs.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gxzprtcv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oimjhzkt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxoqgaoe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mnxgobrm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sehjvxwe.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3avqcpiqm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gvnllvqw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wremrplz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3twhxgqdm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3libpapmj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vvpkmqab.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hibxgbsx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ntynupzl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3atgapyms.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ebembqtn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fhcbvutr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kxyscyft.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hspvgoko.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xumfaufg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3aczkxnbc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ifkoeuqw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kkcocfpy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dmbqtxqh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rwrgziip.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3njvqlobk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ivkqlbfi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vwumvucx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3egtrlomj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ahbercxa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qmxegpav.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rbimwbbw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bszhtnto.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3voxazhgn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vbnxuqum.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mvejvwqc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uniuskrl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfdbwto.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lavylbfv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zrhzzmae.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nmyqzjsl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3crpnsxax.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mmfharou.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tuwzrbct.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbgvqgj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlvkahxj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mowspgbe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jppsoavq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rjrmakhp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3srhoxgvr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3idxtssqg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tuwkexrq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkciggg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zukqoxfz.html


<!-- 参考信息 -->