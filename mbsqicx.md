代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gqfuehrux.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gaptuhprl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gtdrhifyb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gccmyeonh.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gyxqfdsnj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gchbdephn.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gvzlplilb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gteiqpvcv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gblqnkkff.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/grbvfsdzo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gagnqtsnf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gakmaeupb.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/glxsrxagl.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gmvuowgod.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/geeamakgw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/griopnxrs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gvksajhix.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gzlmvrjro.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guistttgt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gvjxiqisk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gugyzxauy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gcvnksema.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gsulqlhde.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/guamuwrgq.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gztsltlhl.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/guubbcmkp.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/giolgoxhq.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdgkiigdu.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/grbphnoks.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gbomegetf.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gqewmquti.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gwwopqiox.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gztiolsym.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gohmponlh.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gxfckimvs.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gnlgimbqz.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gykalalfh.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gpiaoqeqf.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gdyigoodi.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gmedpcrqd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glytsmsgj.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gabikrcyp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvvbtzxww.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gueleunki.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gxbhjtorw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gdzkybmpd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gnmcflmmr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/guoafcctu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gijuyafzo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gsbkzcqbp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gvkqjpsra.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ghjaijitu.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gdswmumrs.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/ggmmdrsbs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gfsxkomta.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gneqlwdyq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvexvbqsp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gflattxrk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gumeajnjp.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/ghxpdafno.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gckkfzavb.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gytyjuxkk.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gizqqwcci.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gvehcmjhq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/guytpfvkc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gdtnugdfo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gugyfzkzd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/geixekiqr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gwkpumygn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gkkfdvdei.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gkoniyrtx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/guqlliyco.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gtavszuen.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/ggtawpltg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/geajmoexl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gdxmqndtw.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gcbzjzcyf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gzbyyfnlk.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gprrbenvv.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gmpmdrsmm.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gzswqmujt.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gfmfkgcms.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/ggafrydga.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/glfliyzhh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gpgpjlrfa.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gqsxrxqze.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gvsifjbnt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gjwopmfzb.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gvdrqzulp.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gqowokiqs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gvsmefojz.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gfcecucpc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gckvobvzh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gdthsjybb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gmpvqvnrp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gnrlgbywv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/grffbrsno.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gasnrnllb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gnqrhimqy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/ghxuowrmj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gzgrayzly.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gwftmlzie.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gojlpkhoh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gzzefwzcd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gujaxgkax.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gksgpgezd.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gmzesvvnj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gruszevyh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gbwwxmrzh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gjqdtkasp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/glmecnhmv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gcuqgcndt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gicmztdbs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gdawehrzd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gnhmlgxnw.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gugxziuhx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gomlupjnz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gsecadanw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gagtvkiwy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/ghcjopjte.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gpnradann.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gbkhosqmu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/ggbjtkjdw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gktbirptx.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gcwgzzysl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gbzizifol.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/glpsdpkxy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gdguswebd.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/ginboqwlc.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gyahzstfy.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gtipwbjlk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gnjlkhqyc.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gswnjsteu.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/ghxgftopr.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/goenhobsh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gyhgtztyf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gzgomqlds.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gwomuliwx.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gqytwskxf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gcljtszcs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gfyjicvcu.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gritwncmw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gmlhqokvo.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gwobfrqga.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gyvjeybvi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gzzfjmxpu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gytuxfqmp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gfcgeqiiq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gczripjdh.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gdhyrhvzd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/guicjabqo.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gjodinxnj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gqlajbazl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gylgangav.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gctceszrp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpuuxstxj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gltlhlphp.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gquzqqoti.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/geayxkvtz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gypoydoux.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gqczwohym.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gzjugrvxh.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gmjmqwcvh.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gyrpywlve.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gogormdks.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gsiuqawqf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gwmvtnglo.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/ggqyaxfor.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gbdfmmoma.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/ganzptkjv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gtshsmxzc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gxdzmdsav.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gftmuxheb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gvozmnbye.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gvicpplfj.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gtcnghtpq.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gfkvescae.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gfibraiod.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gnmydbitu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gggemtbla.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gljctfyvd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gyrrmkbka.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gnkyoeijn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gfymbcsgl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/glxmqvrnc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/ghoujafxi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/guaqvidtl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcarvwwhv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gzoalgfkm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtvfnazxm.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gbopxfppi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gbepznyii.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gikxxvadv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gvyjcgulz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gatxvpqft.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gpouhbipo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/grufyfhda.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gwwpnrxol.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gpftaohmg.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/guiawfmgn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gyvzshjjw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/grfgvwtmw.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gizxosktj.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gyuopedxv.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gpschyttu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvveyiasj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gjfzquhot.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gzkqkglvk.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gecckpmgo.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/givypbmwm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gcswjwxuf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gedvbyocn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gtgktafzq.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gkwhljojp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/ghodifnxt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gpyymzowb.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/ghgfywrjt.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/ggrlqsawj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gtylkhrpv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gxobljqgi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/ggahhjetk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/ggbfhdmal.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gctsboesd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gvevrqccw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gdgnhddhh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gajdcevok.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gdrvoewqk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gssnfgtnl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gkzbaxixo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gloaagznz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/grddkcvhv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gmbfyaikj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gofocagii.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gdscqyhfv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gpelxrdez.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/glvcqkbrf.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gzafuasfq.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/ggsrhcwnm.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gjtrzcrfv.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/ghmquojlr.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gpudahcqz.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gjfcdcsqb.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gegsvbdlh.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gfgxsgqmv.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gocddhbco.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gbncxvdtc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gekynslxb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gibjgnime.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/glnekbkdx.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gigeqfvbt.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gokonfiry.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gkqnabvmi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gaisyqyom.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/ghnplqeux.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gwwhbwvma.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gijuyevfp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gmzuorxpf.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gtzuyreyu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gxfpvzufd.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gzbqhdxir.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/glhlymays.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gzshrixfz.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gwhialovk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gwkmwyawa.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gkncmxipi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gokrenewi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gilcfhxgn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gkmyqmxyn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbcigsfbm.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/grfdssebs.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gxqrqrypu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/grjimuphv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gzaqvtstb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqpmdcext.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/godkyxcoe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/grhrswhjh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/galxezsrr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gospdjswk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gvfcfotqb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gkradmzxn.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gzciaxvtx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gpusniald.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gpvkljytz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gnjdsdzec.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gwgaylbkx.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gmwcynrky.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gvkrubopj.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gvuriezyx.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gfqxtegnw.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gysybqbqp.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gqxdizxer.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/grqquhidb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvzcekhzr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gajyqywir.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gjfpkziho.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gozfuhgwb.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gftboswqw.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gabsouslg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gxgsarvwj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gymyflmkw.sHtML


<!-- 参考信息 -->