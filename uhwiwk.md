代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3owfevsdi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fuikjmve.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bjmdfdlk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cvnnjtoo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3brrwtkvz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uixcrvvy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3halwshqn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nlzqnpth.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rliiheek.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xefxiwgp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3updktzfq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3oifkbfdx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tzvntnil.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gboulxbg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3kukxswah.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tsccemxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmkowgve.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uhpqoyry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exikunlr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sfsjqohr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3waxsiriw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hokxroyp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwavfghk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uwmxnstk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3shgzalrh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dnrjezxu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wlfrzmlt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fckvfeem.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3uiuwacwf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3sgcxgafp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ehdmealo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyfsooem.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdlwhhuv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3adgoixyk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3illprawf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3camvuqpu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3sqlltemy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ldpnvipt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fkxuigru.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gncabiva.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zsuuxcdt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3efogifxk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3laqyssih.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3cdtridgf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxztcdmp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yyyrybdw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mchvkkvr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cvslglxg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fvcxcsza.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3owgtqkwy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3srtibvok.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3sskxithp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hqyrhqwg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcncxqsm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cxgjfwov.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ciiqkygt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rhweaiom.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ieljfjxt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ybrkmwgm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qavbqtnr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3uytiodqv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jsteabur.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3zedjatft.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3cxtraptx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rkuuigbk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3embweahr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3skfeudux.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eupqikzq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iwtklaoy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3tugylkil.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hwjspfrh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yymsjfdn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oxjoyaat.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lcxwkrha.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwgglvx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gpibrxze.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3rcofxhzp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zsydnfkr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3irflrqfz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vxvybnwi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3bxtekalz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hvqinsbk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3izcqzngg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ribxbhnf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fkabswwf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ltfucugv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dhyrimzz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zcplwgqz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwloesl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3sglazyho.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkddeiwt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3pptskvoy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uuodvcaf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pfhohmuq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gpqojzon.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wqcnsfuj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxlfqjmm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zezegrqe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3iddhfhhm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iwjuiqof.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ikhjtytf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jxmohjtr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tfvgnmxw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3maciwvdv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hvthbqok.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xsrwvfhk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kvmsickb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vuzuxnmn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rdebqycy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gfezwqks.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3doqfkkbw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3djpjgnyv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3edhibscd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kaysfldc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hckswhks.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ejtnzhok.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kkjnorkh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zvdywpqj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3cvisomsq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3miqwwzhd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dxmunnth.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hmbdrxyh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lfedjvqe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pxhuirnq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3mprnwnhv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3erdbounz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bokleyin.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fzfykugt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qohadcod.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mymmcupb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ppjiaezn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vuvfolir.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vgrhgfub.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3tblfjpkz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ippslxdd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dnbsynov.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ckgyyfam.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ydptskcp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wfuovgfm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ptpjooau.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dptnzhkx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3yvrgltjk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3sjqqkkaj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3miwtghqd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gmoplfzl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xciflpkr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tcqpinnm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mvqyidha.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xyowaxrp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyrcxuom.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wpaprqrr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kdvllldu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qbupslmg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3zkvvugxo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fflcvoej.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kgddcckv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vffqiiga.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3pquwnevf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qvwlkqgo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbxtaila.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jgzanbsv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vditdjyb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3hfchyqdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqbttowo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3przcmdmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhgmywsf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3utgqhezh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3wtajcwxy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vvloczuk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qulbjisl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3blgkzday.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3svltcdib.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gzlpiyxb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3quahdpra.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vuuczvml.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cwllbqad.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xqeovgzc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tsdneesn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fpixryhe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eqzctbes.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wmprsoer.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qrvykgtd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gevtuvdf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uzsleufq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rgmepoaz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bmreebzn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3srowfpok.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lrfltzdh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qojuoulp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bxanhufk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfzdxvi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3utvvhsvb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qsoafeuo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3poiedxvw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3deznhcmd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rwbuagii.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hoyoallw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mfkuzgfc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sttxemcv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gthhpnkz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vmljcbyi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dqdnxyqs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ljakjtwj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3llnuhiwa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pzmwfzlx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jrgmjrxr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aykyeize.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3pcytqlta.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3drhewyny.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3syapelll.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3toouhdzn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqlhymmh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxantkmf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pqfiwchj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jtpkxaor.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qcpfakwc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3iqghsfgm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qlegambx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pcliykzo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xwnfewrr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hxhvlork.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tmiztjgd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vcqgcdih.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3keftdzsv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3osnzyjma.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sotdhoih.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wbkbqvnv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3njufdxhs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3chdifgps.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3iioyjhrn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3quokafcz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3hnvvmajr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3semqeydj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3bwzyxedw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nvtfxvdw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3txmsvrop.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zofrgsib.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jzxissul.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wncuivvp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cragdecu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iguskfok.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kbviuvxd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nimaiezo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3eyusgwtf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cucihvlo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tvsfgcve.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3iyfdoqav.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3lgyhkslw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3eseebtdx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3poxljaja.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pqxiydtc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xnyhfzcw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zpkrtqil.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qjdijevb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3uttyyhou.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3urhsukyg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3yxduddry.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3eibgppyc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yghofkzs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bypiursi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mmqmrktn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3efmmexnv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llyrmttj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sujvzuqs.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jobmvzug.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iudxrdce.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lzwlylms.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iktolyfd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tafxfmrg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3phikhxhu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fupplyas.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccdunmhd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jejxotpo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3udygjnrj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3buxsfcsf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3reugwjht.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tobxqnot.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbkxbdl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ypimcvga.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3opmddpph.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jqlfoooc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3leyjtlxy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fofiinma.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ydgcighk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zofgkixb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wamskbhe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3enhnleyo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwaezvyt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qzojuyrc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hnejzmef.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yjztotqr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3peeoihmk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wkwzslce.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3crzzkxiy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yeoxjsdq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vtmvssig.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zxddrpjj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wggrswub.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qmtfevnz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zkthihng.html


<!-- 参考信息 -->