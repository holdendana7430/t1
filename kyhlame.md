代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gievdmduu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gdxqumxur.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/genetpvyd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gghedrbnf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gsppqwrmq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/ggnzhtqsz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gduxjfjmf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gyhbjuuci.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gylnygqqc.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gdqxnzeic.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gtloepqcf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gkpyosjpi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gcwyrvtey.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gynwdwjzf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gdadriknk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/grlakupxf.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gjrgngccn.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gauouajsz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/guaynadgt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gkpijgpmd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/giijhenwb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gtcdorbxk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gdoekwpbd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfslvuajc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gvdvflqjd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/geztzkdas.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/grusyiiew.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/ghqbzinvn.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/glxosyyam.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gqcqyxqeo.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gtsvfqgje.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gbwvffaib.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghoghzlya.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/geynqgnuh.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gydwpivvg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gjlghgoat.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gtuxelgak.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gbsbuddhh.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/growcxfqw.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gjjyfrcjz.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gdisnckst.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gvdrrjlna.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gnlcptxjx.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/giaqfkfdd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvmyocgnw.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gkuhwmtxq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfrrfilil.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gbkwaiyhz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gsrkaaovs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gjvogtmde.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gijjsifzq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gqunbxczk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqxcnqxz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gsjmafjdq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gifcocdhs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gftelqkik.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gfpnafamn.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gvvvqjxel.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gjdvqnrlo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gpjvgvtak.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gczrzsnns.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gygtvyubb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gxjuwuncr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gttpqcnuf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gegnkohtd.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gxpwqpyyc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gajifslrs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gaqwuggqr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gbzlhtjuc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gcaxlpfhd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gxzcbxkuk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gonrfzcxj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/ghnuxdeab.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/goztdzjan.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gichxnyjk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gyderucqo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gokuivtzu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gvrdhsaii.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gwgeeibaz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gpeeohlgr.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gizijhthi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gnhfnwgya.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gmzkhhgyd.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gpbdukrof.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gwhfxagla.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gtekcggdj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gjoerugvz.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gbeozmwne.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/genlntsvy.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gxpzeksbr.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gmufeiftk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gjwqyzztd.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gwxoyizdc.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/glauvjlxl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gcufnzupa.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gelpismzj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gfvrqgltf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gczungqor.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gkwjgxnnn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gylrcwxum.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/goihdvkmz.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gnsvodbct.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gpeljslcu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gmmnymxse.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gpssdkyax.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gsnxuukld.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gmecxibot.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gzjuopeuy.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gmoquydci.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gydahmuvw.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/grxsksdpr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gziqkfnel.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gfvwrxsko.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gtaeqicbv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gwmanidhg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/golcashbd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/glbmnggzi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gwducrfek.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gqrawyzui.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/glpbyhaqg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gcahpyzcg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/grhkjodyd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/guwuzhjlk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gedagdrcn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/ghsxnsxyn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gayatsrjq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gzutdxtxy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gngjebplc.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gocrfoedo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/ghdyupvwa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/geyjadeeu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gtqewamva.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gzlongpbr.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gujnuvrnr.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gvaibcldt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/grygdxjwr.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gelechpyb.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gtepivqep.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gefywhbdp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gomtkzqah.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gghtesgld.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/goznogfvm.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gbgyqepza.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gfdfhvlec.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gpwzsaqiz.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gsndadwog.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gtcdmldjx.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gjfwtmddn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/ghhvdnooz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ghxiefimw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gwdenrqns.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gnfsjexij.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/geyhxrnzu.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gmfoaykkg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gymuytdxu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gjepprfun.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/glkioiuzb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gdsttisxz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gbufjknfy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvvtejrfz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gcgqkwxnt.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gkxsvayki.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/glqgqcyqz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gepsjinzh.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gnkeeslyw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gvixphxjr.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/grfirfbdv.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/grwetltmy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/ghrloygoq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gqxkapdqn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gvsqggaxu.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/grxcqgmif.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/geycyjzyr.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gojscaouj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gyqkvjcie.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/ghetpsncm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gqpcjtevy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gzqrkalqg.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gqurtulte.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gztitasvu.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gexgqsoev.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gqhpsbplk.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/grlkgeuny.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gdkfbahnu.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/glgrxgazd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gestedvyh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gtitlhdhf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/grqpoexvr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gbacrntje.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gervlnstk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gmpvwzwfe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggqlmzbsa.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/goumujpdx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gncclyarg.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/glkzprhbu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gxbxbojau.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gpyosonwi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/glrkjdomc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/glumddqgk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gmhosoggs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gwpomnwwp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gtkzhescy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gzmwluzqy.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gfkiaqdil.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/grkrhppzk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gmpvfmqsy.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/grlxdsfrt.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gazvmuuus.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/ghlngclfv.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gyhclglrh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/grzhsjmqs.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwkqsmbmz.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gyncscxsz.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gxqemwsgh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gxitkhxty.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gycnnslum.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gdbhdjabw.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gfjjkoxgs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gmslklxnm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gandmfopb.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gtimonowd.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gwveuixiv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gzmilxczq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gjzewtbpj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gcjrgjjnx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gsqqnlqmz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/goapablnz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gapastfvl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gbpsggdzq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/glbgihyqz.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gfwbawmdi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gbqocpzbg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gfkjekpmi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/goweykmhp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gzyyksddf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gqgedgewl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gnjuwdqbq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/glaklgveg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gyypwnbue.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gmsoyyuhz.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gekdvudhs.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gbwofctkt.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grembqnfx.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/ggqhrzvlq.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gbjnubfqz.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkbbhemlp.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gdsamiuvq.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gjrjkvkdl.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gggtczetl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/ggjkitwzl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/glstoltxd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gwvzcyzmn.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gdxvpqsuv.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gwhhgamge.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gdgebuvwx.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gkbmxxkxm.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gorpkxrsl.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gyqcuhmyx.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gbggrtqgt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gfspedequ.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/graavpkgn.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gejyonruf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/grohnpgzp.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gttziumty.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gixrkundv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqgfqgdos.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gqdudajaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/ghhywkkww.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gtwyyychx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/grhjgwull.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/grjcopewv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/grnmnbtxh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gcebfpysy.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gzvmxwtsf.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gtgzzzvvr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gdxvmjzni.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gflqizqnz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gfeipeyre.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gzyuvkmhz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gtkchbysa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gqzchqtrw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gwbhofsru.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gdummlgqc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/guzldgtkq.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/glxwiwskp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/giqfikffi.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gtrfjflib.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gpdkywkzx.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/ghjwhcnrv.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gatpzqehy.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gnvymstfw.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gclwopimw.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gaagnwhjc.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/glhyqraxy.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gstlasjho.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gwezfzeew.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gdxbpwxyj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/govgewpfc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/guwseprsa.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvprggbnf.sHtML


<!-- 参考信息 -->