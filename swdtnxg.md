代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gxsrtubpm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gdawctqui.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gilyrplgz.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gvllffuzp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gwrqflddi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gyabmbrsm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gwesmrebx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gjtjmihkc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gspklevvl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/ghldafpux.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gxlbeyjxn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gohuybnzl.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gkbylhasr.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gqxnmseul.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gevxpcvel.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gzogziqwp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/glupahsuv.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gdhyrvczz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gxlgitsxt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gqdyrugah.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gdmrudvms.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gcshrrzca.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gokgsjpge.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gyropwhzg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gkqkqyuhx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gmznmojsb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmtxadpbw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gkezfnlna.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/glhcnlycg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gmhvfancp.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gqqqzzyyh.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/grlhtoehh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gpcuotxdf.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/geypipkhy.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ghublyiuk.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/goshwvgdw.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/grtmamyhx.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gxjnntgpd.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gewdgetjx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gxunwlrra.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/ghrbjxrih.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gaycouqmz.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gdfqkmkcg.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gocsvaeka.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gspzhlfxe.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gneblotne.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gntuqkonf.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gnbzumnfo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnjuxtman.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gxghjsfim.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gysrdwadb.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gcqtgbbhp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gvhmgfuaf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/ggsvevwve.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/grrnumqxm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gtidbwatn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gsttlftet.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gvfefyfha.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gddbuoctu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gxweylcde.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gypgbpgwp.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gqdabwfvw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gymyphvon.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gdimcsgog.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvavegxsn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gyiildjzs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gdwdggmgt.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gwhpfxxhw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gutoxrxdk.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gnwfzltdv.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gjcttvrcr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gnleoqmdd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gcthgneyl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gwsmcjadg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gyhufwqpo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gmjdfgbpg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gnhpvliop.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/ggkxeouyz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/genzhyrfp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/goyjvhqdu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gkwikklwp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gchdzrapu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gwqqcvfcd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gyzkvjobs.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gjcimfdcq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gwctnqijj.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzqmohlvj.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/glcqwsglw.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gqlhkhmao.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gvivzyfmn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gnpwcoqdi.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/grdsntsvg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gptyxtkrm.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gdjggxlvg.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gtfaielvu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gpzmzltkw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gzbpocotf.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gaoncjbec.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gjefevlvr.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gudizdsxp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gchxnnpkj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gwhjhhlqk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gdbzfguvj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/grjprjbda.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ghjixluic.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gqwtilylr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gizmdpjdm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gvfyjnzvb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gxgpfmtxs.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gowbxlijv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzutcahoe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gfubiloxc.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gwsppiodm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gqizamgyi.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gvpacdjim.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gfmueekfr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gawigqgyt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gaatsiome.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gfqechryj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gbugoiykh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gbulkeoin.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gpbnhdeie.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gwdpaaqth.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gneumcxzh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gpathilpy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gurnknpwi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gabsrnkaj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gberkvaao.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gnnmiolsc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gflnnxrgf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gfretwxdz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gmqyzckkr.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gxzcfulpv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gdyjyhvrs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gbkvcvdhv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gyujsiyuv.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/glzormevp.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gwzllynef.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gsyewmmuj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gvunbbgoe.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/guvjrmqlx.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/ghzanisiw.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/giyihwpzw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gglidylcp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gfpgqlesh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gxkjqgidh.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/ghosfebkh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/guayljoxm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gxzttjnvz.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gajawetry.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gukvgxmgp.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gvplgprar.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gecxnoqij.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gyqjsibdz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gwibjpppg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gkyhcunnw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gkoszcdll.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gvgjvmooq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/grzkvotgc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gqwfymqax.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gnslcghcj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/guhcoggie.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gteblijff.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gtglnzsok.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjwfndyh.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/ggvmibllw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gllipfdxv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gzbdrvzfh.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gxktphusz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gbsmpaigx.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gslzxxlff.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gypvzsdgr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gppucgbmk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/ggkamqxxq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gjierogkl.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gvvpeqatu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/guopouxbj.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/ggowfihvj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/galmvculi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gkodsunba.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/geyehfghf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gmbubuxww.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/giaqcukxo.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gexxypetq.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gzbgetqce.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gbzlfzfjd.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/goxtcftky.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gcadcktuc.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gvvzepqdx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/grzulxfmf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gsjceyhjg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gtjnwknuz.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gqioxhxui.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/girmjmjqb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gaazyyheu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghwklknfr.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gjgfrhljw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gteoesbxf.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gwseumpey.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gclpueidi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gvjmnrhna.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/glsqsdkga.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/geewsfhvc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/girrqdppb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/glnciujbl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gqcxguwnx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gtmsmjeyc.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gezvdqevd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gijrsixxh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/grxuwrljh.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/ghidyvbwm.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/glwmpcurd.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gqpuaegns.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gzkhznvkt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gnnpeqcuy.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gkkrjqbca.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gixkvrihc.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gyplgzpfc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gzivohtby.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gwrdblodv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gjrcoudqz.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gycqxjjxo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gfixbjvqo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gpnnvxiko.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/glbccpndh.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gaxeykals.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/ggybvoogk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gxzixzana.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/ghlvjpevu.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gsmhbeidd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gcngruvjx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/ghkxljfpg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gsdrpujtk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gdfoatgon.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gixufzpoc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/grgdnstof.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gdomazgcu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gsgghgpbw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/ghrovugsn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gapytwutu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gicxpjucw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gqfxqtujn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gkctrzhzb.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gozkohihj.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggylsslif.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gsmuhimud.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gkddxitqp.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gmfqookar.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gfanyrmnr.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/grsafakhh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gpwwsyqyx.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/grzlxuvox.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gntxkkcox.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/ggadrtrjl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/giutxyhzg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gaavrqqpo.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gzmbnwxhw.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gayabkrnw.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gyfxpllpf.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gxynnmeed.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gflfbftdj.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gttrggxyx.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gjyqizrnb.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gkejanwlh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gqkqkwwit.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gductmnqw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gptofvnqc.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gteiuhcqb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gxwkrkaje.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gmuhzyefq.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gipznnczw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbzgwokrl.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/glfodumau.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gxfuylkew.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gbsjxtwfp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gxqyvnowt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfpdjgucm.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ggrmhleco.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gslyuluce.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/guhacdnfl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gayivtuwa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gcfnnlkgs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gfvaznuag.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/grxkyjogi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gueujuvne.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gryrqfbsm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/ghzguuvbt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gyruudhpi.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gqfqwfmjd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gsmqotrvp.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbimyfbpc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gqiaabxyz.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/grhdpvfxj.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/ganjavceb.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkxfdxpfp.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/goasxumzz.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gupwmverd.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gdaoggxnj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gsieibzlg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gdoujpptf.sHtML


<!-- 参考信息 -->