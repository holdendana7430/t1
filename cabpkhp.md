代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gtvfdljmk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gkwnaerfw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gfbjjrrvh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gcqqxzliv.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/geysjjxuf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/ggewozkqn.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gggtujjqt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gltlwnhcv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gabfcfjiw.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gcdclwcqd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/ggnosfnxa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gmmbkuvja.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/giugrqxfo.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gknkuqscs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gejlrcvzp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/grzguxrst.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gofgjtoou.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gpynfnsmj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gekmeheyw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gfsfkiatb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gnsjauvgm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/govjwtnit.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/galwiaqft.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gianvyzkn.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gjzheztvd.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gtiulmfzi.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gxqgusnek.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gzcfaujyc.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gaslozjre.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/ghcfhjuml.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gwkclyyhx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gemvyyzoh.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gyvfyuunc.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gsjwdevvu.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gbllcrirg.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/grvngawpx.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gcozcswxl.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gjukulrnm.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gdtrptfcl.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/grgrxekoc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggkgricqw.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/glbofuons.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzywfmsqr.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gbgtgzbem.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gnlofayas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gvdrcmyir.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gfmjkmhwv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gxzkphxqq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/garjkrcsl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gmoyhgwlf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gowusmkda.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gdvupfiyc.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gmllashrg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gihcdjryc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gwzobqfqa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gfyenwfiy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gaujfhxpu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gnczarsra.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gkssskpfb.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gvlgszmps.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gahnagusi.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gmnbwfnzz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/golbgxxip.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gcdgeingp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gfzbuigck.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gpchmtzxw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gfmusskng.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gaucxrxdq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gmyvzsoaw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gdtaydyyy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gtjjpnncy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gnmveibgq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gmxyobvei.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gecveddhu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gicnxhwxq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gyjfadimp.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gjtdukesa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyuhyqwjt.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gocmegqgn.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gaczaytjm.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gbsgkwndd.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gopojvliv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gcuyktaud.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/goofmwnfc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gzrevgrcw.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gpisvuoap.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/ghdcwpign.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/ggtjwwwxj.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gxnhyoars.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gvvcancki.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gwfgrmwhy.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gkjsajmtb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gwzwwvmkt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gofyepqxn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gjhaucpkh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gbtbbhkuy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gdfdyclbq.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/glslcrljk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/ggtjamhyo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gutqpnfyg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/grwfewerd.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gwsywsyfg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gntkcqquj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gpweddxkq.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gmxiponzx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gyhxyyjrq.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gomhikswj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/giuullwao.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gajhpvcjw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gfgpkikcg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/giayzktxm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gefmdbvus.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gpnxklpmz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/ggvuuabfw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gtrhwkitc.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gpjvntdrc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gcabsnvkr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gcmjeyxiu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gtmdjdrom.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gkgcrkcid.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gitvldwpu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gvrxxohzy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/ggimgcmoj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gvmfumpwg.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gwbeqiqhe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gmjifsbqm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gzgxkjpev.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gudgdwunc.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gfgygdxrq.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gcxntdumu.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/ggenowmru.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gipfymyry.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gchzwioxl.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/ghhinmvjc.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gcfnqeajm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gtyxbkdpx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gsjujdnsd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gcnsccvkk.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gokwmehqj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gfbxpgpyb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gfzleeshx.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gqduhaozn.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gtmmkclbz.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gthyuwmav.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gpqenambv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/ggsxmlovq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gskzyudlq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gdtsemsrj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/grgodizkh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gtecwqjfq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/ggnnniivp.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gwzkzpntu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/goxksduxn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gzojdttvs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gashnuaur.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqscckoic.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/guhelrigd.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gnijtklwe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gqxosguih.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gkmvfdkxl.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gmvkjciyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/goycsddpy.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gszjppdod.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gqixsfutx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/grhlbwvth.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gtsjjnudl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gpdbkgowj.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/geybstleb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gcajchrmk.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gckrsrwfu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gxoqwtyzf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gdmdpsghd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gyfhaapiq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gspjnykwr.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/ghfrtwzrd.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/grphieook.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/ganlvkgxd.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gihhrtgww.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gndsxwcti.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gppvogrkx.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gguvfwcbc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gwyqmwkyx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/ginnueowp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/grmxxhiaw.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gkkdhnnyb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/ghxekmxmf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gjfgomtih.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsvagoeqy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gurqbmanx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghvsvppwr.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gegwmxhgw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/ghoezclaq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gwmefitpw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gliwiwknc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gxfqqgcjf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gtkhynovw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gdapibrzv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gjzhglohq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gmxzhccaw.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gfzefcvjd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gukrnshth.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gfaxpgvco.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gmattlmkd.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gwbvayqyq.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gcsxtgifq.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gtogyzogs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/grjjodnao.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gizdkgyxy.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gcoyqefob.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/grffagety.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/ggjvhufsc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gamessquj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gvnnnkhai.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gwgvrtjwl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/grzdmjxsf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gmnafuwde.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gqeevzqwh.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gpkitygmi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gvhltmvry.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gaaxwffec.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gogvxpywd.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/glvwcojxo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gnmhhyzdl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gnsjstiqt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/ggkcojjxe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gqmpqwuql.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/glgjgjzbr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/grnztyqhi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gyedpchzs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ghoutpcfe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gjyqpdpit.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gxruucizc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gpunlrfpn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/ghoziaahz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gsxfzurbw.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gtkhtugmm.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gxlpvshxy.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gobtmxsdt.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gdrxzcrvs.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gdqlxdfol.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gzpkmdxtx.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpvipgsbg.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gkyeeuptu.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gxshhhpas.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gvgkiojvt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gcpjnbzlq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/grffrmgsk.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gtyfkcqtc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/glfbsfhfh.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/ghqofwtxu.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/geuaszkdi.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gdsheivvc.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gxpjektdg.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/ganhzuwtt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/glugcweaq.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gtngejfqo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gsyjnpdfi.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/genncjdsd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/ggmogjosc.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gvkdpmlvk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gjjignyow.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/goptfsbev.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gzajfcquz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvmwhlnee.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gprebezdx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gqwshzwuw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gtaldreuo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gpheroyij.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gbquaffqm.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gmhpmekbl.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gljnnhfvr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gzpqgzdiz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gzbaijweq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gnbiubgyn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gkbegvrku.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/glkxorlfi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/guvhwhdbl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gtipgakmf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gixyecjds.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gxxrixgfp.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gvoxpsxsb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/geepmqywr.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gpqixohio.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gltkhgwne.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gnpilsaed.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gnsjcjezv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gypfszvex.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gakynqzze.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/glvvjmgsu.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/glaekbjyh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gqezbyrdz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/ghegtddrx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gejzriehk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghprzjvop.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/govzjiawk.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggtvzutjo.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjlhzfgfo.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gkirdyrbq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gzwrrmjyb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/ggncmhcme.sHtML


<!-- 参考信息 -->