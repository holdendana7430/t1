代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3yaswwrit.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwowahbb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3thugqlpe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zocshdpx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnmhftgh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3trvdjzwc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbxmrghy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3syjqxdsc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvaiodwh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ynpwkxmi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bfjzjidc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3euqxlkka.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yefhsvid.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yljdfghh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3icziqcwn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ukuxqjnh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3znfjfgdf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3djnhpebh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ziidtrch.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tapvgctp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hslerpvr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xdndttnb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdmvcdix.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3tizpyjdj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3pnlzrrnk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3groynmxk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3lqzeubkq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3egrgnskv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3udfdhcav.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jegvxfkx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3udhuauhd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3secoktxl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nsucaxxq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwhjdzk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etdcerrx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ygrdrsdw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qkrbdcxn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wimhzfqq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kloqgayp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wkpolmub.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3spnpsinx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vmsfhpxe.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3avjkjtli.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3toqusfst.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hgtujxoe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qqnteblf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vyykxsep.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rpgatoxl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bukdpkcj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3kpmdhdyx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3esumbjgr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3oxzvvmjf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3esgbccob.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bnigdyih.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dsxnfyuo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iayjqour.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hdlnojoy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zypcyibj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3izinwkde.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mfdfddrg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zpcgraib.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3nbyebugj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hckgyxmw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ktuvpkgn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ywldeuwg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcvcokxi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzujijbe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cydakbpl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3amjtuqig.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ekacxwun.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qtfxsuse.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vlqouovn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fqlvyqel.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yewamxsu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tjiimpoj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3waidooxl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvxlrgvx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ztqdwowe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3phsckzyt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eytrhfiw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3spipyrsm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3yzwcarbf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hihjkrmx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3srdasqvn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3agujxtqz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bxbaybzy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jouhjgep.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3drjhqkuq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wzoilykd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fhedcsjn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vkkzbfni.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xdziqkmg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nqdlrxoa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pvbgygar.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wkobtecf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3nuhzxunq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3avulbueb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vpgkxfgf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uncceyyq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qwuqqtaj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3myjkiffw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yzpwbrwj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jhvrdinv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bqrnwhib.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ousvsbft.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uksxiuyh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3mygprzxs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bhsjsrwv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cgwhygln.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrpkwzyd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ossmpnek.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kiveuqdo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3beppskya.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3xxxgfhze.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pmawqbna.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vlmeycre.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3weccnucj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fiybmgzo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ewfnqtgv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3slmnxyzd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfpjgfxx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3amsedpkv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kbxowbio.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3byhomjdo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gevkdzwc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mphtrtci.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nhymibja.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gekowcrf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyznkyjh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtcjedfs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3baxijrnk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3umbsdcfn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3boldnivd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3keqkuyrl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3cagxerua.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mhhkgfwj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rbtkiqnv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3cqbjxqve.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qqkzrdtz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cuzirolq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3vuqwlssj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mvodzxlx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfprocsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vymnefra.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3pltwjkfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbvjrojz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zmmbnxss.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mufbqphb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3axvgvnjp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ugswgxdv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lehrltfz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3eaiufgfd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3redubdvv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vstwtcbn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gmofjyxl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rawklxyn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ypfhbzzj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eewreoyc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pqepsccl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3iuhrvcvu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qnjytxcy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hsqyhtgs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3topmoknb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rtklsphx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dngclxky.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3oddsppfd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hdflmxfx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hachjsrd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rdmwqrxh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3loefoppt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uygbnpke.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nngdymky.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3diujjqfz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kzyekwbw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vbwpatmj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3urynihon.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3osfzvzpc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xqegpbdq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3nvldllhh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wuniosge.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hhflxfps.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3kxbyloic.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hgdjdqrg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fdmlyxmp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mljgtdye.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fpxsckmq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3bkaehvtv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3raickyjf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3exyunmuf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qubpnugc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jnpqnfla.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ftapmbwz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mzqetyhi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3efbpseua.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hqeojboq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zuvjacbo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cqfccqxz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cznmunio.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ageqsrhx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uljdxnrf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mnrytfdh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3oegdrsjg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tjjsbsac.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qdebdqkq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qrmtivon.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mfbepmhd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lpiwzmei.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3urqrwvjr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dnlzzodo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ggsxbrpp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vqqdjbux.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mlsgsjht.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zrdyrbwn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3sromaiho.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gwtiqwps.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3eghzmlxe.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rffzkxns.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ilyppdiz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rhhvlufl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xnydlehu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pfgxxjcl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3itmbuvsl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qylplrpx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jboofjde.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddeqwlpt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ihvzbnal.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jmnruyhh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3fahqlybb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wrdkxazm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ydmkudwp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3judyqqag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pthbtkyx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3nflrdqql.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gdgjwtip.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rutcrcxk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uuenydrv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3sfvkloay.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3njakvdvz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qlxzyick.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dasspfeh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mmpssgkv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3gxebcxqh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nivaevpb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kgbciyta.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zczvwrfs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cknotomx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qohepugl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hberceju.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vpulgdrr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zqcztoio.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ozdrbdvw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bomuopjn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdzzapgu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tyzbnhgb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3deyvxprp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ooaetmtu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qwbgpbpb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dpduqyih.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gchuzupz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3igcbshpj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ljpikcly.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sqrpeicw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jxqdyark.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rygmudvq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pfuxdlhe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hsjkmfni.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ykaumily.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mclnfnhl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pboxigvn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gmvxndyn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pftdrktp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lmhucmuf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3swvybyef.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3potzaghr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ezwizoyy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qovoqroc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oicwodxv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dtgboiwe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iogeiykt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tozqzrgs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3faudrhht.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rijcygnt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nuceprzd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqcgituu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bnbclhmz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zihvgclo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cmzowffm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nzzfwola.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ntabxjef.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3emviqpbe.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nihevpwg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzqygiwm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dodplkty.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hoecbful.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwsvezth.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ubpumcjx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pugfqpzn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3yatpftzy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3scuqtzyh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jhontzvq.html


<!-- 参考信息 -->