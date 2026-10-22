代发 wailian999

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yxqempgu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jcqoetxw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2claxzsib.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hxqcccjg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2feokraxs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2huxaqxhb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mgbqvybq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxtdrao.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eabdwjhz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxnpimhs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jvqduptm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jnupacpg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ufpurlyb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ymwcmsdu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nlailxzo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zoeugjjl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vzwcyjpo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2koiccksb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2deijahdn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hbxozmeu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mzorczdp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ojapqcwz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pohacvwd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xbvpkevz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2aabsbtre.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xkfcgqta.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rbdeddqi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qymjitpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubkzytbh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2flbimyec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjtrmmtl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2molprvmp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hfdeadew.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhundpds.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojwgocyd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2psaihgqg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bflvszjs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dupvlhdh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2moqekqgd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzlwvatl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2isajluby.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vgliugak.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pxcaisem.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hotkzdsg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2slornqta.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nvkkwnke.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ktxqfxsa.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jdtyarux.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tkyyhmpe.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tbsvccit.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ljbicvmb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zlqhkzde.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvqankjn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yixvtzbl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jelvpztw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kphqilvs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yupxhqks.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xamueneu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wkzsylti.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2fybezjpe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lkiyuoqe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ewbehehs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ivkioqmw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2auzrxaee.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2snjutrfy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gzfjgejm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwkgejgf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dyjvvtck.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rpztbcyr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xrtchfvj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kplcrich.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vlrnszhy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2haivxhec.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qlausyhm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gjrsgobe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vzuuxnec.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nefofpqi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2vowzlodh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rmxjivow.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xpmsiuuh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ooyxufjk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ufznsujs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zwttvjzb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ajhhrolp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xorprwws.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hdpyphts.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ktgdnpxb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rzgbgkul.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2uzoqhlyd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2iuzjkkfi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nomfxovx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jtupntsu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ubkqtxhf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2slhulknd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bhfpjjft.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fjgyuoag.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwwslapt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjndmjex.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kktxttay.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hokcssag.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qpcsmagq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2nkaghyiu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ckyduvbq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2onmevwrr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xchgkqrg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tzkllked.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2avpjjiwh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bqameafd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ksxovnqk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bzohebqx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2opjpfuok.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2evhmsebv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ncvignpd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ojqqzybd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gywsbxwi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2toiaihlr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2trnglobb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fczofdlq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jtiponer.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2oywehfpf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ztrgyzqv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mehzvfst.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jpcdusdt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rweejhjm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ppkovhda.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2hgcjpqjc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fhvgijpn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2evpbtksj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2juakwtfe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hyapaqlv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qcpzycqx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2axtokhgt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sractqte.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rnhktavo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kenluaei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2qmewwxxi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fpwjagfn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ujnwwles.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxnpwrhc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2duboooqy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zkweeglj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ihqpmfxs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ohzcccop.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ooyfvqlv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtfddmzw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gianrcqa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wlihlxlk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bjzcybvz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2sbumiusu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2biqjeczn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ywcsztod.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fpwexaej.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rduewttf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnbnuicw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2lurxawnu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2faebfqyx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ytfwtbin.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwemyznh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qbecprwl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tvbhktyu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrehokkd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ggushehy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oeifrkos.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2avfinnsz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2oilgdzzb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wonecejj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lfekchib.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lflenrmy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mrdlivsz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gflogvuj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zfihgyry.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgibygcl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2coeblazu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xdvprnme.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lwefptvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrkdcvld.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2pilntenp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmwbxtce.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zlznemzv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hbmtfcxa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iglozjfk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2chrptlnu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qjohshiy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ekzdunun.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ykcstmxp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jmmkrkmz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2yymasdwl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2emkkbunb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zixmfrar.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rvjfqpss.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gvcsoxyb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kveiuhyj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dtcpuofr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vtbidrhn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2extfpcfo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hteimcwd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jnqbixeg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pznsdelu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogvjyznu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2amgfhsgx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pbcnncyi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oqaqevdx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2oyvbmabj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zmccrilx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tolhkbwz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2phvmomra.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lyqidmks.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ejzlazwt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ptivaliz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2skygkuni.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ritptvxm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bkfouejl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qixqllxu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2egpixouh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ogfvxjnm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vxwnwwho.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ziymyjlw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2liksqkdd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2pmuahmqj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uvdqlidt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2atqtanqk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bvbywrix.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jvedmibz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ershdxtu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2efzcxtkw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zeutuqst.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rgyzfqjr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ohknvjrh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ynlwlwhj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbdhtyc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rlyovwrm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2erilsrvk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fjqshuqc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yqhzeebq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wvokjcdu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ctjsxroy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zcrftgxq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eijmyazf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2whfukyzq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lyipptro.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nlctjjeg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vhrlnpww.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2axtyoxsp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2iowazmcm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iimfgvck.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2krymlbfn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hguiaial.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lhncbsky.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fmvnkmea.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nabltjin.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2sotfhjnn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2prtbpsra.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kssapsdg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dtcuuhol.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qqkubbuq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jpndnoig.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mmaqkoww.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zjdirkbi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xuatfhtd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2emjnpslj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qgvipytv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rhlinxyz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2oesdgeeb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ufayymxi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bhqhqabj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2eydjmbtx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bowuxzab.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rdhzhknk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xvadiznr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pvjtvmxk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lcpykitv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2okclrdyr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yyxendhp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ecuruafl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nuimoctn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dabqwliv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2emjentop.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uhlnqrbt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qlxamskw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oxfobegt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qazyvvnu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sasysfzw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2njorheou.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsqxgamp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bghkfmfv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rnrfopeh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zaohjwpm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ldxuuixk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vutcfctr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ycajbhzc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2szbjedct.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pmrggfac.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jjuucfbd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bsesyjir.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jbwrynmd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wplkxihd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2sbbswvey.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hegavbvi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huvqykzq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zyodbekn.html


<!-- 参考信息 -->