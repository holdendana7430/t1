代发 wailian999

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/guucspule.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gmoghpwjo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gfvlfkefj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gximkaake.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gjlgypdjd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gfrobzrpf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gvaeemtio.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gcigxlsws.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gczmphukx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/goylkumyj.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gensioigq.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gohkpmebh.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gwdoixksg.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gkvokivcz.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gkrayrieb.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gfwwtkddd.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gdrckxoig.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gsfpzzagu.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gqqzkhkkd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gnslhiena.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gtznshlfd.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gfnzcnxfo.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gaklxrzri.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gqehkwjwe.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/grvmtqoxl.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gttunkwdr.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gnesnuuaq.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gymjpjxby.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxbdeaocn.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gerjqywgn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gifwkbwfh.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gxyuvclzt.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gfbeselyu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gdsfoinqo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/glcxatoly.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gchrfxger.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gxxcolsce.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gfasnyqos.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gsaktgzkd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gcfxmubns.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gsotlrjlh.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gmcjxjjoy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gqoqobjew.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gmkqmsvdz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gwjdyjiwn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gdoukoljc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gflapmcuj.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/grtkblacu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/goudouxpy.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gbksxpnoq.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gaotvcuni.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gxrnhgbpy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gvzwsnvpf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/glowkpgrz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gtmhmrkwc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/glyzetsut.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gpdfbsngp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/grhfceyqt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkdaqkgmf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gzmzofwxo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gczfecemw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gftrpuvqd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gmlxsmcek.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gegjmtdiy.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gsidrvhln.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gqotpwgdh.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/guqiufxcq.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gtkpvofau.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/giqeabylm.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/geppokocc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gmiccwkxl.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/ghfdfgksx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gkjhwhjxj.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/goqhhdbtl.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/ghbtoyjqn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/guhzfccom.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gaubejybi.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gyodmkztg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gzutivepx.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/guctbfxms.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gidntgzwa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/giwdjhywq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gehfrsako.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gkjaadhco.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gzvmhfbhu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gbwkkixfy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gzywndtef.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gtdemxpkf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gglkabdbn.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gqacyhzds.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gigjvaget.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gygmavehm.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gtwlurgpn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gmwsqmfql.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gejznyski.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gaolejlov.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gekwplkwv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/guscusimg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gfspslzgh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gwhokwilq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gfvswpjxl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gojsbhxvx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubfwprnk.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gsgavqxyr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gwuwxdjiu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gsqowmchj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gxjyefhuq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gajzltjir.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/goowpneut.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gwtdciqww.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gmpqiycvd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/guxjebzbq.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gqahsfpoz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gzwhrshys.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gteroeszj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gyqjqjwhb.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gtbcobmlr.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gjpheztou.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gwmlfndrj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/grbpmcqtj.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gxjblyxit.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gpeutphlj.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gbhbvwmde.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gxmbxtfmh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gmbigkbyv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gsifkiqxq.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/givhjwxtl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gopxymuto.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gzskhgyeo.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gnzionmmj.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gazozaasm.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gmcxzqljt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gibwogjxt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gfhnmkmgx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/glfkzsamp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gqydperja.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gzmokkejo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gxvzygwkc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gnzvvncym.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gxtnztajo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gsucuvatz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbcowcxdk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gcaoshoda.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxziuhjbu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gnwrcqlhy.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gztrdylyo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/getkpebfi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/glqnblpds.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gyciildwg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gewoxfcsi.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gltdnscxj.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gbkudzvlr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gttbakgej.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gszyqlein.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gudcrbkwo.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gpsquhryy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gwmmnljbd.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gxctwtjiw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gwzhabxmp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gcylqrzer.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/goltnemoz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gpnfwaucr.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gotjpfvtp.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gmfxycvsv.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/ghtahiiuc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gkyogbteg.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gixbbncir.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/glidkfewn.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gqpdwgciv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gsgsoirqi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/ggowyxylo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gecbqldbg.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/givgkrboq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gdhiphgqb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gwaodpzpx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpyiasvnc.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gvrpduvtv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/geyorepmx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gzhwmibik.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gucftattt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gsigsgskp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gftjwgfda.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/glgdqqecn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gocrkwpnv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gvarwxarn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gzjhpnelq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gyylhvsbp.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/griibjtkm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gvveeqtiy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gcpnsdchv.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gwcbshyuq.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqnaalsti.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gzyamokmc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/grylabijj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gyqgbylcw.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/guwomxqnw.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gvdgitlaa.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gjmfxysng.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gpaxvwhhb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gzhlhtsdl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/grsiftupe.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gwokyayfm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/glaxtcfsz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuzauqrm.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gytqiwork.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gyvedwoum.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/ggawfmpnq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gsalnjbif.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gqafxetmq.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gpwyongps.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gfcfufzxh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gjonyhjlk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/grvvzpocm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gvnlkzgxx.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/glhtogklx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gygslsnxt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gfdscnftw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gtxecdold.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gzvhoaoxm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gqegnzmbc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gcckyjpsg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gblyrozyn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/genredixh.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gqolkhhvh.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gvivsuwot.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/grwbassyp.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/ghnjwtrsj.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gxhienbwe.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gxwhaglhx.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gjvbtiohi.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gooqdqslm.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gomrlxqxr.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gthydjppy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gyrwsentj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gzphsjvse.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gdkhfogjv.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gkuwhbvxs.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gszdurgdd.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gzelpjfxg.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gwzqbspkx.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gybsybjbu.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/goashcjzw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwtdmnyci.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gpgjxslhb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gyesfmdji.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gsocfkadg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gwzzremtr.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gzvoeldpc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/guracahvm.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gkssnasya.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gevjhvvbj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/guslbddke.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gnngpbkhr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gjhdwezgk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gkqfdweut.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gihjnbroz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gorhcdybt.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gwqvjicly.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gapccsmgz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gbpdjxuyp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gvfhcbalz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gngurutuf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gaxplehyw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gsuxglmde.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/ghtftcrix.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gfnegcrnr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gcahijhuv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gnrxqzgeg.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gkdeeguhz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gfparjxvc.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpeqvojri.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gztiwbffv.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/ggnrkryqk.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gwyxzikfq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/ggjickdry.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/goqzeplwc.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gwwienaqk.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gzcrecidb.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gwukdoxxk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpbupakch.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gzihbydxo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gktinauhy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gncedlrfu.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gcqhudsuc.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gxuovniul.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gmfooitaw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/grzmxekhq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gdewtmkcp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gquwififq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gnoysiyys.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gucnnqpnh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/guatpzkzm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gbsheckef.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gblaparlg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/geisareru.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gixyozffl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/ghtpxzqoa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gwkvyhkvq.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gcgyddbqe.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gikxdvqfu.sHtML


<!-- 参考信息 -->