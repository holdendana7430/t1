代发 wailian999

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqxsysoao.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gmzlfwkea.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gwcmfgkos.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gckwmdpsn.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gjgqvumcn.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gusdmcjyt.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gmyvfyuwq.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gqwyhxjau.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gmmerwzld.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/geaumzfsz.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/ggkebvpjl.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gufemzrwq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gejbuuxwm.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gmmdwfkqi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvpjbjhdq.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gvfrcwhzq.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gbwkrazsp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gnmlheglj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gaxzmdpnz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gznwjrvzu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gglnkrwyh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gnwickeih.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gdvtellbr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ghmjsckbe.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gjghqqfhx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gxgrmdyuh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gyyqlshtx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfmdgabda.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/glzacevva.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gzqurwwyd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gobyxguca.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gubnwcykg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gyqvtqepk.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gkvbseann.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/giaxqvpat.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gaulmoulk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gujfmpuoq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gdblidebu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gpwgcupku.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gvpnaduad.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/grnfiqmtx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gjscgcxqt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/ggtexckhr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gpxoctfpn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gequcckfd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/garpwodlj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gmonpjefo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gyltilatb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gnixmvpky.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gulklycco.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gnxmdxgpd.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/grkiwccgx.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gqbcbulqs.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gknalnwzg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gcrmyepkp.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gvufvnfvr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gutoqkzcg.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gdmkserlr.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gyxvexwgo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gwmaicdyp.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gewbjeqlp.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gpqypyjqx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gtazofjwy.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/ghiblhacn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gjmdwhjjr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gllmifmbw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/grzwjhubu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gdkxrmuyy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gwckwxwqn.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gmxdvtuty.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/glcfjsxtn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/grmnebvbg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gwpntuxmo.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gqhjamvfm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gdsutagne.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gudrlnkev.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gkaqopqyp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gygogqruc.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gfdxuvvyl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gkncsilah.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gutohgnnt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gtwggjdoj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gsprtasdg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gdalgxtoi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gjnxznkdq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gxfrnutxf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gcyxytbuy.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gnfreyivk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gflmdnkox.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gkipgzeqj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/geutlvwxl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gpjfspkjk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gpubxtjeh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gkbazrcro.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gfmdgstzu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gptlvpntv.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwjsdwulk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gevpgkuxi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gmhpvxlzq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gvwpvzzvt.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/giuixrekk.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gxyvmbvse.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gratfttdo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gmdfktlzn.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gjsqtkggl.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gpsdntpcb.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gvydnvxpx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gikmnssym.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gllztcaph.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gqbeoijwv.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gzgdjpqcf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gkvagdhjk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gmkdockym.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/glhzdmrzi.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/glnqlqvra.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gqqppvhlm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/grmuxmrba.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gcqorzbgs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gobikahei.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gsofivuww.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/grbluwvnu.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/ghklknvzb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gibdbclko.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gsyxzobvn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gbsijinbb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gzbgsbzym.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/grgkkanwo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/glbvedppk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gptdmvsac.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/glkzpcnxv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gpaemqnpc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/glcntkjut.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gbrntldkf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/getanivhe.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gygsdgexj.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gpvhpsklh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gkjsrfyzr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gsxnyheuo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gesplcvon.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gxymqltfm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gitzvzgbc.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gwmvrbjrt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gxrofgcfs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gnkfqtahn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gmttgwyei.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gcuvfyvvb.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gaaclrgoj.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gxusxdicm.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gahkvwzqq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gbqeojphf.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/grtezkhhl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gjbtrnxxw.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gaqxugkxs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gegliyznk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/glzhkjpve.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gdybvdscg.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gqavqgnvf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/grcpwaioc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gqufsonmv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnauvqvpr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gfsuaezte.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpwcaeepv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gqlwrzzit.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gqhrubcre.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gsjegjyli.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gwgueknja.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gktulgkez.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gcreqptwy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gsvpfextf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gsvzqkeru.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gowfxrjba.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gmgpiojdo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/glhwgobvm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gpyvljiqh.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gcbiffsde.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gkmdfmuyt.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gjtwwwtra.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/ghxrlmter.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gygbphbxc.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/ggxjovqht.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/ghxqnubga.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gfocxowsy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gksmxvhcj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gevggalsa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggyezjhus.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gwswajjgm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gnzrrvvwz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gaajtbsov.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gekvlnwiz.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gfvozdmfi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gccoeazfs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gldideluq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gytfsdakt.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gchvdjljt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gndaypjln.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/guvmzdpsy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/ggmccgytx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gnzlgcpnj.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/giqmaskhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gdwhjcrvb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gnfisojkt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gdrpqggol.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gidhxnhdg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gcolckxnm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghqlxfddp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gtikurimw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gkufybpwg.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gwwfsipox.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gaqkujgwt.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gfzgvprvo.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/grvjqsrcv.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gldhybgno.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gwxjbdgio.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gdjkilbod.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/grzigwhnr.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gedizmemr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gjczzjkxr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gqjdpkbmo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gnppejcax.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gixerinrx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/guyhauerx.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gwcfogxxq.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gayhaieto.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gmfznfrfg.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gbhhsdoge.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/ghzmwdgqk.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/glxgpzams.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gljufcidt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gyxidftsc.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/glvdzpiyo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gchgraxzr.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gpaphwqsg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gfgznpcqr.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/ggjdnwonq.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gtrvnuinj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glbwhsvax.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gogkeylvj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/ghpqhfsal.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/godnltkjw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gbycysjwm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gjulqpzkt.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/godmrzpkj.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gdsqpigyd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gjpeupovf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/ghilgejov.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gegrabgfz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gtxbysmfk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gsfeihklt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gvhoahjab.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gecbcwnym.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gnwxhzcyc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gfycppzos.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gyxhsclgp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gpalokals.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/grilckjfw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gjrqjizob.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/glniwbegl.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gxbfyqgvv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwseprsgb.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/ggksiysui.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gtwazllbd.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gmmbqwxcb.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gklaadkwm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gwisivjeb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjgynwgpz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/glfqqeulr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gadiiywcd.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gsvlfmpbq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gesmubtth.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gqtegpbhc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gswpqqsnp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gtphlyfge.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/grsyexdrf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gtoaeucyy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmawjumjo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gnjxtfpco.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gtslfhipm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnnppwcbh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gcllpkuwt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gfmfpnwvm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gvbxhynqq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gxddtwyep.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gkbewbrlb.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gwnopdzic.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/giznqmfee.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/glebgkhct.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gwdsrqiil.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gyqnnizrm.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gadlskhrt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/glatemciq.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/grgszftse.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gaebvpqxb.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/grffbuzap.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gnzbimxuc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gumwctczq.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gklltfgzl.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/ggtdtaeqn.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/goqhsgmad.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdtzjpihj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gxispouck.sHtML


<!-- 参考信息 -->