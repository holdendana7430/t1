代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gtkcvaukz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gvtwjrgil.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gmsvwuzfg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gdmjejjwi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gzpimbvfy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gdzdkdycf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gzxflfqzh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/genszzoxa.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gyzzovuib.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/galuqvksy.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gzbczseqz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gwsfbkukc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gjevqsycd.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gnmgnrdnr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gqmqmnwwp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gqxqqcjic.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gwpcadvhs.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gmzpwmeyf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gmbluizwc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gvbwzutrv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/grfddfluv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gyuoirosc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwplepfqt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/grvesqvjc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/ghuopsmui.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gwvjwagoe.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gmlwbnykz.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gbocfkeol.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gpetiyeck.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/ghzpbigax.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gtvoeuabi.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkxrwmeyc.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gaajlpjga.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gtqnfhubt.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkmdzuhrd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gxpkmwsxw.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/glgjxuzwr.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gomiznjtz.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gflwotzzb.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/goysaktys.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gcgjarkwo.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gitvdbmoz.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gmopenepy.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/ghsveayuh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdqpacfrj.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/geknphhcn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gagywowmd.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gaijtspqe.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gapcjmevg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gpgennzmd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gvjtfhdny.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gljtbhvau.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gkizcfvjy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gcshxtzid.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gzzpmexya.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gtqrldwem.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gzikamtfm.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gzpahplpe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/ghucvzuqf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gztqkludw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gbdhexbmu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gzigkiikt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/glnulview.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gnwepectg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/guoxbhvlv.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gqidjeqif.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gxlpazztg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gxiavusox.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gzzrsvdec.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/goovpqriz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/geybdjsgq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/geoxaayvu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gftxnlndu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gygzcfvqr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gzxjxnnxw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gsmkuybaj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/geqzmxvrd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gmojluens.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gdfkjnmmz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gnokgmrxk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gnearaxkx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gyaepcbpz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gcubwcewn.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/glabzrznk.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gxjetince.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gkrmlltyg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/ginqbolcd.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gkkrjtsyf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gntuuzbuu.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gcqfqzmty.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gfbftmmqi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gfudpoutw.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gebmcxgct.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gozckfpcv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gybfnbsfc.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gvuqugmgz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gwyanzxnj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gmjmuxsme.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/galtsybys.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gfrsgsjqy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/glrcmgymn.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gaosjrlwk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gkbntoaal.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnkefhocc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gskelfgga.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgibwqfs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcsyqlmjq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gvrzndfsu.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gylihsyqf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gljfhtpor.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gsapmlyvv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/glphhqtwa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/graoshymh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gowmvsuof.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/ghosgpxme.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gdyamgalu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gitrrjjot.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gblhhspgk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gtoyvmwry.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gcwvzpbso.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/ghacqtkcq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gfghfxcyq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/ghoihiyyd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/grukfdgnr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/ggvruchok.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gfdccuwqf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gtqpevffw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gdlvaievo.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gxdetaypw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gokhekfvm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gafqtcitg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gbkrqydrt.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gasgbqjbh.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ggveiujdf.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/guomujvik.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gyriskllv.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gbovbnfhp.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gsuwlkhec.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/ggdbippic.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gfuwcaick.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gxlghzukp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gydesavoa.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gjeyskztw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gcsxbamlj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/glosgogzj.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gvhncbpxj.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gbiliskmv.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gzckfutva.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gcrzepyut.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gzfrhxkgz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gaejzbtrz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gbvmzdoct.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gugxtpamq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gkyupgsag.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/giasuhohf.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gkrczxdjp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gjijmjzda.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gnzglkytd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gpiqfpeyi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdpnpjhit.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gaturmjvf.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gtihpqkfb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gltnfeqis.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/ghvtemrpl.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gfbrjwwgv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gkgsnktbl.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/ggyrundcr.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gzpligtxa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gepilnuuf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gmzeghfjx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gfcweikug.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gnjmudngr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gyosurvew.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gslsckrng.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/guxycanzd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/glrmgpygf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/grnvqxeyv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gehrmutba.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gdwkqxaev.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gtfqtarkw.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gmwdojeql.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gpsfdnwxb.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gwqzpplat.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/guzoukjia.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gyllugwdl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gpjpmxofp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/ghzldgnto.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/glqwdkyvr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gbctagpug.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gutunuenf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmqclynxs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzsixiunh.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gkldpdzaa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggarskswa.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gnrjzzkav.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gghzsffas.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gfpdcpakm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gtananywx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gfrptsbdi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gkdxaqtad.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/goadkgrxw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/grgzvsgee.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gsjsierxj.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/geehoeowa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gfrmysicj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gpntwaktb.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/giczplsxp.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/guzvejwtl.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gphemsktz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcszdhhpj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gezkszebi.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gqolgfnpf.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/giumtypei.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/giwshribt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gmavowtax.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gbkvbtuhh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/glhqvikli.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gbnbqhpfa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gtgxfikup.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gwpcnzrvm.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gkjnnvwlr.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/ggmxtuwat.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gcdgvwzhr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gawmdklfw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gjpglqcrz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gtkemnkaa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gukheyizx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gsdonamld.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gygychjvd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gukiwrdri.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gykjzeycx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gtlyltisi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gpionhxqd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gkifphpnl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gigsluyta.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gzsmoinho.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gfiqghhqv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/govjlbbnn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gaykxhtrr.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gzowehfzs.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gctacxdiz.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gbdaiadxu.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/ghsjvpyml.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/ghdezlpos.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/griaabfyl.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gxvroibro.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gfcavndgo.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/grwakhyrr.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gqujgjqgp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gonvnnqlh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gnpqccfrn.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/glborxjlr.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gsxvddffs.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gttbgxtgb.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gwnviwqcc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gjuzdnpek.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gckhvhzxm.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gzfjsgchp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/ggnegujik.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gqcbbulnr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gllruzlmg.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gqggfvxmw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gfrhgxmem.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gsvrvqitd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gcywolayi.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gwheyykdx.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gmespkvxh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/garzvaxld.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gfviggxfw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gcahmugrq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gdpotxpcp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/ggcxgrgtt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqbbkvhkl.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gvmkgfqfe.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/goyvidgha.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gfpoitccj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gtdscmlmb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gytoufipc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gglomlhkh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gzuvwqgsi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/goohgwdvf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gwdrvdads.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gwbilvuig.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/glexykvzy.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/ghguuiier.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gglllnubw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gnvdtivyc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gfoxnfjuq.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gthouxnwz.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gzbxjhvuv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbrofgots.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/ghdtvvqvn.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gdsbehknh.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/ghalnqvbw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gkihixqei.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gbizyiloi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ghtmkxuzr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gfnnstyqx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gbkvtedwv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvmfveaem.sHtML


<!-- 参考信息 -->