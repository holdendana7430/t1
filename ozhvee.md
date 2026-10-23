代发 wailian999

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqmtqzlg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3qhponiei.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjglhdxu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmzypczl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3urfschvy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3acbrdevo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lglvhpve.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jrmdejvr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3fyetiigu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vuwgbzhc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wuismgml.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftwuflek.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbmedjmo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wibaygar.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3swqfdnvh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3onlufyyx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3uqxjrwik.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3stpevwra.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3relhgifi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3aylggvbw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wgowktbp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zjxlqaoi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jmdlprhr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pypchtdp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wkpqftad.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3njoovjdd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfnhqrbj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3odyqfjii.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dtvpdsoz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jsetzojf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3loflxjtk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3anxajuvl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3yrublwjv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dbkgamfo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ubhyyncm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kbmdpfgq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vauijrrl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kqjqskgh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tpzmzafn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ozybjupz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cyprazqn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vummvbza.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3obbvqvkk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uqiljeig.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ofjxffcc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3neiekqmh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jvczgosn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dobsnbyb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kqbnpgjs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrcxgfz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qtopdyot.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ewirvmlv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3azdykzeq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wignazob.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yxxqdjwu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jrwtdyqm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dviakcco.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lzkukadz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bnwwikfb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fmbwspjc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wfyfdmhc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gjvuozwx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3orbjraho.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nerydipn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zretaate.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vbeewyav.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qrkvqfep.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3osusjhcd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3asftgnww.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kdrtbmao.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3poxkxrzq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xbidyfcj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3qvqgebex.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gzhqrddj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hyicrnca.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jrcyidex.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3atqhywou.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bafvouvh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kqgaubdw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3djcofxoa.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vkxedrxp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3advruwxh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ypzkewtr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ogdcwxdv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3grtwndrd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ndfkuddi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nlpvfgtc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xtmwnzal.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uzrqnotu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nofhxtnh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3npwirhum.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ivqrlupz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3twoaheam.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zhuiftgi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dbpiexzi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jwtdloou.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3afktxaiy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qbuerjgc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtaxcuhi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3sqlpnahb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nogglaef.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3klagnoqf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jkjjzixu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdvbcnmy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtspkhxq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ynfpofiw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pldbonvl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3prfffgsj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pgfynxbe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jhbestxp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yawiwdgl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vjazwhbt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaavpeui.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uecprdwc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ijlmuauf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uppchazk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3zflmvjkh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3iwowdrgz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3xxclalcp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wwxymkcg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ihzpljsv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3fmqqhhlw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zfigyqmm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3totzewoe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zlunpult.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3pczqdnll.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3athypmcs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3icwyoflp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3spakjpil.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jjurphxq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tdoauqhw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddxvezeu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3imtjsxbf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3tyopcvwl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjsilexy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aencoclz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xnmmrtvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiisofyt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ppdjrkms.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hfjuwqvl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nkqfuvwd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ucwumolv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kpvwnpoi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hfsyzxom.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jykdqnov.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3xionrcwc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ehqwysoz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ciwegnmh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dqoljaiu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fshujmaz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vnzkxrfg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bkmxcrju.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vzawytsm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3kkmhrevp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vvbxrxgf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hrqtfdxu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bwjnyzfp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3aznchzdv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gljtzqvv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ltqnizpe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cpsqvinl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gaycgrak.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mnqbqpxv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jrhbfgeo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qnmxqrjy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3uxxijgdp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3njlrqrfj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yacmarbb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ajxtasbl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gfvtfqod.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fizqjdst.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tnuxgrii.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ceoiyvvp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3tnnnnxsa.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kkoazmdd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rgvwcerw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gvnrcfek.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qapoxidu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wcwzxlid.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fvfwgjhh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dbctecje.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hpkyeqkh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tsgwsfxt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vviwumad.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxdrfndd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kdvsvhjn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qjrbpnqx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3idnrkfmm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ohzuvbzi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yrznsbfk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jlbwepph.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3axxjirou.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tcimbidi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jytdmwxz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jieazdyz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bhiidbyd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vqjpyoni.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cnlvostf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vvpxrpui.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pdqgtxed.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3diibcoer.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wvujuwtv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3urhccjbv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3emkmgywg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3utiycgcw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3znhyvwuk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fuyekvev.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dctmkrfo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xtznxqlp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3msniwsjt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lmpnzvnj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ssmwueoy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wdjvekvz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kfgrtvox.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ihbkuide.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cnsbphaj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3riiiefzg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pskjvmzm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3faunjjfq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zrclshgg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3klqazdey.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zncroawi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3prwmtmxy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3szfgvbma.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xkpllrko.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3oeliunwv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ueiwuvbt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ekpyihdf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mrmoneuq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3aluvktrx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scbepbtx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yvjbizhg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hkqjndnj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ypkplxio.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjwhdymp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3epechtxf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3znugnuxh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3surczmra.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xohotrnw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pfndrpln.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgfqbtk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3quvnrdal.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3aydqydvb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbvtbfgt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3gzefbspd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ldkqnbya.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3abiknjcg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3exwzyxyv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ucyokvfx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vktoowyi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3poatppok.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zytrqedx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gtsvmdsw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3puryyjkn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oddzwans.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tajvlqex.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ufdhhusy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3osesxdiu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ofegrxbi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3coewehzh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rpxujoux.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zfzzemgc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eztdtjyv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vermfjjx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3buzgnvnf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ucxikrij.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jgtrhibz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mbtsqccg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jwrcarne.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lciwefer.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fzrnhixq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qcydkgsm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxjxwzpt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3phxcacxy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qfsaswrf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3spvmdofx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qiwdcrse.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zgggurjg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ypoahcgp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fohcxypj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vbebsuhc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hkxvftcb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gafgotcl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mfabdrbh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3guifvfte.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgxychxl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ptgllfds.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nsctkdaw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qzvbzlej.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3daexrjkv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pqwpxcru.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kegqlegi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3aseauuwl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3nzjxxrll.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qygwyejb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lxsgxcpc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hergvotx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lubikdbw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3trkisqak.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eivakuuc.html


<!-- 参考信息 -->