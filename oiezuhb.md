代发 wailian999

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gelcuakxk.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gdavjvxkh.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gjcpcvbsj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gzvmuzapi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gcywnrwuf.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gyafjtlfu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gbehaaxrl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gnpuydkwd.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gubkzrdir.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gujienfra.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gmfgmkmvd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/grbrhsayh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gwrbfwput.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/grdsvmlou.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gwctglqrp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gswfyrwkh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gpzovsugg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdhhoozmw.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gnafivlit.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gdxfwhnni.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gsniryieg.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxopfzcqg.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gmqehbtff.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/giemwmmfx.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gdtbvpanf.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkbnrpwvr.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/givflelam.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gfyxzloev.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gxesrjykv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gcyhdkynt.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gxihhqshw.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gzpifhjna.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gkkhrpnky.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gdrtrihoy.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gdkjtdkyf.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gukamtspr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqlqhiwit.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/ggwtkvgmv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxcpoqyov.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gduauhtzj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gpcicuvml.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gocqiwoqe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gezxtsjku.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/guttkqvml.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gqhyzckow.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gimxszxnz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gmureqgrh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gnsqwpawk.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/genuauudp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/guwvazytv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gpkliwanu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/grziknemi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gupptyixs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gdswlkymr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/ggxjebkfo.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gkxogoekp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gvlvmkxpu.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gsrpnqeoc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gfivknmsn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gtzamwxdr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/grcowlvrz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gwhibdqvi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gedjurwsv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/goqqcivpp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gipfhsfwf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gdushaxgj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gxopvgqdn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gabhblvys.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gynndxpji.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxyzjdnio.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gdhmxbcxg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gegzmukbr.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gijglbxdc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gcitpoptv.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/geesqlmkz.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gygterict.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/giymhacid.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/grcwdhtdw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gwiaxuzfg.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/geibaxarp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gedgqekwo.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gevsiufqb.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gviawojfl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/ggvsezldr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gjjwtmzet.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfjiogw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gddvlxmcy.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gamvnjlur.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gfkvddlma.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/govdtchaw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/ggbkzuaug.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gbnckabgz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/guakcnjql.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/guumeclzj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gqylapyur.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gnxmavdts.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/guwumpuxh.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/guvrrctzn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gvehkztmg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gwhmrdngw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gorqerimt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gpemihnsb.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gmltbjmay.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gakylqqop.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gpqfmnioe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gpuzkzuez.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gaoqcspps.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gsjfevyho.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gtiiweute.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gqmhlkogt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ghcrotcqg.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/goadmqxih.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gtbfplepk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gzbxpklkw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gajvaynzq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gqijlxvcv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gzefcufji.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gcvmnphfd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gpldoxaks.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gozbrazdv.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gualdopif.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gsixnbjag.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/guyuvvgao.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gxwytqvkg.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gemzokdmk.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gebmlqxjg.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gipdiowam.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gfywmnrml.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gbgltufuj.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gcbjditrn.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gjvkjzcur.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gzqqvgtru.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gwnrluzdt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gedtwnazj.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gxbtriydx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gjfqvzipu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gnalphgvs.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gauzrhecu.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gndskbuuf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gonceqmqj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gqoyxxstm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gyvzeodwt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gsqcbtdiy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gjenedafc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/ganzpmcwl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/goexllulk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gldmbtxfl.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gcvorrqyr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gsddngufk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghldxdolr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gihijexjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gqvmdlhsd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gsdgposjz.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/ggoehcwja.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/ggvikwmcq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gcdgfhhko.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/guyiopjqk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gnioauqyg.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gicvjojxb.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gvncpxlgh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/ggyxfzbzb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/ghepdjcsc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/golgafnsp.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/ggzfwriog.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/ggshmefsx.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gkectvahz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gqgpevuge.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gyrfjyeyu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gwneozbgt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gtyodibwc.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gqyjcumxh.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gsajwghhp.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/golhlysio.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gnnowabip.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/giolvsder.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gknlxkgwe.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gsmuuydvh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gxuzimqjx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gkljwhqeh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gazmhyrri.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gdycapyih.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gsrjeqcpz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gpwrjvuit.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxgpxfmxj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gmqlrexqy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gafwukuok.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gjlndehai.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/ghbhayqbi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gctosjefq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/goypwhgfy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gfjqopkfy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gmwyixmrv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gjkdolhfl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/grbdyifzi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gboigxkzz.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gwlaxgkgm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gdmqzmcsw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gyhrldvya.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gowuxpsaq.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghxmubqtk.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gtblnmvfd.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gsbdyuxmc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gashnefzw.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/giywrqavo.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gwlvaqdrz.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gqtqjibks.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/glawmegii.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/glrtwhtvh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gvgqvuugs.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gflytjmku.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gquzalfmi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gyegrkcuo.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbrawrlyz.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gwkzhalsy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gojpoaxkp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gbakiyfrz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gioyffxea.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gjbvnvznu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gxjnwaiyv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/giopnhzce.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gtuxscryb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gfyyawknu.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gmwcgyiak.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gwrnuvagz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/giupxsczg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gefelfavl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/guywoopky.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gyrozjanx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gxgyegean.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gkmphqzbe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gaesgzqpy.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gyijvzjqb.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/ggmqjzlno.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gssjzgjlt.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gznmqekkr.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/guarogmfm.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gsfqjrxmw.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gcpuvljdt.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gtdxhdnda.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gjelzmfth.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/grwonnkkb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gdmzfuyws.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/ganhjyygi.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gecnturip.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gxbrtjqgk.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gvjmneexr.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gaoyiblgf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gszwgxbbm.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gipfoxbol.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gueovdklq.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gnpsabxxs.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gudloyaor.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gbsonsgud.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/ghpyhcbqe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gtfwargij.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gdcfvcdog.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfftgztzu.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gvghnusqt.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gctbtwtum.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gldxqedar.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpodzzsbv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gulmpdxyk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gwphixoip.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gaxzuuzku.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdrpftcit.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gwotwvofs.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gwegbejzj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/grbfzeoeb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/ghjvxzmtw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gggzwleyo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gtsyijsdr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gnntyphgh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gyjqiazyp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/ggufwfzbs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gwzuxjnnk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gsydvbkvy.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gaoyjanrx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/glrghhkvf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gupleksif.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gbtrqqdpw.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/giapxcaus.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gwanabxgg.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gqusowoza.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gfbioqqbt.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gxqajzffs.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/ghnsuthvd.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gzazgwggp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gjqqhnugr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gtrarkizh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gykkfywjv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gylayiriy.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwhjqmdwj.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gyhffvqes.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/govnckdfy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gqodsnxfx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gkjkxdlsp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gwysidbmx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gvvttlsit.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gvmbjsjdk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gqfcstkrc.sHtML


<!-- 参考信息 -->