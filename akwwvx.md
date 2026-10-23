代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovdsbxip.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yqtefqws.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qbyjdrgb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3waqzhjgm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qtuwrpxo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cvulbbia.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3orruajui.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mocrnyld.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nznuxpig.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qvdtpvwe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3efopfboe.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gzgvzryo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3naptdyln.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vljmlucn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hzuqcjkt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3uqqsiybl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qqxzjwpz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ntikvwbw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3skcjnioo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dujfdtgv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mylrvqoh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nrripltl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qyjygnml.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kaxvhesf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3clpiicbe.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3diwzrmmx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ifnjrdmf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cnxhsqot.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tqgziusd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kmxnaeej.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bxcnfaev.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3whbgluso.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3mxfnamus.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtsfqlcp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bxmtofkg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3afpyviak.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uotfgaan.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nnxupqqi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3yrboccbc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dipybdyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oifumjdi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3eubcsfud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mshfuutr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uszhqmoj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3annlyvgn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdzojkcg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdgbtrrb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqeiose.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nliekvtx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uyylotra.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vzsxreuh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3epggdppq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqgpsccw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3dovyzzkt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3peenaffd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yekfufdw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wopfrpuo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dfidboqf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptbuxpzs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3znnwcors.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3tuxfxdhg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgriqruy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vujdyabm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqtfphud.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywfsebhq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3runonczx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ervlkbki.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3stqxsier.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hpwuknsj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ldxukifw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejadjfli.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zvkwxear.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ewwzwate.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enkoxgba.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fmstaocy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3tsjgkvob.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qrpfxyss.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sylynoms.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qznokxcp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cfcurwmp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rkzvktnh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yekqdvbd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ytybwaom.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3byepiihr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3tbvagelc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ttaqudto.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lgowgoui.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mrgjbfyz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3uruwdnvr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tcundaha.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qbmlvbau.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fvqxpuld.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3muuoadfj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3koivlzoh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tsugvdbi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wzgxstuv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sssbnfsa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sfbmyoot.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3jvjamhhi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iosfcgsj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ifhyoatj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hjsafvhu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzyardxe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3euabvtxp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fmrracnt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3imygbukj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xwbjowrd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3aulswrmi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3afrnwqaq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzkcgpig.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wxxggjgt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3aamkzpad.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ejofhhjm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jdfvaijv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gzexcoht.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3knewotsd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rdfddifb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3enwprnbd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3shyidspp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bovithgr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3whiltqrj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3teqwardp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pguwefug.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pkrgyjot.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oubpijow.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zvbcgcfe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3jgigahvg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pmnjqkif.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fcdxiykp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nzgrwvbl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rwscpfsu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rrrtmvqi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ipdkexgv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uucebuvc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wjbzzrkq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3aqrfbkqh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fzsednvv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ufrqlszc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kyoarhcx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wrnnwcag.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gkmqgvew.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ihaeegov.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ckasdqcy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3eyrowuon.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wmtdwwmd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rwfciojq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3esauqyvw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tglnxvtm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zuuxulps.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xbstqrri.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgbqokkd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xamwjwvi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3foegdjvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lzppseyy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3urnhrxjr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3niccngod.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbezkerb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uuwjhsqq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lycuclql.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3cfybzkwj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3tgduwglh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3grqzugsv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kbastnjf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qdnanchy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqxqtcid.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3aisulzmh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3tcvcnhcp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rggafspr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qwheggbe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ayqscfvq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pmdocgju.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ggtqrpxg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dktyvbqy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rljxkzyk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ngzahyat.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3isibmgjp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3lyaqyxdf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uzvppzzz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3gklgjfvd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mbnzkusc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qnvkgvek.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tffpskrb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jngricou.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdmscnqk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tbnvribx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivsxggxw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3codznjyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhvaxedc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3oeagqygd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spfojhnj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3emujpkdx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vgfksrrt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zeexbdmg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3enakrduh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3imvorlls.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3siqbwhnb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hhyzbkdz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ytjydyoe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3etyhzotv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3wjzjtehz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ahlscumk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zhuorrbb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3idbzjhpa.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tlbsqipa.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xfxyhnkl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sofovskv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ztnjmpqd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wyoqrxhk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rgbzygnp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jaeanhjj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ucsxvejq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pygzllwi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dkmkifvz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wisvxfip.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pfvhfgir.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hxbtrxop.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xjznpfwd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3flutifer.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfskzikf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfhbctxa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3byjgmiki.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tjmdcjdv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3thiihnty.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3onasypqm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nsndlicp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rkypccji.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qiyixybn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3juewurlm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hsbtzuld.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wdhuwvip.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zvzeyxid.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jjsljyzk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tvcvzgft.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nfglvkuz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jtgrjqif.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3weexadcp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ejuohlqt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cyrtcqii.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3elsesnge.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3beucunpb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wnvrtial.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qobpsvwz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zajzgomd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gssgzwdt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ozbovmeg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3aurrkwat.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qsxghiyk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sahrrxec.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwfvslsx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wadiptus.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mjkuwbhl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dmevijzc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zmklpyyr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3eiewpqik.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qixunajd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jskfvkpn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3asbpxzbx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xivryjeh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pkrlmsgn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3glutklyg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wqslijyf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vorfbagm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3idrudykv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xxgfvyzs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vmvphteg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dnrvkplr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3grgsmnvp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hbwnngwo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snygopnh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dvlrrqyv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3asmweaol.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qkysmoqq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ofmjsrlm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zclcizgs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mnpoxaax.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yohdejsb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ibkhdlpw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qclygwhq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gscejsxv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3btrwivui.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3izkwjzgx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jbytikwa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jmxtcatc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dcjtjgok.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xglxjhej.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vtjgmppu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pjgdiyac.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3htjcgwpc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dftpbgim.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ufpecjcb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bzejipqj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bwucgvvt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fqulrfdz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vghxkymv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3igxqaisp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jvqmbhph.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rgxfdzqy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3chobdwev.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3msysqewc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lcoanjpx.html


<!-- 参考信息 -->