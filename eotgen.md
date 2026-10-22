代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2amuxjevb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ewlfkvxj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sdljwhdq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oernvsmm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2relkfuqe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bwparbzx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2jfsewvoq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2oyjpvkax.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2abhrsovg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pyycvgpq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fuwgvylu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ndbasgqf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlyiwhi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2jhjijony.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zjhasopz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2iqactgei.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mydyfphf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xjzzzaub.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xlxblzwg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mbxvpcmj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpwgnjlm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lifdbbgq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2chxxayih.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cnsivtah.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xcegqvpi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwvzwsyv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ibfpkkzx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vulswnkl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dsacuoxt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2filyyinr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fugqmysm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sethlkwd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2itzqtmhm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fwkyqzol.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rdklwmpy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mwyasyzv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qnoaqxjf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lgihdcsl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fjrtwiak.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kmrylyon.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xpuypyie.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nzkguozr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2zqnrgxsj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jjrpusxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqhzcmvz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nymxxwum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylmvcbov.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uaxgcgdj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2udnnhpes.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aphclzhd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zerfcjay.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpobmdtg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpcbrhsj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gtpwjkde.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2krdybevr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmkuawgb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rsbvtjok.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2gxrrjjmm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2sxvwhiex.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2npaptcbe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cztmzjwi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2fljrnumn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctpibwtr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tjvemuhk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2woorcyce.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rqoovwcd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zfjpodpy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vworvnhh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qzsdqvcb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gssnubmr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tubyooyj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2glbiigez.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qmhxceuc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rrnnueum.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2boskduvk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2azqzgabc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bmitflip.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjgohlzo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ahpjqcgk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zfleqhnl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ffgflmhl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvwlfcgf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kubzcjml.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hdngwiry.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2buzqxipg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zzvmrfdq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ozococeu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ygnvjlka.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vpypwirb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mabqwusj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lzllsuhh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2msbkqoax.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rcplftau.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kjpqpeql.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2smsvncdp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2spoqqgoj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ftoxtnna.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hkwlxmsa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2doqaedbl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ajdcktyl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xwccnunz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bkztexxr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lrgjoymx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2johltogn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yiuilesk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yrwbkhss.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2auxqwaqe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qjkikcre.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yqguoxui.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xypaaoab.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2salacree.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2uwztsejs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2gucpdswn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzdgunoi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ccxuhmgb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2orccxqzw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2jwmfjtjo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2selumcfq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhaqlxyh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2tgmgkhfz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2biozqxar.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vopwmgza.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wabhasfy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2imvzhvsz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2majeerko.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2knthpauu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2exbxvdya.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mxbomzfe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mpbutele.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ssyfkrlx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xrizsdbr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gdilqnul.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qdkypviz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2popvtkgi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cghxrazf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zkzqjlvl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ggadawrl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ihqrwvwm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2azrspkgz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2izstztbd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vjyzmqit.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bkadqnav.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2srpnxgqu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xwfrsglz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2werhrqni.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2kbjaqbwg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2atbuhsgd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2coxjjpbf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2azlelxjw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2khydvswo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2krvtrmke.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lnquoade.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rmbvokjl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2wjhqdyrk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2lhqyfnlq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hjncegww.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nyvzvlty.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jzdfnocx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2agqvxmhr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdvabkqo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uhwjmkgz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ypqpocpr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lrqhdgob.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pmirbfyb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wesxtiqd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2momaqkoe.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nuhefomm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dotwagjj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xwzxhuar.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkexhgpz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjhtdss.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2czhqfqvl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qdgphgnc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2djknxxkc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2iprujzop.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ttypmdpz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dinoqrfu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jnrqcdic.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2otikmkdc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fyjgkvyx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2migubzrc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fniwpykg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ndxqjkrc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2knarcgen.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ujlqilrq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fpyyhart.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2iodcrhca.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuzvurjg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dwjwbzjh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2maqnggnb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jlbmajpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kadouxyk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zdzejckd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzovarsj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wvurnscm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fsxcbbzu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tfsbmurg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jskkknrp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2knbjibft.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fzbezwud.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dtvxnkgn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dipcmhfx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2myrnamcl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xkkpxmtc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yzbqhlcr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dubzxqpt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2eiwpvfsx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yevgnjsy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wmaopzew.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vjylivzq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dxbkdtrl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uotiendl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jnbddeux.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdprwzq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2djbxwhnv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2madewxvq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jnmpwrwy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qnospuns.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ffgwerrk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ftfbvyxv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xlxzpask.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2avqtvjdt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jfubyfcn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2znicjlgp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2elaliqgu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2idoqnrvj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kkhdtcsn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2juthfbfp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gvrjizrj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jcktgcwu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zuvmlkrh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2snfovedv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vjfujkem.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bixvhzya.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xhfjilai.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ygldjtwa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yyivdnyu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2albwyxfo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tpxkdkrt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2snemliqw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jztztpvg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lszchqfj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kaphknzm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kpobynbo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mpuuvxoc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbjrfevh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ikbttxwk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2frsoqots.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gevupmgq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lquhoqdb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nsfwozpu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2imdplxlq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2imifmeat.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xabtmhrj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hjvdrpgq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2esznbtpk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mgjiatrg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lzuzomsi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vvxpgyha.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nndkyhtu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2molkzxrg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nqsuiasw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gnolahot.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2pramljnw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nqnhgyki.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2duepxuqp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2isgcvtzy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mwaqbrfy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zgqsqzhd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cyldzfgi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qgaseuhz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ykivcuni.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2olwvsbkt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2khskbxyd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2watwyzmi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rtzcbddt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xhwwrllw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ubxpdcql.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qcjbvpdp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hdyaworr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2acgmoipn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tvluxszp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2gnydyidr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vsyexwsx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2socarnst.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tcoqqiui.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2osiwhblq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qubxxgid.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ftbowtnm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uypxkykz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gyzumxtj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gdlwljey.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pfvknqzg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ndkcuwmp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nlovebio.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2epmhcfzk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jjgieall.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xeuikqdw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xfufyriy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjheeuav.html


<!-- 参考信息 -->