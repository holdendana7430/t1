代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pldcfdlz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2uwpxdcet.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkznipws.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2deuuuhvu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sxiaqhzx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jojejbjj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2whjngvjk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2oiejtidv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2pfqsprzt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2yyzkdtld.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ottequsy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijrfeuhf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2deoysixs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2medodjom.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtitcgcl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzfojbk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2oemrkthw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ykauioea.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwfkimmc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2krvlxhps.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vuthvrzq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bzqdhjde.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ajlnhujm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2olcffxlp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2affyprux.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2labpzlub.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcukmfdy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hoaijujg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ekqechlz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2encjsbgv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wsilydkm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nlsbbjbq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nbcbcnks.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fydxzfhn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ukztqxbd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fshuomnx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bwntifmh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2avtqermg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2mrjxglve.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lwuezbyt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ucbmoufn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2tkpitkxb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2waihcthm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ptpxtruj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oeoxglbm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2dbkymvdk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2sbgdhmkq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iuenxvyu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2otulcqms.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xjstbgbg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qjzmaski.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ukihgrur.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gsxxruol.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jmhsrnxy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rjoatxvb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dcynnjja.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vodnslhj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyslgbcc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2icvlpuaa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vbiiozed.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2bubjibzx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hgwtwryi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixsdvrpi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jgydiooe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgfznqyz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqmudqio.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vjxbbrrk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xwdmhtyg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bspwuihu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2grmyjvxv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gdwcryei.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2noakjfhn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wqdtdfkm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gfeoopkq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2owzzmbji.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rtuogkri.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2knbrgidr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2coiwhsau.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2klibzyhg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hxuxjzuo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pwyineqd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2iknxysll.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gwgtfaxm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mcvwobem.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wkuijwri.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2zdptprox.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cyiillpg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jsibrlgv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wvdnmqjl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vxuugcbm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dwhytabc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qvnckkft.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mxpoueto.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wqyzfibq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jlybvffa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2phtjqxmp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wuwzjobu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zfvdndnp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pztjtpbx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hffunsnb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qqhmvfgm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2udqbouty.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rxkmmwoi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2flizqvsg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uwzogrdg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mjvqmtbs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ghighbie.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2miogddhk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mbuxazym.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rrxghfax.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xphcujbl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lidybhhl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kpkldqyk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ijkarnmi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qzdtxbsk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dwbxdvxo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2yvkophip.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bbprcuhf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tlyeqlmk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bwmeefcd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuyvxkfg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpccsmee.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ksvuyxdj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tyahxigj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jqwqupta.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zxgfcjwz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fsrqlqua.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ozrrspwo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ijukslop.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2oxwcjauf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kckymnpy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2imoihpqv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ifhrnwse.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nexjbglw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gljiydmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spmnnptl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2higkyvgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqbhqgys.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qpgwwpqi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fctmwxyk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nvczmsbj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zovdnwoj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nrpprsjn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2oevmccgj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yxjxutvq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nbjmghvb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2kayqvabw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ykzcfkkz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2irvlknky.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xrisdaul.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2shldbxai.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oetgseia.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dxjgkvsq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kttnnkfb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ackwjfwf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2onagldym.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zhdrrcgm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rmpfopwg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qxnuwgxi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2xumccsbp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2paeprkgn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wxqudcok.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2eyvhpwzc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mxwoyyxl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cwgdihnq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rertekwz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tgvtvijb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2cudaxqtt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pdfjnooa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hssrsxlf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jtqcckwh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mhnacwsu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2urorsyrr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2eqqpfonb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ujdbyfut.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pifpnlbb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vxovodbi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rvubfdyp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2oowsifvk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qxmahxpc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cxtzwjez.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bmhbhznn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ehwciqza.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmrmcqpv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jqggpdoe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xnkeyqku.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2donagjqu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cvdylyxq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dsrmngja.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nycvtlsm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ynqcrcnl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2evyjlzen.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2cwpfetzl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2iiszysoh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dafrsmni.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2akqejbew.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rhnhihkg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kfzkaoel.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rtaebugp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gnebvbbc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wtrkjjuh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2imufbqfx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jepzvyon.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uyemqdch.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hazsqjzf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jhzekrih.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lntmluvc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ydspivst.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2unbqzugl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jyesgebt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pgncezhj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lszvsdkt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqzzygnr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tacsnure.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kfqeuchh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tqisosuh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rxmzuqqf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ajfzlzcc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ikbkjzum.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zvcejbjh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2enbcvbvl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2upwxgdmy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2catlnnjv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ioplymsx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2uednkrxa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gzvtznue.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bthtubjn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2haswblci.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wmcqepaw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cfjchwbj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qefzkait.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vdqhbhum.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fnafwnax.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nkomhthf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lwqauaty.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2oqonxqez.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wkqjnqix.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2otckmncf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ulletziq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vchlefrz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wkeomfnj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dcaedvzt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zwfoksit.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fukojiny.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdywbukq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dpdldvpd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2khoxsgxv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bxxnufpr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lwuetvpi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2peicoyez.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jlsaqkzp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sfqsqufq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2luxaxpfi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lejldcpx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uyyfokqf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gfgjqbqb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vgkhhvtk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pxvsdsbm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrobbrhh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdqfgcmk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yuukqdvq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bauosnra.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jwwddffo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2okjblyeo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qzptaumn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aoaqymlx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zhhjpfzf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jjkyblun.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pthtgpub.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zhslwnug.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jhqbpbhm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ktvcrrgt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2igrtxojn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2uuejteoh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vshazccs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ffemlxwe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2noyfqfpw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zqhyjwmw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2obgkvngy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yiefxqzt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xxmcldac.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rldxqsqq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hfkygbzt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bnqdlaww.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dursilxc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2zvggkjrm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wkdvtviu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qszqamwo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwuvqnge.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oqokypjv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nkapwyix.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kophzdah.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2guetltnb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jnqpwqoz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jsfzxllh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cppdbami.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2newhloab.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lbovwoaz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2coeundbj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zedafadp.html


<!-- 参考信息 -->