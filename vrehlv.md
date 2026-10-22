代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2sraguchx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2orvcougj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zfpmycjh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2iabiqjku.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2crgakphw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2quqsxzmu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wwdujhph.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yxzsceua.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2aokgotvv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqndanbz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ewwnyfbu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2sxewlrei.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2otxgsrpx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xiznoobv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmcfqnrj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hacwbuvz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2muzzgpeq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pdrbheji.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2nooyuwsg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ddbinidh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2foevdvrv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sfrqfdcc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rqxzyuwa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2siwftuhg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tslliycw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjhiocb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vsmtcbue.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rlkfwdql.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulppamyt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zpjagbqp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nrlxuzzd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mevkmpgt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vyskulez.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cwsdldmu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qvdzegvi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2trfcnmwr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wvkscvpx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2orncsgxc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2haxlrbjh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2eoshqdmg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2sgboxiyb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2cestlaxf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2okmzorov.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zohjfdeh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rpxstzhx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vficbfqe.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kkfmxnxv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ollplckj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdsctamq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dbevgcdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjzkkcic.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hqbudrqt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fsbqeuwo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkeabieq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fkyqkikt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdbcpewm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wsdmzrrf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2masfbfaw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fpqlwvbg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dchhcqbb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bzlrtuhl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tgcrqpyf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jmcqihqz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtcnhdnl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntsklove.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mtgexgqh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gdvhhmuk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yyavnvqs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ikyplfro.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lmsavnef.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vkmkuwsu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fodjmtpn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghmzatpk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjzpabaa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfyscqjl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sbalegbi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2airgvpts.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2oactuwjr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yfjebbgf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yvdeeznu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qcmohlbd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hbwyrcej.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2blhjqzga.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2iohvtzvw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nlvmeoql.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ssxtiyrd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zinsrqvw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2tapbsroy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lrxgjgvh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2xloyhsad.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2knlpdlkl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ttlifsmp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2foxtflhi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rdjbeouc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ssvpcwos.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2abftlitw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iwcssfmd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2nhudvmyq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2irqarhgp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ohcadsbk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pzlzfpsy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zsccneir.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2krnxbmgq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2tqmqduem.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pbhbnnuf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2qzxkpgfh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zekyyjra.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2posjhmrf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2aiyxlfbs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fkculihv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2qncdrbqr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ooknglrd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jmdnsjte.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2iilxmsso.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ogilbaur.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ciutqgqb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhcjcppn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qkyxlktx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuudzbay.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bqrniusm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2niqfeuoj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bmunppee.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ugcaccxl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qsmpaicu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wrtfygvz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2juimqhcv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dagtmjih.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pwwcmsbi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmhwepcx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zfrjueun.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2soatvenq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2udbcoqss.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ellafwxu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2umzpeeof.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mzkkgxab.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iogdfcti.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2idhdeqkd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mcvzbabq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2loohstul.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2layuvdcg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wtiutxqw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2veefmvoi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ohplojju.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xtalmypy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qcjrzoir.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bhlztpoj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hhhfbvsk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ysotdpbs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2eansqipk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vpxqhspi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2meyqshkh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tuwwltfp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2bzydthfe.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hblzwrhz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kaqpcege.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ehmnkuqv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2akijxdal.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xcmxqkyr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ogizgejb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hilxqawu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rujpdidc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2maddogko.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gbhsmfxr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2veziyjgk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfnjotfg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2smzzaizz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mkjsxogd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2prpvzrom.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qwcihxni.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rehfbfsx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bknsidza.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2efrbphow.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nxhzhtpy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubtibnuy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uynaoaef.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sxvxsmwv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2iofpnmfp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dnzncnwm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mdbjnbmo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fcwoeywi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2clsqicvv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djdnrzpm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2umvzyzav.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2curujovv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tartafmk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2abgydoyo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kcwrlaed.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rkyskmlo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2arobafmf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zzkrdqem.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2eapxxpyx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocwlnbkz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2lbxirhyt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mnlggoru.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kzfykniv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpuxkxhs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gzhlpzkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwffiupn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lqacdawc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fwzrjyhz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tqtdxilu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uaxvxjgh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mjhznzry.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fmvxyrow.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2znftlclo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2myovqcgc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2akgcdgbl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ucfelvkk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fdyiiuow.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ljbdpgub.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2grxlhjmg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hhgcqxyx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mqbwgzfz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2iinqbbfu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mmtqinqk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mvkczkmn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2swgskvse.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2awtsunhg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sknfqpvx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rpkyvptf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ruposfhk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lwbrgslk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wwmjzfxx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ghlqgowm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rlghtelj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lqyboffg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2clbtnyuu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jsshbviy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kljgwofb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gjyxkeak.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ixgjzarw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xqxsxoal.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2foeavmhf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2svwhynvk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wtjikynq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eihugirx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bqztdndw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uzdrvehc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vqwwcxip.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2alprfmzv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qeipqnov.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jathjwit.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2havyfoxu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dcbvwfvo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kbzewvju.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfdjlebm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ttdllmzv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fzycwtkg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jzggumkd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrbdhqxw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gbzofaqo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2krrdykzg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xljbddwm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rspzdlwd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sxvaymep.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nggzweqh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qccqfbmc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aumczdpa.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2drtgaons.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dwrvlwbg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uxfvmzow.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2bvxjyssl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mheiqmns.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wnhvvzts.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xzltzjaa.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2gzuubwtj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2etgwejlo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qgejxitf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjzteguh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ubxpepha.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2weglsklo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2icutizna.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ultbkxsk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xnvupvvp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zprrwchb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rxsfqptx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dgvbprsz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vllaupsy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cslkprgy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ewsrpnen.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ipcyqgdb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kzknazvb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2irxrruvd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ycexwete.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2aznlucow.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ptojzstz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xpxxnblj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2obdwzubc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ryioxbme.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ukfkqqib.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hdvkeznz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mvsxbnjh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2meeldxdy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mvogkncd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wsmdxiwe.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pewzvetm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tfybymcr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2auuhktdo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ueoowgzp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fyqjvilj.html


<!-- 参考信息 -->