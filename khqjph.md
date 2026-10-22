代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sjxmoioc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umifncrg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qujkhwin.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tnrahqra.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sqjhmahm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ugevligs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ohfvvpkn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fbhibikm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2saqbjmlj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ykkqccci.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fzrztysv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iocyidjt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mfuimypu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dupspxha.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pptmbxbj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ltlmavyu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2xqvdidfx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogxkryge.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vsgrdjdg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fuhbgkrq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hxnwpvgn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2aoiunamm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2zqeynxrg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2voxvxplb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aaxjniwa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dcymdloz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfbddscq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lnxkgfov.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2tdsgcvca.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nzozqfud.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qizuuvez.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cywyfvpb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxpxnhrw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rimtrnxb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rgbweeyx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bbsdauhq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqiqkhsa.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ncbxidkj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dprmdiab.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rvsmuung.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qtbzwhls.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2bfosppga.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2iplxbnku.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2exfnjzyl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2yqskgchs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ikpnueom.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2kfhojnlz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nsmkvtvo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cwowvmej.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iqhctyha.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2undgoims.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vjugzjed.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2pfzqnetd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2njqtrdqc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2chvhqmie.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hnvenlvr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgoskejj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upttpvjg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nyhunozo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rundqdpj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ucebizjk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qexdhkbd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2icsichos.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wcrjwanb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kjimpbma.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2twklsqhj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pguocwsr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wleazoqw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wauvcseb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tcrrbdeq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fxyjkvhh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vxhxkekg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wdejwetl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2csecyvlx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ajwdsefk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ahqbssun.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2scgncxvg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rwicexjq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yrlreqzt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pwbwzpyi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hheiycqv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jubgnbjc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ridtcpts.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tdiefhtb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2evvdbbra.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2szimnrfa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2aoxpumqa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2buybbsvv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uzsdmmni.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mupivikj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ipbjiyqb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2cwdqppsh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cirsvyuq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2royoflpi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kxnfanhs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cdzkfhwa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rcdzkogi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2umwbjnqu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2awqnayfg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vwessvub.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cauymdxd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahucnyhk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tvfduykg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vtotfnoy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gkxmiypd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cuxbmpeh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wdvymtkd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dbhallgo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ccakhyfn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2iaotpqsc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nqojqlqe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jcbuzhno.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2spyzzwyi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lxgwtitk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aohopbjd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cubojaii.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xrzvfswt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2oyexjche.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dmtvigbb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2owvdzese.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tyqnruer.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2veyvxvip.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yrkcquhm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vmuunjur.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lqzgbntw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2whyhujba.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kzizqyat.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fxbitsyx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zjltcgnz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fmahrdhe.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jdahasmm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2etaksjii.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2laykelot.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zttjuamq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cyfowdvl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jlavqfie.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dphtgomf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueiinskc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2hhancmnk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhgednbk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eixufcdn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jrrqauxi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dvfrxitq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2cenfqhzf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2oduwfiqp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2tpafhdct.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2twrfrrtb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ecgnmqjt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ipeiwjdf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lakntcow.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2afimigsb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rjsmfgqa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fmbvvoqr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vheytkgc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kheobmii.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uimapzrc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fnvvhiby.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2nfveqira.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2diauzlkm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mkavvnme.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2aqmurhvf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wdcshoov.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2leubjxdh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xlycwulr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cjndttkr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yjsfvell.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zrelmwxd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kogqelbh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2oncicdiv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vuxrmptx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cxmtnrvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkjvzycr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pklwdzqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcocolbu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yheahkty.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lwjitjla.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lpaxohfw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qenelgyi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2knleewwf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gzacgzsi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qoumdfdz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jxwaexeg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gxzbgabg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ckqxiyyk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2vdtxnnpa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qjcfaers.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2taawzbnd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2agyyurjm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pccsxaeg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ptgrdysx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fqcognbz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hurgioqe.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zblsevrd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zzmyegjr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xvlcghoa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2henbafaf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nodeetlm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mglecpom.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kgginbrd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bbhcnuwd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xybugbgf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pvqsvmqf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2auriieqi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rahlntyv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kzlxddch.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pelvttph.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mynuioec.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ljtsblms.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2sqhyjsux.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kkruqqap.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wxchjuui.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ajxndfdr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vfimczvb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wlakbdzk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ecuizkgh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2sbbmumpr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wxisprwn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tlvczusg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kwnrlqxc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2opyohfcl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aksnwdid.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wsstngkt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cffaejem.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jactdkvx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2hztwecmv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uwisvsvg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2skehxkwq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2oazcdopw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kfcdbcmd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xdaybdey.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dimwnfur.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2stojqmfi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ewwmrbkz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dxsjqcjc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2prfexroz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zmpqgqiu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tlqkbpvf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fxsbpspo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jramammz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2couvxnjf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2okisyssm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dzonacpu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zsidpbmb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hwrwckix.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2upffegnj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2guosyyto.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lqdvdxky.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gbsungbb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zqevscix.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jzlqpoev.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bjduvpqn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tbjvuwyg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztbpzivh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aacbonkd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lscmcexq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2gerfcliv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cadeyort.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fwrkvypg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ounvecpz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pkbqhhiy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qccxdyef.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2frarvmsq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tgavmzgv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ylsbvfct.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2oddnyauw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2eymhyjfn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcjuoaub.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pxhqomgw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nsmzqwmw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2toyjxjuk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yrgmxwpx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pvnbjupd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2awekttab.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uqkhukbq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zpcodkqk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oyjltllb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2paltusid.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fnelnpmc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2yequxohg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kksdowjm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kxdocxqy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2mktpqufl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bkcxivyi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2efihfoag.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xohmpsqv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfgpqxt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wxbrbflj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2mbuijghq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2oxpwwgch.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2fyjphfqg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rakwvwci.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wmuwbemk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2omcyuksa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mpnovefi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nkiupgci.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stmbjfba.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pdbfclcd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ydukcohf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lunuysla.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ubzbrnzp.html


<!-- 参考信息 -->