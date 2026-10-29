代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gbflndojm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gsiyuunqd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gqtfakejt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/ghidvalfy.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gwevzzeui.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gzbkwrunz.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gvmsucinv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtclqbqcw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gftdzbzih.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gqrysjtnm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gbfasqrjs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/grdrlfejs.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gydvmxkof.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gncjgfudu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/geutsfsgn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/geblzwwzl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcnwbgllu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gdqztajqb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gjibzwvdd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/ggwhhmblj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gedweqrzg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gtbqxjbty.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gnfgjwswx.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gklssqgzj.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gjvfumfia.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gherjtdsj.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbtnsrsfv.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gpyazqkqt.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gbsfhemab.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gjqhwijap.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gzexgtugi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/ggddiizyk.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/ghsbeszra.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gcuiuiutk.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/ghrvcxkyc.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gfsyvwwmx.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/glgqtkulr.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gewdspjnc.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gfyongufd.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gbkbvqmcv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gscapwdef.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gtzkcvhww.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtiqefzye.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gjvphfsxt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gwitptffo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gkajhfgwp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/glbezdetj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gzolkfbvo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gaqvbbsnf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gwnvcqrif.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gyxrxakxz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gzrwcknvx.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gnqrmcmry.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gprvluydo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gsvwkyyby.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ghhghysyw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/geumpiyvc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/glbonqsta.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/ggpfwqhyg.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gmpufpzfo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gkfaiouqv.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/guwdniard.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/glcmefdeu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gecvofdhq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gxgkhorgh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/glnupvyhw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzbicarxp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gpzmpvnca.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gyigjdaqq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/ghiknjbmp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/glyqifvmw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gidpqnwia.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/guvjgppqt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gsrzcmuww.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gocusfsjr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gpsfxmakn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gzozsmnve.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/greqysjkz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzekmxrhy.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gifrhxjfq.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gyrizxcia.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gvsdhbsdw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gqdvmsppa.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gdkhoywhx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gvzsfsduo.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gvwokntpg.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gzoazlyma.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/ghvxgdkya.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/garllhtis.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gouzfybfb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gojzfjbxy.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gwoafmlaw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gokpngwpr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gbzlxclbb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gtrrekbqg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gceonbbyo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gxhkwmcdj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gjmnrpssk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gqhcdmuvt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gpnifjwdk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/goyhdmwnm.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gspxfzbdw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gnvncgdoe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gniwebwgj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gjbeijnbr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/ggrmlmwum.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gdprzvlks.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gibiahksv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gqrvyxdtz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gszqlkfxq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gtwdfbvdr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/glshvhway.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gaxryhkxu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gsdxxortg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/guafwmzro.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/giiboyyvb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gatgfhvvm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/ghytplwll.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gssrxhykq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gkdqulgot.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gplbavqca.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/godswitrr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gklgjhdjl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/ganyzarrg.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gpkmhtlmx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/ggcqakydu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/ghsillgwe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gupmznntc.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/ggvfmchiw.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gctyyghcn.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gptuzkzkc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/ghoetacvf.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gihptksuc.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gnndmosvf.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/ghzinojly.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/ghuiwuqpg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gsgxymwiy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gktpgrsei.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/glbqcrfpq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gdttkepfh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/grtchqeuj.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gzfvtcrbr.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/ghrfvtehd.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/ghsrykbns.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/getpxqblh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gawyyrdnu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gxdmkgtas.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gtxhmvmjs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gspxxqdlo.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gpewwgbbx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/graptabdn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gauxjsopi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gkzkasams.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gsfzowkhb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gwpcuieju.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwydafbkm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gcihyifik.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gefrojexx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gdlzhknzi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gxyxlrjrn.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/grbiqahbt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gsdfzpquu.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gfxxiyjos.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gczinflgt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gloitluqx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gzermngih.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gdemmhzhx.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gehavyzzz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gqhylgyar.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gqoxnyyqh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gjpzgwchd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gnbocshyj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/grlaahpii.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gmkvyynlk.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gjgfufbmz.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gurqawlvg.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gcnwpyaph.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gtgccrcvp.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gkwkwhgdn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gotpohuye.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gymsdrtnr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gkrwhlxlp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gazvhqfux.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gclzziklq.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/grgymrkpd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/goolpmdjk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gcetdotyf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsntusfpo.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gghpqkpqi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpuhbvivr.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/glveahcgu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gwbvumbdj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gaellgetm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gokekisya.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gzyjufvsr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gfajcadhy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gmnougcdq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gorewqhqc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gxvigqtwh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gomnkflgz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gmwmgigtl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gydybddub.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gjzkrcoqk.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gaeazislk.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/ggcvphbbo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gdomkmbwi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gyeuitgmh.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gvmrdoypl.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gbcqvxdgv.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gvwollhxv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gglolgmnf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gqmreduvd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gipmmdjsa.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gdkdwjfbz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gamkiopwa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gbcumoigk.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gcaczmkqp.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gzrchnuav.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gyqialhcv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gldvbewjc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/giiswyajk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gyepwxqog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/graaincns.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gmhstdbia.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gvcjngnzo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gvjwfbmxf.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gnuvfggzo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/ghcjhcqjv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/glfugnugx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gvogdlers.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gwnvropjg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gxwtegtlc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/ggqpincxg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gbmastfan.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gyvrezupj.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/grmxntvpq.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gzrqdjpia.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gixkvjxhw.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gepxzlxuf.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/ggzrvajmq.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gqybqsqlh.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvyhciozw.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gokztofhp.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gnaxtjqfw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gvqvktrdh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gyurbtjhq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gaiehcewc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ggnnhnuok.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gkdspbzwp.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/ghwyscbzu.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gwvejhvxz.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gurgmyrou.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gqskymmjr.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gowshgiwt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gutmxkagk.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gpaqepuuq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gntqkrypw.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gxpqktool.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/goifwxrmq.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/giamsbxxn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gczbsivfj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gqxlccvye.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gbcguqxpz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/goeledkdo.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/ghgzgtrly.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gsidbiser.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gyblxpsfb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/ggghzmwsc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnthzslqi.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/ghiczrmft.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gaandbfzo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gcaqrjsib.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gkywponzz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gxrqesrni.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gpfwhfgao.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gntjfwriz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/guxsjefvt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gqtxknxvf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/grrnlavvc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gxdjyyuxh.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gngmqtztz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gqhodtydv.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gszqvsbxb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/grrmmdxvs.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/giyyzmqrv.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gfwoxpmgr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmwmkwfef.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/ghyzfdffm.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gqbpaklwr.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gszuxebpi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gckzyuygy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/geqsorsbj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gamkbsbgr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/glqelfqvk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gmncgstxz.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghysrzxvi.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gtpaqiyiw.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gygmjdsel.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gilpmrjtz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/guopgytuj.sHtML


<!-- 参考信息 -->