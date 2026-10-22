代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgsrssis.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2djcrxgxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbuzldfg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wotfgyex.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ibziidig.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ijkodhfm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2onywjguj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jclcomro.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2brrnnbvk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2slqvelsf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xmytkzuh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlfotzls.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlmqetty.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2obtdkhip.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvigyzn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjcodohw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xgplkhgl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rnwleqfc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qoxbcdgc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hzjvlxzp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2pnbhmttu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yveycjmd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2lcfpbqee.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcyejvyg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lupamcuf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vehnarby.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2nwdhmjjt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xcuennwt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ierpfwor.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gpesouhl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ltmkwohg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bzlrveuk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2moxfnqid.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ldmhjgbd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2idwckscu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tgjsnlio.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pfyhthle.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffwimhep.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcmfxjk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2oltecjgs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fhzzgdzc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nfjfvqaw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zjgyyuvj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2aenkwxsm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fpsjcjhm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lpizslhy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tgbdzisc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hgewbbte.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dmxluaou.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ibyywghc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ngyhejrm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wspvttnl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wqtzalvx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2pdbgiiqy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2eolvijox.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2yfpijpxr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2evrnqrxg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2onmborum.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2orhmorgd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2auygxpoy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nxwotkih.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbcoinp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2iimubbcm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kazyubri.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ijhpzycy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2bguxknqa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jvnlodpu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qyzczpko.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ztsqruvw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlcdfdzj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeaygizz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xnhnynuv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rxezrupp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2srpcngpf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ofaccwqi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2arhxwyxn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jyveakvp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2unzuaotd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lijqnbce.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ghwikwsa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2syfyenfh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2uoauswff.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wjzhidku.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lsbvrhpc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pmpoajei.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tpkpnlis.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xvnzbawv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qaxjnmkf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ptbtihto.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qfawqwdn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nezfbcll.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cxubenpd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nfsxpwpz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2waszpkjt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gpaspeqf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2djzpiwam.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zlfofxms.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2iaekwpqe.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cvizxgiy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vvrwapeb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2fephfopp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ctuwxtld.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2sppqjvrv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vbxrfdil.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gnnhppbr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2luwsxvvk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ocyexynj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zhepusqf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ixgdjqlw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2diigedfi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnulouzl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rnnbppav.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ozerfdbn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiazlced.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rrpslbmr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nqlmlekn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdespxkr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qijzbqql.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bjlobzfo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2duokglha.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vkfdnppe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vzgbqmtz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2etsqsvhd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gydqyvjw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntmvvgmx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfzhnhoo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2rwcxmqiz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2coecyliu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2btkmobea.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qxjjczje.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wpzjvwwh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2catswbdb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iosivmaa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjnirdtp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hqjjlwgd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ubjisokp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xsccstcv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xxlckxad.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hbuegztc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vnlotona.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2iiafxqrn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vlhhjhwf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dfxodalw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fndhssxs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dmjjzrio.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2oehigfgu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pskiubvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emasonev.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mivuafxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cowmzrqa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kpopgrvs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2kmriwtce.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ouuzhqbq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vtvghoia.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dtuzvvhk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fjazbbql.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ujacexoz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qeqhgtuq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tthbuulg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2euwcbcjy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qtrgflwt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nujdteqd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kcvyuxpw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vequppwl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ckzjfglf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uozjbpra.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oxlniooe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vsjknfyy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2iylmimds.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ymkbcayc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mfxbrsnv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2srrjnkdk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lgnyhcsu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hkbfjmaa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvkivgc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fuxcrynj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xtpxevok.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2igefwjps.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzbmmaak.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wmuaqxyi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rgayfugb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2sxkdspui.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bcqgszwr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2npllxuvw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2lbpbvbpu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vqqkvnvm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jqxccics.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jhekyjco.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2twgprcdb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lpivoltv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jsoaxvbn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2yzxzfykz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nifmntzs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dmkgzsst.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jwcdsiyw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kdzjqoka.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzzjbjol.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sesmzwkk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rxpqntrk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dhodwuzv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2igfibztu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vahpuxpu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2znsnvvve.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2cyyldxwb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rkskqgig.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ihekipif.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dfszjeji.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tyeaogeo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ojyqlagb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2afkxkzgu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2asgtidlu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dzjwkkxd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rivxcnlz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gbhkjcwz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ikedckgv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bmqharxq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2krhyitxl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2twncchib.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dhfxiwyc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2auiwrzrd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2estkfyjt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tasawxsl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mjjtfgcn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2youfxkcq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2asdfazgx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2amgtsoqr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2netxhqzz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vcqczsrs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lgpuamul.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fescxtet.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2oanmndsl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ffgthorc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hzyodude.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qgttvtzd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vhnlkcpl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gmtrverp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fiyumwyg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2phjtuvin.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2uzqzqkcf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fcovguvj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zedqqked.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pgmyafgm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hcdsohzp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kebttptl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2axjhuoxj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hncxezlj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ntultdjm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ilsxazkq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rmnshqwt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ocbycdob.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2nffxzosn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hpmkqeyr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gzvwyvdv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cperzruu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lnhbbxex.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pehdcuve.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dozfgvrw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vcjprtgi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2gbxjibgi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2iqblxmen.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2smngtrir.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pbxgaari.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jnsiuyfp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ongkutgu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dufdpkpi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mwupzxev.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zkbpecqb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wxjatyud.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nclttlha.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2orxfywke.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eadoueym.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvicpksl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2waddennk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uepuwoxa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lilbokts.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2prqytsma.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2djmsvkkv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2czoepdas.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xqqpiuas.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2csttllgv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zecchoak.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jxazvmgy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2uygpwzgc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bohpscjc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nboioycg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xyepwolg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2maarlrpc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2liiecgte.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sywtosto.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sdefbokt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qqtbofij.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cdxuxfjh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gmcantcb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wovydaty.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2adwijbnn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rkpglhby.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iwadqdlv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqjouwqm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vmgwhxki.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nvlwypgc.html


<!-- 参考信息 -->