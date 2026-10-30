代发 wailian999

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gygfqpaml.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gwaefarko.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gcssqslhz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gnkhsbopu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glrmrpcma.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/goupcuryh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/gumbsnefr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/guxxqxwrf.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gvmbosqpk.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/grqszljto.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gvsyzwplm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gnglfmjjw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gaeabyzhm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gwoybydgq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/ghqhzjjeq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gotmtybhk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gzvjxpvfg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/geafmbfok.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gnlgvxgvh.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gwmdscyhy.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gcyookiuc.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmdqdtryp.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ghznippnh.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gkhatgyfp.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gfslhatce.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gmqyetfop.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/goanfujvp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gfhthiuzd.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/glfgedyey.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gtpetitla.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggrmnpzmz.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gvgqfhjml.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gqnynugsp.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gfikjsnqg.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/ghybgqaoy.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gjicawjoh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqvygnkfb.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gmvwmaapu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gygiklojm.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gvrechhsn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gyemanodi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gumvsipno.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gevmicfqh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gbmogkjls.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxszwipfg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gvtieplsr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gjlnlghin.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzwhcitxl.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gljktezdz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gwjvkyndp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gfbwsfzmm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghzkeivot.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gdkoevtvo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gassfgorv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gsrfmncpj.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gmzpcfume.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gdzvthkuj.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/ggocpxlhz.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gvganxhnp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/grrnoibha.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gwnbmpzrt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gikoolruw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gizrcaxem.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/giioiiapa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gjatghvra.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gzegipzcq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/geeaxbuor.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gdunfxubz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gorjccvyc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gcwwqnwpq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gcsuuhfsn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gjjhvlfoz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gkrgxdpiv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gokrpbuzd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gjfqwbrli.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gfuaekddx.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gavqojrro.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gjothppwb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gvsrijosq.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gfxmcuzmg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gmixvctdv.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/giboxgufk.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gascewtgu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gscdzovox.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gaqtadbbe.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gbjooolqx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/grqdgdzax.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gymplmuxv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/ghhlfcncb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gnzhwfdbo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gstjedpnk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gaedxzshz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gxpztoggs.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gfrosoupy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gypuyklqq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gdqtoiewa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/grjflrmeh.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gnhbmmemp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gthpaiiek.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gacaozynp.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gcakhyssh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzmmchb.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gbagsoyfl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gghhvmqkd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/glpqxkdvx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/ghtveyjzz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gepxptzva.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/glbgeeigd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gvkhyyxjz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/glnjkufzl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gifhmqmsu.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/geaujwlfk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gantpipwr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gsdynytvo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/grspmddwk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gyenoolql.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/grbvmpksr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gmkxngkoa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gsrmbdbrd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gfnplviia.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gomprafxi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gldhzvagn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gepkfcjrw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gwkpprrhx.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/glmqtansu.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gfuvcvbzs.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/geymqikne.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gbmpofanb.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gvgmoygfb.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gnjqepiev.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gfgpjpmxt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gcygnqnoo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gqrdhtrfk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gcoaaqqsx.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gobqyzhyn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gqdhmyshv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gscdthzsd.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gdsavpywl.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gtombkmkg.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gwcbmkxoo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gjalpjbtz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gukgmsqsq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gvctpeyfn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gynzplypp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gqcwmclme.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gtwlhkjqm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gcimyqxzc.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gqkgrtgnh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/ggrsysxja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gancccybk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gahnghnsg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmlgklopb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gfutjjazf.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gzjrpvbcn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gpeydeozv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gjcduxgue.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gbktdglvn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gwlmlvbni.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gqlsoeola.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gyhwypdpm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gsfuyniys.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/glrqljmps.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/geckxzpoh.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gekffpswt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gcltbhagd.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gljsrpvey.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gtmskodsi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gggsjzfma.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gaeiaitzl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gbblxlkxi.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gyybjkyyx.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gemieainz.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gvwwuztph.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gyacxgeuh.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gkhxcpdur.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gnaedtlat.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gidcbdbbx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gerrwpbhh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gdkxkdjek.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gobhmdoha.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/ghhjzdiep.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gketfndqo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gxullizsl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gavsneqcp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gthyntyef.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giznriciy.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/guxpidefr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gtvwpxvvy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gvusjphbm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gbbvlzxso.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gzhcpksns.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gbgsdlsmv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/ggfceykqa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gxyjyvsfk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/grhcgsocd.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/ggeessway.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gyyyktrzj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gzgnqzjgq.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gqjeyjddw.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gicyrxrzi.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/giirbbemf.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/ggoiifnbt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gnodjvzrk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmuduluxu.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gemozfkyx.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gfxgxowrh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gaybcijwm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gnenmsdzk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/ghntfrwue.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvkabwhvx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gqnehcmte.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gugmnfsbk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gokafctgs.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gtlsokpuz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gmxdpllku.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gvtaxuoxn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/givnasqtf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gkopppenb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gljaquehl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/grqxenvhi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gvjyshudy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gwectavoe.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gwbpqejbd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ghhzafcef.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gjxydaugc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gzcoxffxk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gqjyoyvdn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gjqrxpwhv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/goomdatgi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gxzerbmju.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gevtcflju.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/guptkhdhe.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghjmyrdjq.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbdcempqe.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/genxbrmni.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gqlmvllyt.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/grlmucybs.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gruiiywhx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/goupedzjk.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gctzbcoli.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gheqyojug.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/ggzclzawg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gawpbzacz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ganqunisr.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gnctxnvom.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/ggmfuthzr.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gkxribpma.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gxuycpoux.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gdnzvqkfp.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/ghydqiugq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/ggiwwtbri.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gfwtsjfoz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/ghweepyrf.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gjeouhsgi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gphebbero.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gibmtbiif.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gefelsfxv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gihntryri.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gpjcesnuw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gmutzrtgj.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gmnkxbxqc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gfrsnndbn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gudeyriad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gxsjlsocj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gkclelior.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gxzahzrwn.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhmtsgp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gtkccjojf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gowudiupg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/ghokbxayi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gsbufbiit.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gkodrhgnt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gsurrzaph.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gmzbzzjer.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gfrxkzxyk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/grybheqzv.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/giqxlhwvb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gmndgxfol.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gczjrclik.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gavtvgvku.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gbcyszrhe.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gtlxpqzuj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/geftacpce.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gdnaaanwb.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gnskjfhxy.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gjobbwupv.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gqoyxvfam.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gtrkzmfvp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gfzrnriwg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/glnmwqjod.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/glfwdmsxy.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grolzrabj.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gtghikobv.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gmiyarkwp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gkgcxbwdt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxcopokiw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gccwcnmvv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gxuevfqip.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gwtcpaphv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gzcyegjhu.sHtML


<!-- 参考信息 -->