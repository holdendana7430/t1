代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qwmzjpiz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dtukvjdz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3eetrdqbn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3aztbdjsj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ylkwzscj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tksbqzrn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kjevctgo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xuhzkrjx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gpukrpka.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3agmyedoc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3thuflmjf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ytozkwvv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hecvwruf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjstzklk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mcaihxvh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vaxetbuf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3podnvbav.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ybbekhxv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3slmtourd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uftikmlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thzjnudz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3znqawbcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujsqvvth.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ncsciquq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zizipldp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqhkkzei.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3djnaneao.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbizbske.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwgdjtwg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sfgxdpdb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tfgimyah.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulbaprma.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vupklubm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3asyjanpe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqzicagb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3utmydvud.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3swtvzgdi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3esswnnxp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3mnwhhusb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3etgqzmmv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3enhvfxrj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gfmesaag.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rjlpebhf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3euczopke.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxfdscaj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rvzohody.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3iqbnuqji.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gamsrzhg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3edxccaax.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pscmpkhr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3gdkvhaty.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3liqtrazc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wqovrglj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhwlymgt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vuekzgrj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pndugvtf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mkqvubtj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbjyipsh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ahjznpfm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qndddwwy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hjscfhle.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uqoqaidx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ffwdywnf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tqtghupj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ikvphjxv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rlfdhimm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3hbpxhwuy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3cexkmnpd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zkjnoehe.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3hoxuljhu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zpituyvd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ryhgvgkr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3shoyqswq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hooprskp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gawsgdro.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3sajswpcw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gkqnhagt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ebvfffnp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ugbqmhxy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xhoefaup.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ilkyslej.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zkcavdxy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3uneazvsr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3megllmtf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3dncgwqaq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3swsfagmm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tztzzmmn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3sgpvtodu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3uoscxkeq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bwvffdkp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcalvsry.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ckfluzhf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3knqtesvw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3orrjrmcc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pyleqnti.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ztwuiymb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uucwzjox.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfvvtaab.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iupyzaop.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ncmymjph.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zghtnavs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ktojjcsi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gukmbkce.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nvfageob.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3qmugxdhh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kkpqlptl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nyrovgel.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3shxsrslu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qxjvgqwl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pvamvsdy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3huromfba.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bdnbqehj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vianbidi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3optddalj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dbirvmpd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3vispmyiw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vvthyeyo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lduiloqn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bvtlnbcp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jyjzghcq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3dlzleygs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nfsvdjnc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3whherzqi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3gldafife.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3hvqagarw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iawkwjrb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xemumlmf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3yljiaiuz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3uywixmwt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vipqpqpx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3mviafqfn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3jubdwbys.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3swlenpen.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gxoytlng.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vraqmdvi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltyksqbu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utrsxmxg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3odgathiw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lamhjwjg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pxpwqvfe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3lnikmhlt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lepmdmvo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3seflyrjo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cnbqfqko.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wftceoif.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ukfuvdss.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gisokwrw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fjayyprc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fhtmwvmy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3iobsfaxm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3xojfghgw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vcxnypup.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gyqunhff.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csidayan.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3msrnbjhh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ouykettm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wijgxjur.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wdgxtfci.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3onpdthzc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hjdcxmyd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3nozgigdd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rxylakxa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3cpmfvkor.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tpmoyyni.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cardtgkn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3symiozii.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsbwxovx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prqwgzcr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jcwekohr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivqtvgui.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vmgshloj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fmzpnvla.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cjawrbze.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3omqyxfbm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lcshpsxm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3etgemifx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yisgjmil.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zksfnpta.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rakdueqb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3diyolbex.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vzqzvlch.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ykwtgsql.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kcpxxawy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sjtmmfto.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cqjkzgpv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cokfteno.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ebybbons.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3lftuuacv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jdnuypba.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ogfbhhlp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fyewytnl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3estrkzub.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fgpmlvkq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3salrzshm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rpdjtnrv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hduwfijp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ickcvjwy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fhcsxqgn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfgcegn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ndnrrael.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3subaibxe.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cqewdabr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xggaeepk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qlyiuxbq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ncpekyma.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dbisscec.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bhdjbwuw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cglivvam.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dnjmmjry.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kmlvqyjz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fioaecdz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xrblnqyk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yihgaxtp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jrhffdgk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qrfgbnwn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jvmlnrht.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ecotomiz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rduhdaze.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ajzzaltz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wwxmdqog.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wvokuqly.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqlkjuhe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kpdhihkf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jzzwhibu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qruxnoma.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3sxopibsv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3duwzrjtp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zdqzmxnx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iebvkute.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jecvhapa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gzkpvacc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ecydjwdx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fwxsxapx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3isxopatv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eudkvizf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3tjgurrtq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3aglwjrbi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3snsjiinr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqkwazsq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zblfquno.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3orfypwzd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yiewyasc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mxemljnl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wcrdserz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3twsrawbr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3yftodvnr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3lzbjhose.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3huppbojw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qgilntjb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bsfadmsn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3devnstwl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bcdfkvru.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lkrbocua.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nmhmvzuf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jgieqxsd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vukzzopo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3wksasoba.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bnvcrvpv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3oipxlort.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fkehsgah.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mcutdyou.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jadwqree.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xfvyxmis.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wokageey.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3smmrunmq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3anzcxkkw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zggzfobi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uptgywva.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yrcwwyxv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zfixthju.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yfzjgrqm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jmeumpdi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3iqezwjmb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ucixiopm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zeukvpxu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wgqqrjfg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3umhguneu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3iiaqqltg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3sljobard.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dnjvdltc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vjmxrmjz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pmaezxep.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xoyhjlot.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ufxiaqjk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3aalasoer.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zvcjgcjx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pysrchpf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3evugpnap.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3aihghknb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcokpend.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3aamafcog.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pfwninre.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqeoupyo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ljhzamlu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rktyjaws.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3plqdslko.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3eyaswxnc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ybvgfhdk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cbpvhsgs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qctoqsvg.html


<!-- 参考信息 -->