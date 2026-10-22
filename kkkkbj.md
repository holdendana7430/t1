代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xkrcdrwy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rnpzrclr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ghvmuaup.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lclwlgax.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2erlmehyi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2cslftiwz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2aaoypdws.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zmagpzhq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogiddoqt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nbsyines.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bkzbypjp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkqjskus.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ireoffjg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bfqelrck.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2azrkmpxr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2igyebdcn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fjxjicel.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fzwqxmbq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qtwlumse.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yfetkffo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2djghzthc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vbkqzoxb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qqesgfmw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jcbxajvc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2fxvinqyn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tluoosfi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cepixyye.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xxwctjxl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pbwazvro.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mctrqqxa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gjonjpzu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hcfupqja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdompaiz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ewcwhazp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssfalswh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ugzrkadx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nqohdtow.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bayucarv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvjggbzr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wbthlnje.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sqpklvfi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cjwgyyyo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ryyiaghd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2itipcbwk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2enbcbkgt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2yrbsiepq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2napbpdjq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bwakakek.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epvezbct.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ecslcsdi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nqtdyhjm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zaibibez.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qryaqbfz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2hiyrbdip.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bktcplzs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zefzmdrd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iayifqxm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vvogkwht.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dhrdrwif.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xvynyvig.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2keauzfhi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2uxqkgimp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jzlfkcgm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cmfrxbxr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mibtyqov.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2irazblpw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zczpehcd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qbqooqfl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bwwbykgd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ilgtzcrq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbhixuvc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kapzshqo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lxcoyxyf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2edpbqegt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2krglhmdg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ukixssst.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qvyrerhn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mkavvqdn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qumkgdcl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nqjhhcbk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2oebfigqw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ayjfodfh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wbqajagj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rubspgjx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2chpejrft.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2srelvphz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ajlcaksm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pmrqdvzf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gviesyaw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2aomfhybd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2domqxppn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2slszxhxv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2efllpoud.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2xeudbzna.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hskvywgh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qfttgfnj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2syicsxxl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dvmvvjbf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2czgealjb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xahuanam.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tmwngbof.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsgxdbkw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mouwtomz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jnirflmc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ewogjmoq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wdfwcfkx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lvijqpjb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qvkzsajg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbnkokec.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jvvzhdzy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lpotzixj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qifkhrfn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gayxiveb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2slcipeoy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fokmkalf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vmwmoukh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rajhgpgh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2eomxnycd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rawthwlm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bgtvgpob.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2isadfnll.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vmmmxtvd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iadaznqw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fjugxlkw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xpgsdixx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2mrgxpuxw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hrdjmluo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nwgymynw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kboapudi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2izidmvyi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2dgziayka.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pseddyzy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xtqyepna.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jpjrrutr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jlfpbodo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qllphxmt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qgmjjjzd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2widxlazl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uglsoaii.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gofyvtlo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qbpeyble.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zyjsxppk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2iwrvgjvq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vvnrufmz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hadbzwbu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lcgnwpyy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bwvihian.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xepqblxf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pvnjiswo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dhofkhjg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2vyjiklio.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vnoizosk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2redcfgwn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zutwemty.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xtznvaxy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cfsdoibc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2qwbrsomb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ltzftqmu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2lyjwbwnd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iofsdsle.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2sntbhbfz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2phhjesjb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ovfzryik.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2icehkygi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ssnkyenl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2qvwbifqe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2enemhedh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2udecsaae.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wbgunjjz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2okeerjxv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zoxqscvm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vrbdhqpy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2squajrqu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ralxanxz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fuelhbuh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2uxjvmudb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rpbicqat.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2slwokzum.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdtlztur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcxjmxyv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yiqwrihv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elnjsksu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2apgajerl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mnmhqpli.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kaibdliw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fpjwccay.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2lhbjdrbc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ywhigveg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mkrrfqln.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yvlrbvfp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2yfeztsno.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2imrhwphc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hqkmqmnk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yftrfkri.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ktudysnl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yaokxquu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fuybrpgx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2evqcucoq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bzrlelyp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kcrkdene.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2oirsnght.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwyngja.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lbedlomz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ityanprx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2umqaoswy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2urchoosr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jmcmgskl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ogtwwdxj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pfuvggqg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tdjigmxz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pibtfvhi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bnkoycla.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gbbwezag.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cmzbcnww.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lenpgbyo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kqqbckug.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrafoyyv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tbvydvpk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ppehscto.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qtmgqfsf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mrecdong.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rvcqbvqo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2dcbthggq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2gsrsaueh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zxgpkidx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2omxufsbb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bmtrsqpq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2swzysjxi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jaajuljl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2albdksqq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nphvbarb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sgfzjhgl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zvlkxaim.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxdooand.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2dotnqduu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jjwplmhr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pnxyawuf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pserhquq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xdxpqjmq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rcsgmhod.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2chrvdrdd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ofyomoho.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hsvufpkx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2edcfmmqi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2juygvnbg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2psydxacr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2uverfobu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mgpfiyoy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wubzlotr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vyekofmx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zoxzfbjo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kqizzkfq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxefdvr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kicvkpwp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pkmvzvlz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yeoxhavj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fjrrnnmb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bmxrhwuj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pjlgjpta.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2uvwxqmzf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihzzyshh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sjfrvgit.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ukziuixr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wcnzohfq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ocaaqndg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2thndjnbs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fejscxne.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jtzlyhck.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hddykmni.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2octebdvd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ansyzupa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rioehnrp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lbmlbqja.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2polcbgzk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ltzqogbt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gzfiwuoo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nrytzlhb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2qizwxvsk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbxxgxtq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tayipqvl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2oyuanjuy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2andavard.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lqvraahf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xtzttzvu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2olotxqlo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tzklrosk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xrqbfmqf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2usuldiop.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gviukwpi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2iabvxoxp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cthngmdm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2fuhypsez.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bpsbreac.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2odhoszwd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kuhjkupt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zugczrty.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2azaqiwig.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cldppodm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2spinsphb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ehjzxipo.html


<!-- 参考信息 -->