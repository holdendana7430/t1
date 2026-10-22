代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wbxkqpid.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uttasrey.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tuhwfhpi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xhengcfk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2locvjagx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlzjpmse.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ybyvdaac.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pqahscfd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fmstoekz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tueexssf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2steddccn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vvirmwvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2moosonso.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lphjktzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojpufgsd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgiarmts.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kgmiicca.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aooxnqqp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hejcxhsk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vldkjsvf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xpaisglj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nnprtdtk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvxirjsw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2viduteqm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2onohaknq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dxgjlxos.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kbbbwkzn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aujrchcb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uqagjlju.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zqhjkxbs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2oietagdz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2gftuhxaw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2litqmkkp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vwfzfznx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2biruafdp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wmvflwfy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mnoxytvg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvlizslu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2lhhibmhj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ykioeitv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2moytbjrl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cexprgqa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jpiyufik.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vgdsyifk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2toavwbuq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rbedcsgs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ouhcczzn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jpwrujrr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kgxtshzf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2noxlarmk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cobewsls.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2sqzjzwxh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cfnnpitg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2oljgcqoc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mdafrodj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hcdlgiqq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tduiqggc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gmdwydgl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2btvkowyl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ntgajfsk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kzcvuzdj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jicoocex.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nupculav.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jrewwnek.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hajgibhw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tdfskdim.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2csvxjrob.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2nsnhyzdc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wrdujler.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2gyaudwpu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2gsdflmhv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtqgtfyh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjoeric.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gtfguark.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zswgcigv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2supttzlg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tssardmf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bflhghto.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xpereojv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2pdsallio.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2uesdoisn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2twonqgkv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rootwzrm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lhiaosux.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ujwpaldg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldjgdndh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2inarjjbt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ezalqkph.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hcfrbvrd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftfgemsl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dbmsztnr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xgudxhdz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ajndrcjt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wiadzdsj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2coloaigk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zhwghjbb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2uxzvgtqx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2swcdetuu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pkachcsy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2cjzevsml.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ihnqcrqm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yquxxvws.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fnqdokqz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2bocncxsq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2torpozln.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2cilwnwmv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2oxeckzgd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jlmvyfwk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2aaxaasct.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fgrycqqz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2qwqbnlbj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2igjttfsq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2quekhjec.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2blntcgiv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2gyirhafc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2enqniamr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ztthjrbr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2miuddyov.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ioizkrxd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2nksafqux.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kyrukgbp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2modnpxrb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2whyfopcm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xtbqwuor.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mbvobfvc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2enivdvyo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ockbemsv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bqwelbhf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bobjycsr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dqezbcxj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jgfqxfup.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2khouddlq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rtadkhhv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mbczjtus.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gssawzsa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ijmcxgdz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nexioddm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpjzalwm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ebzbuosi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ufgyytzq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2sfepurji.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2odhpnbxr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2srevczrf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tqxfqtan.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vltightu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kulnyoxs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2icienelj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sajkswrf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vdldcegq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ylsyqqyf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2rcsfrbqc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2phoebydh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cuimpwrt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xvubible.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lrellkir.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2sjlqghtk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cfbbexcx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2psycfkpf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhcpyaxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbdqmodh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2weqxcwkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdazxrbo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jerlgdcj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2oodnkeek.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gsseddih.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lnhbuumz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tdbsknmn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ywesopkb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yaarlkny.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2nliutzwb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lhjfegcn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kuakyyja.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2oypodoju.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nfrbybgk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hwcgwnvr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bjirwskg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fcvcrrxv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gdrftkue.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rfxmqmxh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2afgyctem.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2akbrotkl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hohwwcqy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2woudeeee.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hqlkbbvk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sqnfrgqt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mxfobbiq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrnsosw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fpmmnkmw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rhhirdzv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xkwlunxa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2umzdruyl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2onpyhhms.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2sexegfft.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jdddeskp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bhnuvmqx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hftjwuss.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mboouvtt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wvxiomcs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ezcpbhao.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wzssnhrz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oxmqnpyg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hsfoxyey.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ozddagzv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rzjqpoec.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2feykwswf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jajbordz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2slksmelc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rpjkzkqd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrhspqhi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pkcrapet.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mpsdrdal.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cpdlelvq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2cquxmbrn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hyfbmmkq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2viplzuie.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qrsqiqay.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2suqoozxn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2fraotvck.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mgjnnctw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xxqahbda.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zbppnvsm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gwvrbpvc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2apaiuxnq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wkwrxtky.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gixbbbay.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kjgvtlmn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndjbntwi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2egxttgjh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mmpwllah.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2osimqjav.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsodwnsh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2iigoninb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2suzapijy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tyueruyy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rrsfpchr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nvuyqyre.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lnmsmbtx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tzwhoqig.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qghougsi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pgkhjicm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yprvdklq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rwowphfy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vacsboig.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wnpozsef.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jbvvfetd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zoijmijt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rwcpnxbi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sbvpblpv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cinqrrui.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xjjgsdgz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2teskolaw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ftluehhr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hbqhowhi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2azkwikxz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emlleing.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2slpxqloa.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2chvmtnlt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2aleouawi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2addicmwl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2krnjvbjv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sgbbtiay.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xgycfnbg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qdwoabab.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dhfacgtq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2usfrrjre.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vgqwwhss.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wocmqbrp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vmdzkgbt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvwalwuc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mbqtbnfo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ftjbwsfz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xkgemzlt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2smpustla.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2beipospf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2worhkpxz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ygimhzgh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xqspuezz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2clmyulat.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdueyhrt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2amnmunae.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jqngbfbw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2roeroqxc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aakpbssb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hygjyxme.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wnyzggvr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2toadzqtc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2upouuzrx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nayascys.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2prqybkir.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bsrsgngf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xzfjirav.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gqjhxmsh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gwuprfvd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2bpgzfngt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2udjjeowy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mxomiebq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2byuccekg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bjzxieqa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjbdqrwf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bbimhksv.html


<!-- 参考信息 -->