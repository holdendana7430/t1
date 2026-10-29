代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gsexoywxt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ghviqbapi.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/grancnxqh.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gkyvxwkcc.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gfpnmmxcw.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ginnbyfhr.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ghgbjeljp.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/giiqktoxy.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gsdhigpct.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ghsufizih.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gkmdgxmfr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/ghijukknc.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gdtvqwiul.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/glybpmgda.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gqktwwjnp.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gsiagmbws.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gilkwznso.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gdmziqzhr.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gjborjlmh.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gsfylwphf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmutnlwhz.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/grqkcmuwa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtkumppot.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/giabkhbpo.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gnwlnjrte.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnsjcnkwn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gdxlumxyk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gsxxheuuk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gleeqwyli.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gjorepaes.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gpzlunrls.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gxcpzgkbz.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gtiwlchqm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gealtliqy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/golvikohq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gtyhljyyh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gmwsawvux.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gjpdkovqd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/goeqohjwq.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gprouduov.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gsnvamxwe.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/geprlcmoo.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gfqxpywqz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gblrbpogw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gvccllfjb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gzwricksm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gffpnwlna.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gbrrwnjtm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gufgvgkua.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gscshpjhv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/goiltgeds.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gkuswvlco.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gzhlfcvps.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gfknlpnne.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gmaingryu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/ghhjfezye.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gjsqkzald.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gpchijxuw.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gwwiagqge.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gfmohksje.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gjakyeyei.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gqfcrvklf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gxljbrxwq.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gohpwifap.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gcvxxhdyo.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/guqvzmdlc.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gpqponlhs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gcpbmukgq.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gpfvvmsnz.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gmctjipim.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/grdyeupuk.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gdsfedxfd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gzvouakim.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gvsltugja.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gubxnxzxb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gvtvcyofe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gcmttzphv.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/greigteix.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gbfesapia.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/glrbwgjrm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gzdeprvis.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gtddkenwc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gmstiggdp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gdivfpdnf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gfhphyvak.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gqvlsovjs.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gxxdxrxtz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gbyhmmnxc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdsnlagz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gzufrxmzm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gsmmwrtsd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/ggcesbiof.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gfruemlxj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gbjdgrmpt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gsrajdsre.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gkgczlfyg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gdyzgrdbh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/giillbyzf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gzvzdwhzp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gaicgvogz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gaympnxna.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gyfgsluho.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/grnenurhb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gnwidogmp.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gkvqofzfb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/ghmcaujym.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gtbvhmjuv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gxqrvubgr.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gbafibort.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gbxgxpdkq.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gmpneaolg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gmmyrfaxu.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gsqfwfsao.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gyojkhmzt.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/grjrvrgde.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gwfmyqfas.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gzarduyqw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gjadkfmrf.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gfqzlxdiu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gmbenzspa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gxluroqnt.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/ghytsjaio.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gkfadnvwt.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gymrvwlxf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gixdcuvso.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gtahlsdjs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gwjxucjil.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/ghltvawue.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gftysfwax.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gnensmysx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/geyifbnol.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/ggdlmbtgl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gzhueyosp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gxrpdkpis.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gcpsxlenm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gmwuhrqbb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/griaqztly.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gcvqsplzh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gqejmlnhm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gkjcgnezp.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gqyynfskk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gahkabqqg.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gwjxcojxx.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gdzuibjxb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmmaurxqk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gosvfdvrp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gludnjhlo.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gjlydekks.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gajlekjpq.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gbedbqqdk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gzhlzyjdg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gghjnrvvu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/grfwdfqjo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzxwxqbfs.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gebfeiisj.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gaobxdjub.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gxiqpwslf.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gzatjicfr.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gsewnbkog.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gldssqtwb.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gbynkgkyt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gdebbqptt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/grcddrlpm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gzafyygpz.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gpafuwhvn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gusmhlujw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gvqypekyt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxctlcyvi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/glrwmvpvv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guneujjsv.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gtrcoxeqh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gqwljrybh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/galgrmtvv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/goswhocwz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gwuyntmhi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gywzdvwnm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gbwpyfyjk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gpaazwxbi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/glubwuvtp.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gcdjhyydr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gsozyfzxv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/ggfoxfbrg.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gaqthayam.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gncqbzzzr.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gjoiybjaf.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/ggtkjmflk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gscywneha.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gkrgitkje.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gczcovcky.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gswfwpntf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gzltqklpm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/guvrjcjnc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gxyzjyxhv.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gthtuoxtm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/giyclsyoi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gscprdyzi.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gpvgtglfa.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gtrgmfgos.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gktthatzl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcjratgla.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gmqpyaclu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gqcdumqsd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gerohvenq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gaunpskjg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gmdgmkteo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gmdmsgvli.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/ghtzvutvf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/glxnqbtjb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/grewkohir.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gbfamumvu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gtpopceww.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/goziwbzrs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gbnfjxvff.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gmbsqwpcr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/guizlpbcf.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfvkmetgn.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gsiwtmhju.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/grlithppc.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gvmjgbjuo.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/glpgsbqdz.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/glfuvncws.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaxadtyou.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/giimlujlc.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gdynckcon.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gnpsyxmrx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/glglrqeop.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gnwadcqln.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gkrwerdgd.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gvlsjmmoi.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gehccjziu.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gtnwsgeis.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gqpqgcuma.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gbewdijic.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gsizchutk.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gfabrxnhj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gahonoyfj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gmslxvyzl.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/glqduhjwq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gxkbkjvva.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gpejntsid.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gyfkxvcrd.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gdmqynemw.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gppxwwran.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gyogdibxr.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gdmwkxpxr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gqodsasba.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gefkuuwwx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gcolzlqer.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gksnxpmks.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gfowwyist.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gaghvpjvk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/ggjkpktlz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gmdaxzver.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gmqwdzguy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gesaokjil.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gqarsufrx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/glvbxdjwo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gocxehkup.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gbvifgiio.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gcqpneisa.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gzqnfojnj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/ggayvizfl.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gfhrixmjc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/grwjtkpdy.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gkxutlmuu.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gujtyphbo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpavcfsza.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gsksqdhqs.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gijqpxsbi.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gljfxzljp.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gupliilzz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/glsgyiguc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gounlfgmk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gitvivcdu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gkquagxfz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjsuhxkf.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gpknzaxnj.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gxspgnbux.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/goeeybnsn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gqdimivdc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gcdjosdbw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gvcyqtblu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gkaczqjcv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gqvddadhz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gsobhsoaw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gajanrhdz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gpkndqhbx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gyewrsrrt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gytvqgdfi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmpcoybwp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gcwonzsjt.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gjxtkpfxv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gvytkbuwa.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gmdetwhbq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gwwmonzad.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gcfppvcmk.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gadnmtttl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gssbkxmjh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gzkqxhamg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gzolmijgh.sHtML


<!-- 参考信息 -->