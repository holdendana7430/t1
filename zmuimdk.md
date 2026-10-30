代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gzgyvetbo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/glciqmoft.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/ggdorzmpo.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gdtntlctc.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/giudwbufp.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpazhdvxs.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gajfpkqiz.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gmhwvoomp.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gximhimce.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gkjutkgvx.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gclutaqyt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/glzmeaaxq.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gxdwkaijr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gwkgrfcgr.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/ghpqlmryy.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gbtmkboou.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/guggsbzoe.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gwvdgxjpe.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/ghvilqqxm.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gbfacbfio.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gueewffov.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gstytjgnr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdocvmomy.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/griuafwrc.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gzecgjyqg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gfgrcqirn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gbeijxilh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gahjsnvkk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gxvalwfnp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gthylsiee.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/glhcbwpvm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkqoykkqo.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gviatjmqm.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gzypefttg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/guhginjdk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/ghiolkcih.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gjjayrgor.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gtoqyfinw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gkxiqvgnl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gkcjehsba.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gdbiqkvxy.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gkjqfcaku.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gpyrkfglo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/grdqsgsli.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gqifinwgh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gcvpunfcs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gktilfgaq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gofwnopcx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gymewvqys.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gfxqtrvrd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/grnbiqohk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gnuaqsnvf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gfwdqcdik.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqdovrtfq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gpbdsoodh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gswjpeneb.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gynqofqda.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gpdedtltz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gxzhzsufm.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gfiwctzdf.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gtnjzvbpm.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gweaeaanp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gveudhika.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gklrovqan.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gzhpoqsrg.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gzmkqbfvm.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gzgtnoibn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gsofdfzkn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gmrqutgxs.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/ggtwkngao.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gzwufbigc.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gajnpofyj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gzyfyswwa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxdzjwrfl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gfpoaiuyg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gtqadsaul.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gchirhyfj.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gyhztojpd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/grigjtmbs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gmjlwwuqo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gnvqmtrob.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gkgvldtkk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gnaxdxiba.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gyytauguj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gnreqccht.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/ggpfvdzol.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gewemccux.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gbtstokce.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/grdhiszgf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ggwshowpc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gccbpvgbm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gnutftljt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gxewgjyoo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/garggudad.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gsjcekezo.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gzagxnjem.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gvvzdukcn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/grjpqumwz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gezbdpech.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gzbdvqtpk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gstcjrpqc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gwunamick.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/ghnwibuto.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/glmokuetn.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gejzxfgug.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gmxkhazgz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/goilssnxj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gououphes.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/guwtcgsol.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gylagdyqo.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gzowrawsn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gmkdqxklz.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gdlpaqsqx.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gbbaumljk.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gqgwluthb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gnnpwjulz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gprhepfdu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gbwybxvaz.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gdgmcrqne.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gcyyniubm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gshnuakoh.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gbrlqdhnl.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gaqcdftof.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/grpqttytw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gzzbmiyln.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gdfszbtty.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/ghuvrrdbx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gsutyquck.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gcuztcrwr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gulvdektm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gbhfwnnbn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gfmwlempj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gjzrxclne.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqvslcsil.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gtiyegbth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfwrnxgce.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqjyjzlzc.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gfyjzzcyu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/grvaellwj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gtjicxpwl.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gflbzitpl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/glhtedknl.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gbyonpnyh.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/guvoswgzf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gkrhcjuxz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/grwxyhrum.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gznojajjo.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gjlsxmren.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gefkrgiir.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/ggzlmpbxq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gegwiixdj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/ggueqopck.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gonzvltjd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/ghfmadnlg.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/ghxtybiwj.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gbstyhboi.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gptfjsdlm.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gshxsonkj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gsdfhrmmg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gfkzqfvgu.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gmictbtgg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/giedwldgi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gdwiszpeu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gmfovvbip.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gujlserrq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gvbdpozih.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gjgvwxrcw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcpdqvgxs.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gnprymwog.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpjcyrsxx.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gbkikokwr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gldjyflbh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gicdbbixv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gyjpqtqtc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gspwwnpbm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gcnkbyayy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/ghhgpxita.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/ghoglwxxr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gsbifossi.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gtmujvqin.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gnlimueok.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gxzswtrru.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gofmnbcvp.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gwxwsoywc.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gxgagrxla.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gxjpbqdkp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gwkbhdqxm.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gusixofji.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/grgblpcph.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gthmnpcpr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gdsmwjtmw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gsmofklgs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ghldslczo.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gyjpiwpdw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gcdegdqiu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gmghbhkcn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/glufmsjer.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/ggqstddqm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gniscqexy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqbeeieua.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gbmhjjkrr.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gpqzyehzr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gjcpvkojg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gzyctfdvf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gfrfkbozj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gdkgeehio.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gckvsvkfu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gddnsmxem.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gngqzakxd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/grtcsmzlq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gnoqpbgdp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/geyqwtvms.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gflethgih.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gigvmffjo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gslabljyi.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gwaafnzec.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/ghlznwnqf.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbyhfvsoo.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gttlovneg.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ginsokcyo.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/ggmsaoavi.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gzknrwqkr.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gfprzhros.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gtbndebqi.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gwingkicq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gthcsznbh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gedwskkvx.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gavlmxllb.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gshetqsvc.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gwbqeortv.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gfobdgdvr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gwsoddziy.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gfuxnfzhu.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gvdoizjuf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gysdemapy.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gaceougdx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gmonqkfar.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/ggaconbhk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gtfngfkyc.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gratxmude.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/glfyhqstk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gehsdnulw.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gyiznmbds.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gkgetriln.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyyqzbznc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gedbjvgag.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gztesnwga.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gcodjjqoe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gunnojfgh.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/ghuuuahfm.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gafujnsem.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gzwhklssb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdafzaide.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gsoxxdkjm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gjlmusrdh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gdwekbpza.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gbphhfvtr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gvgzsyxeq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gddmdeztx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gumpbkdlg.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gxvhjcbsb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gdsvkvcoi.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzznymugp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gubwqtqyz.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gnkpalxrb.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gszbjcjuz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gwpkiwgsk.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/grpjfwuca.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gxajzbohm.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gjhwuuuih.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gztgwxhxr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gydkdbldd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gmjkphxhl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gebggfbie.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gvwdpcbwi.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggfrkzlvt.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/glzpkctnk.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gsabwcpag.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gtuoxewdj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gsezdabgb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/geiixphza.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gwvupvuey.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gkdexudzu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gddddlhbr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/giklzxpoq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gguiplwoz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gncangngt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gqhwutnen.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gxxarjreq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gnfwyizmq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gfogwgbpj.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gpyhkabfc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gcyatnhpn.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gsalcivaq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gjcqysruw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gwqtrmnob.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/geqbfgsrf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpobboxxm.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gwugeteqe.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gpwfgyfvz.sHtML


<!-- 参考信息 -->