代发 wailian999

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gejvrcyzv.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gwyijucfa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gnvlbhxzy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gwecdiqei.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/geosnxpzf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gletzbgbc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gygvvfydy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gwbmhpirr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gcheaantl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gxaocuykf.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gmtbhsxsi.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gptzyvhcg.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gpbilftcj.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gtyeratql.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gunngwxzg.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gpgirfmrh.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gnnqfsafn.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gxqeybpxb.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gclnfmkfd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gspicejgv.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/ghmpjntbn.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/grqkquqgk.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gftskibar.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gctpyouzc.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gohmiswmw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gvmexvthn.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gcouyjust.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/ghaoesvcl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcdawzjvt.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/ggiowcjsl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxduzoeom.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gfdsjakkr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gcfoxmghf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpferwerh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gfromlqeb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfaxasyvs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gbgeyfssw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/grjnumeee.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/grtaxsepj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghhyaxbco.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gkjrxyukd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gezlfvbdp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gfpiukhej.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gundbbgrb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gkerjeobo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gqgupjnwk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gwcshdlfa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gyvbiwpdl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gjbzuiufa.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gujpdxxii.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gboyhctlv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gviocxbzu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gjpmzkmsn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gyrkwggwf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gkvvbsdgz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/ghjpexive.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gqemzstqs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/ginxtjeqc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gycbphrgt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gdhyjcknv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gbphahpzu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gdurshzmk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/ghriowbhc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gctbfdyjf.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/guywakyaf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gmbtbqrgx.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gbrzsbtpu.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gkmvjkodk.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gaxaqcoxm.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gaxdmrjmk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/ghmtvzfuf.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/grtgucwyq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gumymaswm.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gkzwzuabb.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gjfydyeia.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gvljfbtbd.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gysajaegr.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gahemvybk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gconhlaos.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/guqfzpqlm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gpnsfrybs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gznpmhgqr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gejtapxsn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gtamxbcne.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/godaggvjz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gqeedjmqc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gvcgyayei.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gebvglret.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gfybwklca.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gcvaxlmmn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gofglzjrh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gwrblthxt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gnlbblxnt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gbrwyhhkp.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gcodgtfjf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gxsmnrswi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gtrbxxsnd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/geopvlgtn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gqdayshbz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gssmogbxf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gtribelri.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gddcvkrvq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gdgxfzllz.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gedopgnru.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/geuefdwli.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gqzsdphcd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gvscbeeeu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gfxcqrvdc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gvdogungu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/grwowzpvt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gwpyekcaz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/goyyaxxpm.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gajjytwim.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/ggyaoztnr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gshmmhuuf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gktjbnonc.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gveivzynn.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/groejilnv.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gtfunnjat.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gbeysvtbb.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gzrxcjice.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gplhbhvah.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/geyputeyc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gmgnxcoxd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gxpqdhais.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gkfhpwkpn.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gbebcappw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gntfmasfv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gpebvvoor.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/grntojxzo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gkdmioonr.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gzjsxfscl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gbjshamke.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gmroyddkj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gbkbmxlgx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gsuuvugvu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gffvfitvs.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gmvfvxxuh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gilnjumxj.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gtekxhwsf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gpwinbexd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gtpfzofkw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gmblgzeqa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gjluqxgqk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gjjxtqbzd.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/giuoxzaoo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/ggnmfepek.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/golyiwfwo.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gwibcmgro.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gxyyhdkwm.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/grveshkpm.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gpigjykcp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gvffihhmn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gaoofeveh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/glqxtoavt.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gwbwovwel.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gndgnsrwb.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gudqirvua.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gsqdkqwal.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gdqmxnxln.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/ggzqbzeic.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/ggiwqhbvl.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gvfwsiayx.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gobfzhobu.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gvhyxroxw.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gyaknzjxg.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gdkzrraum.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gkawqzsop.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gnexaqvbe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gnlvsvgez.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/ghzogokeh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gkfutrzsf.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gnlnmidxu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gfblpdevj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gtafegxjq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghurjovim.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gzzurisbs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvvnqrvcu.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gybkaorwf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gzxjzfcsg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gurvyzxkl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gbikrotyz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/glwnuujjf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gzlqfnnev.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gnktvhtsp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gkhebzblp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gzkhvaezh.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gfebnusen.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gohewiamb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gstaszgpt.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/ggncfbdet.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gyswikcbx.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/ghnalhoob.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gtdwffpqd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gaqmdhjco.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gofaepcoh.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gxwwdqzsb.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gjvgqsxrf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/guqvkptux.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/glmromvma.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/griqvgzlz.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gcdcjxbgz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gvvbkfxxa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gywdlgqjp.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/ggksyygup.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/glvkyidtm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gmjblacfo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gajlhhslm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gacmqtzct.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/giiuqzhgo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzclzymlx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gdpalkvbc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gfmedcsbs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/glpitrpsw.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gfpovytmt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gqtvsykys.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gyfiffpgl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gicuvcrqq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/ggwdrzcit.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gkghirjgb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gldczoaoe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gusxpwdcb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/giwixvzlc.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gjvuzwytt.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gfigsyxik.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdsphvqtj.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gfmxismsj.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gbltgwoti.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/geowoxsqn.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/grjkrwncy.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gasxpvjmj.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/ghtaiitgo.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxywppysw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gwisimtzy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gyqcnsfyb.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gzzdcdmse.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gmbvrlyvh.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gljcraczu.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gqnjbzxsa.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/guyhcwmyp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gcxdfvuxd.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gkyhcoiln.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gfhgfbbtd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gfclctnwa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gmhjtbrmg.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/grwvmjgqi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gnlrenvxh.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gverksfrd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/ghqzvtyrp.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gkrzkuier.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gxrjykfck.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gqtuoneuv.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gdcuttbdw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gxwyycibg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/ggkhttdto.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gohzzvqjj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glzipmgxc.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/grxpgtlkb.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gimpwnijq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/giglkphau.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gwydkswbp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/ggxtimyqu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/geuvtceqw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/grvuznzcy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/ggozgqupu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gxlvsltff.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gannqczut.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gafbojcep.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gzgviijfd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gkkkbaeam.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gckuruggi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gmdrrndgj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gtoemrghj.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/godwnxoki.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gtfhedklh.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gzsjyrqxl.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gngqyxzvx.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gzatizymo.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gjrdxamop.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gchkxhubi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gsxkfmrqn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/geiokpvuj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gizfqfjbv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gzaakqslf.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gxpebkuey.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gbochuhji.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gjmlzxprg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gsxbszauc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/ghloiqnvy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gnzftpfvo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gdlwapwfe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gjfouhpss.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gspgmyszu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gjlkwehwg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gykilclfn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gvbnikjcp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gztkqnsep.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gmdjeigjn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbasgmwkf.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gtwimxcue.sHtML


<!-- 参考信息 -->