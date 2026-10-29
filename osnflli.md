代发 wailian999

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gsgbsuctj.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gyyksujyq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/girjraxhz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gburxijgi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghdfhykld.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/ghfszpkdz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gefvzeddv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmitmuixb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gtpcyvdpz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gasdvlpqa.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gkdjakhth.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gshmobybq.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gooidkrew.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gasbzmzqv.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ggffqkxjb.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gjeufritt.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gdwrbcyfh.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gxgjddeqn.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gpynoxazg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/grkshuvcy.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/ggopgppuz.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gxluqiviz.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gvffhbnud.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gnrgmvupg.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gedmzcumo.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gtaiqfela.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gjgpylbtu.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gigwvlfzq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gstugpcje.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gpkyuxdng.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwmcvpjaw.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gcodqntte.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gcdtxplur.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gmoxfpvkw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gcikbvzbr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gejghnfch.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gulwmomzd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gomawvkfg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gfwytzqgl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gdvliqfra.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/grzoijpke.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gmbengmmw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gacclgxul.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gqlwxhvdn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gnjxxfril.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gabapelqp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gtyraauqw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gevgwczqd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/grutvijxa.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gfhliiccf.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/ghwxbllzc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gltudlyos.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/glgpwjxld.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gvhqjjqzu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/giaytlycz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/glkptubci.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gmgkkfepl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/grwlxdvrl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gabslkzxf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gdfrurvzx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gaqezlkra.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfehjrmvo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gbbvgkztb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gbwbuixfd.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gouhowzyb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gfpbtfetv.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gullmqpvu.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gpoewrzvv.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gikuirhvp.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gfxzmeeua.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gfveqxbow.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gdoqspoxq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gmtfoexjy.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/grpojxyqk.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/ghbgqffdb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gulvjmnub.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gfdvtydce.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gypbcuixg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gqmzcstbg.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gdandslbq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/glmodwocu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ghquuznjg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gwzktyrzt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gewjspetj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gcemyzqnx.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gsqctehcu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gwauafgto.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/grsiqbqvj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gkugejhcz.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gpcbbpdfc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gnrimziot.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/ghtbnjikw.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/ghafiuikq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gmyuozysc.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gjlbeqcfy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/ggweqojqd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gaymtzeoh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gfzltkyqg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gzgvvmcdi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gscwhoflx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gxslzrfwp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gznbmarlt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gozyneole.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/grqapypgr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gtevlsnxn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gchlsglbn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gyfxqwsqt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gtgadigfy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gozclrlau.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/grftojkzp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjabwmvzk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gucnqoven.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gjndhowtn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gkjpygzex.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gjekuskei.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/ggqisweod.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gqduczdum.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gfddxmguo.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/godnnkfza.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gslfjlelo.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gqhlzurcb.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gbigsuffv.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/giccepezg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/glbxfnehk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gdkgdcmhq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gkmpcazqe.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gmehxpvki.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gprypsgle.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gjpefdzru.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gykohrpfi.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/guhuqxham.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gnjzxzvhb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gcsyvdvzk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/ghyyxhjxh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gcwjbfnav.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gvcwsihju.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gieawsseg.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gqmeiihum.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gmozttynf.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gqalddulm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gxmxijdrn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gyhwbirxi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gqqxtcwmq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gjumqkkdj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gjiullvbg.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gggsnxslk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/glgrktjdi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gwglzqmwh.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gznduiwfo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gpijqgyij.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gpnipfwqb.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gldmqvilg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gxkferyng.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/ghzdcsndd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gkzfuxgjq.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/ganydsayr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gjdmkxdxz.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gockilkni.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/ghmtuhcqa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gkvxarcts.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grouqbayp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gbffisxpw.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gmdojnmfg.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gebjydutk.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/grmdxkfse.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gjxoiobic.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gfcigkdte.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gmvvphqyo.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gemkwgcge.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gbchnfvac.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gaercdpnk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcnfylwmr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gkyorpbxf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/grpzjohnn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmoplczwm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gftgewpiw.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gzjortzlj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grbocvemv.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gvvzvgwtt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gthghtvjd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/glxqfyskp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gfjxbgpcj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gcgvvhvkw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gmtiegmbb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gfxrwufll.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gvefsucoe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gcibvxzwd.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gcmubkodt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/ggzrgomeb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/givqwfqwf.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gosfofpsw.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gluchgrkr.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/grxxgmotc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gpyjthjzt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/ggjjsceuq.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gczxiflkk.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gsejyjefr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gilsmljby.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gpzdmpxvf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gocdssnjl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gitrdvmav.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvvheleyy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gvczmllvi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/ggzmqbkpo.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gqbbqvtgd.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gcnbofvbt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gfmcaovyw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzpvthoxw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gcajkvwnk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gttynfzmw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gcqqcyzwj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gsbjzhrkx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gnrrlvqup.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/ggxnquprn.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gksplplae.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gqufaelka.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gpkjowkxd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gcuppuhbk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/glqzereyt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gocwyfqlx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gqoajppce.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ghiipgtgz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gwtfrtoya.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/glyjogphg.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gtruwulqd.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gzwwtduby.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gsmnyecbn.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gvutdwuhn.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gvwvrczdd.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gqkrkxjhr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gjebcmjnq.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gxynjbypa.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gqcegjrwz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gegexinqn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gwekhrumq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gdmgswgus.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gujeazwrq.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gsfjdvbaz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gxcqnovqs.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gikzyljqz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gocgwpyjs.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/grskzgwcq.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gzeqdgplz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqznovzq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gzmkzahkg.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gmdviooxh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gtitjavbb.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/glcvhpfbw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gfubyvicb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gyjkeuwrx.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/goymxnfzs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gzcbfmovd.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gebegxgea.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gairgwvxk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gbhywftaa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gityjjafd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gtdqtrtgk.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gvnndcwgh.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gdrtmuaqm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gtrsjxubk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gbbelutbt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gagpwdpsj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gjorcykqp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gdaljelfi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gzjqirwxx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gnzqmhnvv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/grpqbbugt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gvvqjpdow.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gupxkmkcw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/ggqygtvcu.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gpdqevfcw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gvspfdjuh.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/grctjrdkt.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gdtnqutwt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gyboxewhv.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzejcfllp.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gldbaiyol.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gweonmkrt.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gkuxbrxvu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gevrtvdek.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/giqswcomy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/glrvuufxm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gtrcjbfya.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmmxdcujb.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gtkzsojgv.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gyxsrbmgb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gnwgfbnmm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gjbnbmeat.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvjgmkhey.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gfxxfmonp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gsidladlm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gtanyucoc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/goxsbblac.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gkcqusztv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/grfumgmam.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/golinsvey.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gxuczripx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gremkwufz.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gtqfgptuo.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/giadyijpq.sHtML


<!-- 参考信息 -->