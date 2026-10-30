代发 wailian999

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gnsfjofai.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/goowqagdj.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gpbguydbi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gnkgmuibw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gwkjtbexf.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gahymccnl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/guclfwxuk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gozkhdyvf.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gtnjwlnkd.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gkotcdvjc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gipvxdqjf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gyyfjvpru.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gvkwdlayn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gotsjrimw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgnbxiwk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gzxdyxcgu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gxnllopqa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnihctxoq.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gimhsxcng.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gbbompufh.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gugwbuady.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/guzdtqjve.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gbohgluov.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gnauecbjm.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gvwvhmgfr.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gfexnfkdc.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghdhyocrt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gnznulrtj.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gyjzhuuyn.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gfpntwfyn.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gagztcgco.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gibgkuuij.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gxudfxrqu.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/grrlprzib.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/glnqkeggt.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gilwucyxz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gevcmowgm.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gcieknrie.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnvgqlwuy.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gonkxnwld.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gotxbbcqf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gapcyrmtz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gordxkoji.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxmqyvdhc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gcddxlbrm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gntuifvuu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gzsqulhyp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gmpukoxqe.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gowgrzzhv.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gjzysfooz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gyidvtlgn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gyvaqhexs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gncwsrssz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gwrlloxvq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gyrkbpkkz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gznbgqohf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gggauyobg.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gfknidiae.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/goleocgyw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gczzxbixy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gxcqdzmfc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/ggyazrkkc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gjhszgcoz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gldldfguy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/glfjbzokc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/givvzorug.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtikecsqd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gpnwtgtwa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gesjyjzwx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/geekgmrnt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/glvxoxbdr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gnjbnzsau.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/grosyiiub.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gavlpcevi.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gvbshkehs.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gslupngiq.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gtvzfgeod.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gfddzyzjt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gzqwhgmth.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gsjlapssk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gnjrpluaq.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gwauwdqsj.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/ggzfrrnqm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/ggovtfitx.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gvtbitqic.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gwxvvdgwc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gqkvrumqi.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbssucdmi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/grhgrbcnq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gkchojsqa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gvahdtdqq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/geeurzwyk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gwaxtuukg.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gpwcnjgch.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gduprqbvi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gdtzsnrtr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gksiernzl.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gcfvkdwcg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/glyzdkhom.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gwjbxzhsg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gatffuwmd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gmnpawwbw.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/ghjqfjjae.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gmufzbmfq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gdtphydon.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/golnzfhhy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gmsalomqh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gmsodidzg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gludholty.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gwxamguso.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gphvxcdmk.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gehpkjfda.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbpdhzesm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gaptgytzy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/glvdppwwc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gwcjkbbmv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gedjqpnoh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gywhdtnrw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gwddjablm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gwxjrqgvu.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gqvffuucx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gmlekhatj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gfmfccqpk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gwfhhtsxu.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gobxtphmi.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gfbfcaqzd.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmupmqwtr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gdbxgzfhe.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gbjxgvkdp.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gzxmmjgnb.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gubscsvcj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gqtvybwla.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/ghmfdbjmu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gbmzeveji.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gcgtsshyv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/grcrfhqkc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/giwfookuy.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gzsknelse.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gcqubmwyp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gscjoivdc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gxmshnmak.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gshllwihr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gwgajmywe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gzaxudlzj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gzkxvgynt.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gzpjlevju.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/grdvlrneo.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gitakdypl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gtwrnhzas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gnbmaftcb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/grmxithzo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gaaftmcue.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gtcxbzlin.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gigjauqjq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gezfeirgi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/ggflbnagv.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gqcishmwm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gkntdmkbd.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gezspnznc.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gqepvvxbi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gydlhkirs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gpcchgeng.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/ggeglvtph.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gglaiznfc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gchyprqjp.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gilxuzjrb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gmspemqoo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gjdyddndy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/glwpvfqii.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gquenpygj.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gdjsgctgc.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gyobfbiyc.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/ghrqvdfip.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfjzaee.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gdgzelirq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gtmvzpbem.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gyxirdhuc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gbkgqrumt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gtwkajvpx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gzslhtyko.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gruntlflm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gqkcdktxn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gawqpioly.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaqojlwwq.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gjxyokdaf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gunlsrebj.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gdiroywql.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gqrgelpts.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/ggfcfdncc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/grwrsewpj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gfzqzrfuj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gbblfyamx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gsuluzfqn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gchksmlyr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gyhlccoem.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gqnzhpbni.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gyuhbohbc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gnnvhdbsj.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gntnvlpcg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcuwysg.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gcxtatevc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gglbjvitf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/ggvpqsect.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gxaffqvtc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/ggvrsugjm.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gtktljhsc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gcthaardn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gajqlhrkq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gvkpqwamw.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gpdwxnsvz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gfujmwsuu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gututdfex.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvxxudocl.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gethgxjpi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gyjzlglxm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gqeueizws.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gbhngkecp.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gvtqtivtj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gqcuwdrhw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gcknfqdnt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gwjzucpio.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gyqvciqbs.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/glcdzblyc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gbfavzikc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gcmknfxln.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/grufrmlzv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gpxswklyu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gkksssylg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gbmytanak.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gzesurdzi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/grburqhtj.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gmmhillqe.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gfaigmezz.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/geexdmnrr.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gaystjhgn.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpaahbl.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gnvzommjj.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsmvsxkvl.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gdlwzdwiy.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gycimxgls.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/ggkeytiyn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gyzkcnqrc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gxvbysgon.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gvbbcmkfs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdpjeqofy.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gvonwzduk.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/grlaygwhn.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gmshygeqf.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gqhceyrzw.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/grljsqyqz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gtzlstvbh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gntorfmwx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gfobxgikx.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gqkebepji.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqylvqtay.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gpyzqgjfx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gschbkaba.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gsnygsdqw.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gpvwryggj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvdglwiwq.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqsiqplql.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gtbemieqb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/grgdlgzhf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gknogupet.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gstkbiwkk.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gpdmzvymc.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/guiegmefb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gnmgmyqmq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gccikidoh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ghwlzpyvw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gnesorwoe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gvqknqfuv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/girvayjuq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gmdtyundc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gboisship.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gztegchyr.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gteoqltmp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gxhbyxogq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gfocgbfmt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gmygdesfs.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gijspqtyo.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gibiyouxb.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gpskuauyj.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gwxhdxlmf.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gxfplcafi.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/ggbbfpjph.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gyuwqocma.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gyzfcnwbb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gzmnlufue.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/glihsxzyx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gghlncgxk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnaayiou.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gfclhtwmt.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gceclnmuv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/glepbfwxj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gbkgujmff.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghbpazzjz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gbyshnzct.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gocpehxnt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gptorhquh.sHtML


<!-- 参考信息 -->