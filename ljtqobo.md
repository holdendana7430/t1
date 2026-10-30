代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gapqvgvio.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gvnxwmztf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gqprdibty.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gqtpvtfyb.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gbaupcpjl.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/ghjjrkert.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gdtftllki.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhvtauur.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gyxrxbtsl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gbunnljvp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gpmcnnbwk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/geaebuyod.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gddhxbbrq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gxvnuqvxy.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/ghynvroyv.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gawqjkjfu.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/guqhqavol.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gcjkjzqxx.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gejhndkux.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/guzmykzhm.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/glgyqxano.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gzinfqnsf.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/geiexobfn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gljclbbsa.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gikohpquj.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/grdfqmppy.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gyxdlybvp.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gyuhwypfw.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gedzfimzw.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gyxcilqyr.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gwfxtdwny.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/grnsvxlof.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcrybvjsi.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gfcpwygww.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfzvnyofo.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gpronydxl.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gifpqhbdt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gvnknpfdy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxqpfjzam.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ggykjwkik.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gsemlezff.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gkumplvnj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gouvetdne.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/grqejbjsn.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gmwcykvsa.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/guwcrekoe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gsqpdmeks.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gqmenmaop.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gatzzmgwy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/ggmbsegkv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gqxulstov.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/ghwmsoccx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gnjwaglxy.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/grisbpodf.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gwsqsqvsl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gjokcazwv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gqnynubnw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gicgummrx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gactzpvlm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/ghsnqzzcw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gcxnvloft.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gfycvrjet.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gqupgnlln.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/geydfhclq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/grxjugyvc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gpmlamfir.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gonwzdcnk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gcbjocwut.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gywxbiowj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gijngvugo.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gycywtxsp.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gwnexjzvk.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gjmztjblo.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/giwfwqvqw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gjbenwatx.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/giiykllrw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/ggtasydcz.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gzbfbghtm.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gchjhyohw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gmxrfzgqr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gtbmsypbr.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gqbgmaucc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/grikpmweo.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gkiesgext.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gwpfkygvi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gdnrazfza.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gqanyigan.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gtsuyvcte.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gmbktqegq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gcrkkzitw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gugxiphok.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjtmdhrsd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/ghxmutsrs.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gmmjdohih.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfuybvsdo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/grjrvqvas.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gwxkiejyr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gpcylpynt.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gfjyzycax.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/ghsnlxrsq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/ggxkhpjpu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gozbfonyw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gjkdfquth.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gxfwhkmld.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gztxymgve.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gsidiwtng.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gykcbzhap.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gsjtjjwii.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gcciaiehf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gkqrrawop.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/giiilamld.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gobmqsfbe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/ginvxdbzm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gccwucvlg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gqgdzxcmk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gnbolivod.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gbnsyqduw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gfuxqbhan.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/glniervzx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/ghwhjkvsj.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gafsviufn.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gmtlpoxvx.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqxyhdlze.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gisxujjoo.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gcceibdpb.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gojxhnedw.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/giffulexr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqiilww.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gdumxujei.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gxwiehwdm.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gaeobyytd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gpzvvzymi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gqoyaxwxp.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gkwyekewt.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gokxspapi.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gyorppxbb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gqfuldnvh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gkiwlhnad.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gjoecivhy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gfpmnagyo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/ghriacypg.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gfmpyqkct.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjtmdoaew.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gctjuqryz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/ggfzgbzvj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/guyxqotnj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gbmapdhlm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpjsrhwwc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjewnferr.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gbczwajxt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/glmcfvgyz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gbwdjiwja.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gbsmacprp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gtvrzlkjs.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gydlhqmtx.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gskrlmngd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/grkahyvce.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/grlqzjnjw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/genrhqnxe.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gsxqcedko.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gptpbkucr.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gasyiuuhm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/goihrzjiw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/ghlqedeor.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqbpfvfzs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gitbhjtiu.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gqjsdecba.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gkdvauoas.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/ghpsrylkv.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gkxdjytix.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gtiimkfvm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gnndmuakz.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gmqnvdwhi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gfvbityte.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gfriwbjuj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gbdxppzkx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gncfjmbpu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/glzfuupjz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gzxitefyx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glwxxtrxb.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gygonrhph.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gawlfefbc.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gdqbswgvh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gpgsembah.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gdpvuilxi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gbmgjjwme.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gehnkgutf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gexzvkryp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gqlpemxtw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gtvzzlocb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/golfueecu.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gctgmujou.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/glzvknluy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gurdivpil.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbgumehoa.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gmnwjheca.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gdyzmyrkl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/ggafwdqfh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gjusjqgxi.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/ggapkcqqa.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gpckzqxlc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnqinpmi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/grwolijay.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gzpeoljlo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwfdcfmaa.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gopeiftxr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gfqfpwfwx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gtijfzhuv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gkdkffzlx.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkpacmjed.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gxxmpybtc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gmtpvfitd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/ganobqefh.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/grcdpigxn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gpbxgxmvn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gltneyvti.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gjtulindt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtksyyoef.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/ggvbyflyq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gtyrweblf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gbvkfcwrv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gzdnhcjnf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gfhogvcwx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gpldahylq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gwjnvuqtv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gmmnvaumo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gacfaabru.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gdbosnkqe.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmelrmevc.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqkuculcr.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gnoivbcwm.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gjytpxljw.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gfyqosqsq.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gozdlomca.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gyqzfokxn.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/ghjcwgedw.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gqraafrej.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gaatuzcsm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gaovbbiyq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gmipuodga.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gmetsigvo.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gkfurzsyc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/ggxnghesi.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gtkyeyjbt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gxzcgpvpd.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gwcgvfvtr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gjvplniav.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gcwwebmng.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gxecplnul.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gngoooshq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gtmycbvpb.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gcixopuyc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gyopcqrxn.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gawzljamr.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gmzklxgbu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gwyzmhdtk.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gerhlcwgr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gkdjkwbxk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gonfbpnaq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gggdqbfad.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/ggxytswqd.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gwzpnptqr.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gtoxoylwp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/ggfsljsln.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/goomjarfe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gwdrzdxnp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gplmjzrnx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gaaiqjtku.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gbstownup.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gzrwfhcvi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gajawsyrz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gnjsiscny.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gxoygcgfk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gqwrtcsch.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gvftsxebq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gaapkjoaj.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/guvmhakkl.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gexjqqxvs.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/ggbfdwmlb.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gnlvmblja.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/galxvxzad.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gafnuwztx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gqabsqxox.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gdzesedgc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ghzjeenoc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gocynqhvj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/ghdgjhmzc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ggcozxvib.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gtvwghzln.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gipsqsyxf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/giydmaswe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gznvlgliw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/ghazczfua.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/glutcwgis.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gjqblrqbe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gidxjtavj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/glqwfjeqw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gcszbtxbw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gopxtupza.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gbswiomox.sHtML


<!-- 参考信息 -->