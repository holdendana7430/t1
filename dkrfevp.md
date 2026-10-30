代发 wailian999

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gaeqkesnc.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gcocvhrtu.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gvjmsmmge.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gchgjfvmy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzqbrcos.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gcdsgfext.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gvbfryfzt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gqcytjgir.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gzaqqsfxw.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gfhfgmogr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gqnoxpglc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gsgnlukvi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gsaiyhrni.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfgydmgz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gtradzywt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gwdesicii.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gyoxcozro.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gzpyracqz.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gddqwexhn.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/grznidwqt.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gzaqujpqk.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggbaeuzhd.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbreqqfur.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gbnmzpxnr.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gjipdztsz.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gjljiztme.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gtjoinxqg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gpmgjnyay.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gquputfdp.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gqpttvtud.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gipscwxhg.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gomupybfb.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gqhgaisps.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gkoubznlp.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/grxgegpka.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/ggtmlluph.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grthoauon.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gvounqcyp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjlwkasrh.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gogrbncjs.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gatufyulq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gaxpxrsmm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gbbqvdaqa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzxhypkzp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gfmuvnpaw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/ghnsiidvk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gflvvkyil.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gbsqvtfxb.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gtgukyhbr.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gqqljpplk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gkhmwaajk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gkzhclopk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/glfmoycbk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gevshwnkx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gwqnmppjs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gnpilgdqp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gfgdsqgdk.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gmwkyqhhx.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gbkukbfmx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gcpblilsn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gjmukckvc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gosojvypo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gvcexdprn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/galepsnoi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gkwxqgync.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/ggbpuxvci.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gsfpjnigx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gxyvyglsq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gqhwgvyjl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfmkzmfku.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/glstcxsmn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/galuyonit.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gobtxfafh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzainpvkq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gkriavycc.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gmnxdkccl.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/giecpfdqd.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gnjmxklfi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gdyxwjzub.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gtebpkzlz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gpmdjlwpu.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gdeairctz.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gyvkbgynq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gwgmpojou.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gygruqrgb.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gygkfttah.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/ggkdjbasx.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gtdvjlayl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/grukshjac.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gqbvuvelv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/givtqpiip.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gjngclbam.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gvxeghquo.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/grljhuksa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gmywbjvcb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gtpsnziav.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gqfhdyzwp.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gjxeppsdo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gqqboyhji.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/grhestiiw.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/guoyazpnp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gaznokpyl.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gwqjcgzto.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gpzryylxm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gdnykdybn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gdpsjbqre.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/ggugagypb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/giasggene.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/glaaepkde.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gbshsmqhr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gvtjrrawc.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gbubajukv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gqsxuuqif.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gssymojtu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gmbkfetwd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gaiytqqxt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gthlokrjo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gfkkiypkt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gjrkynbce.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gleermyst.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/giwmtcbof.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gngjrkiiu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/grfjnnbdy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gefohdjss.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gasuwbnsc.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gwjdjqmpi.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gaknfzlxl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gogozrvfq.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/grtgctltv.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gklhvengc.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gfcjuzynv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gvtkwegpl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gbbhcezlh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gaqumfzym.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gbnewrepx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gzkuhqzgp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/goicbsoum.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gdmaizimc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gzztjclce.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gaekjszim.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gaylbjtlm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gqmbsnzwr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gvkuyqyzx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gfzuumjgq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/grcawytxn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/grszzpzar.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gzzkldpzz.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gojaoautc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gumuvalai.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gipbcwhgs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gdauqijoq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gwwywpeou.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/grrkqyeru.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gqbgbueku.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gbxxypyvt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gueuccdko.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gbnfguyzq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gnbfxtwuc.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gskhzaxvq.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gsxyqtkkt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gxipmcukd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gnxxzdpwf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gidcrqymz.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/ggvkxyrxo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gltkxyody.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gbbarwpjv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/geimztxfm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gfnnmngxb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/genhazphc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmxfsfywl.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gtzxoeuto.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gxkvgxnlo.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gqhbypaei.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gmufqtarg.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/glnqzfzqg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gcrpcrdoz.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gyghjhfei.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gmsxqkyfw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gnejiblua.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gemwiycpt.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gbmqjblqc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/godsfxocl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/ginqwacxk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ginrkxusn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gxxwozsjm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwxcegvpv.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gbdswhnii.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gunirdrly.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/ghyqvdhql.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gkmovdcjc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/ggkwhbpav.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gmlobveac.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/ggaqgfxjz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gydpcmmxj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gquugpven.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gsfnhidiu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gnqlcgelc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gvoxjqdqj.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/ghuxayinf.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gzgvtwzcv.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gbltpefwy.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gccuktzjq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gjfvibqzh.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gfzprvano.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gheebzcfa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjlrhzzvo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/ggsjadbru.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/ggcvjyfzd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gikacejux.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gnwauvcmv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gpgxdmzkz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gyuvkhxke.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gtxgxmhaq.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gcavdciga.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gduxzvurt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gqddsdzeo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gndfkfkty.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gpozibobh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gtdypsjuu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gujfmlpte.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gduzrivzx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gmdhepbtb.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gdqfwzvck.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/geijjmfwp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gdwkvxpfh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gmlasppxp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/ghaiitadu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gbpauiyur.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gtxabpnsa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gzbrkyfqa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gzowfaiqv.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gmbnnzrqp.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcabsveyc.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/goosvnsmv.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gppgcgrsp.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/ghcuxytnl.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/ggqchntxe.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glndpmtby.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/glprbgxgg.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/glugglrth.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/giyabnmdd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gqpbzywjg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gbqlzycep.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gpvldfgnz.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqirrkulm.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gjhzbzzuo.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gtgvssbzc.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gxsozehge.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gtftwlzxb.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/ggjsfhgbu.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/ghcxjkvgf.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gedpsvywf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gvxusczvq.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/ghjiimzdk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfojsdfym.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gupqvvkpa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gmztoprbf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfcslsp.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gmcaiedwc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gtbihyyak.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gvrajthsa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gdojibtha.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gulgtinyx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gnnzfaqjx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/goaeozmqd.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gqqxdegel.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gesmtdyrc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gmlzwpcvn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gqxsetatl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ggwnyxguu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gqhrmztdf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gnispgzbx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gycjzchia.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gqliufcqh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/geipjzasg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gqfltvvtl.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gmqrflkuh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gpwwpjfcq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcmazxdqh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gldisdtvj.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gqffjzqfs.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gwzvfcpjd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gwkzgupej.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghjfgeled.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/geusvpnim.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gghzluzmk.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gyyycrbce.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/grxsvzjzy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gukmqumcv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/grmpqtjnv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/giqvloxec.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gpzvulqzm.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gxzcsnmsx.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gcfstwsvv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gycbuejjt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjwxjikbq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpqgtxdxl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gpkxzlsfz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gontuuxob.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzlaxjjmj.sHtML


<!-- 参考信息 -->