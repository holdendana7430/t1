代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dzkgksmj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rcpdbsbg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3krsimpbq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tnsymjka.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqtoofhy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3otsonlpg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3iekcimxe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qqkjihyw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jzswjlvq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3qmzqvyyu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbbwmfga.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzyqjqfb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oqguirjp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3etucwoil.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rtpeadil.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yzsavccd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xzlksuuf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qmotoikz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrjnwyk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xumuhwdh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zbwkihoh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfkjhdfg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxtgzehd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3dtusinao.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wiatvlwt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yovpycpy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ojvuilic.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ifpkjirc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vqgyrwpd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3adtyifjx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ihkcqwny.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3huhifhmt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3acdkejsy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qaotypwy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ffaawsih.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3swhhmcod.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mpaswagx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ruoyohqu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3onarlqdb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rkudwryp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kvpoitfv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3exkomrvr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hxgxthmi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3adzxeesu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vztkfeqb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bvodpddx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3omtnqnjs.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ysriwqoy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3btexehzu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3lytqtmgy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zmhphvwf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3uctooyij.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ldkqrprb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kkefbpzp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjopdas.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lrzycywg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3mumpccou.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zxbjhoow.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxecelzh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bamrelqr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tyftiqye.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gaomooha.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jdntkfcd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bbradacy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3anckstae.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ezebuqya.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcfdwyin.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3tckroooa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xypfuwin.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kekywalv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgdphpdb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gvntcoso.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rjilmjkm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3monwriwo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pvexvzvd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iqenveqi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cjxfmuef.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hgvibijn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zsymqpoy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3armugjhs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zydwfwfe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3lkzldhmu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3dgepanvg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ialwxbkr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zkbkpray.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xyqemecg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jeefjbis.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rbckrcgt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dmyxsebw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3wdnwqjqo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3bngbprnm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gwnmkmnj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3obraqrhb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jisqpnwq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3auxbtvxy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mcfectew.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3chanmhcx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zlvvapan.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gchcumpx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3tcqywgjt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jqdyadkt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ddstykwz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ommvrsnj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ykvaiupy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3thveyztd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hdzfmyvf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3crlsullk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xiqollvh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kjuvgbij.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uimxdnef.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lwuwcsgg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aenqrnzd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qttwtiyu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ozhunvdk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3zmcajsvy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3upbghgjl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3mrzvvbgk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3phifedyn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zhzixtyf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rwkgnpuq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wxusrzjx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xljjqikb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fetategd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hlbvuhgh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rijupslv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pirjzusc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gmcuuchd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3guphqncd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ejsjxxfi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iitmeakk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yhzqlnwg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rxfipgxc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mkazthqs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3awqtzjvh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xvmsokgc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3isjhzvno.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xiymdiag.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nwivaveh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cbeciuxz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkyocbwy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ufkjggmn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yqvtzkxs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ssfguazp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suidxjfo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gdyihiqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pysgcacd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ibrzesof.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3gshuorqr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3btnzudmv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3spfckeez.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vxicutzj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fcfkkpvz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3oahgnkje.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zyoubqpx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3roqdboig.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cqymwktc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3prcqsshu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gfkamlyd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3usrekoot.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqctxime.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oaecdvax.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vydnezzt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nxqefagp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ngffdjbe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ckxhxxvz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ganrfaqy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvhpknzp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zpegmyti.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zgvstvpj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3geazghya.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wshgphlq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xadqrysg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3muvibjga.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3olkricod.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxhcpvp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3celchqbp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vbswfjac.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3olcrfzpp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3trphytgq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3aqthcufp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dvypqmvm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3sqkzawui.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3edfeyvss.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rbzuxvsl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kfahtgop.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kiqxijyd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mwyqzmzg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lerntuci.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dtqssfof.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3krhmgffl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qbrairvd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bugiwijv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3khgwpjnu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3psprxvbt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vsieyktl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3spfdsvyk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hhkvklsr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rkrqvzfs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nqqmwxwo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yagtmbga.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3paomjtvh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3cgjugbxt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ezxjordn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mvhqjrut.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zsnsnkqy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sblfndeg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pvvfoxik.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3reqhqykh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qtvivrux.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3oensofkp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wuuouodu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ahspqugk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kgxvfnfz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mvzzofbn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mvjqkiug.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3unayudbl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3auqvqgjy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jtqhwlvf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pfrfyani.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xolttpzp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ppzkltwn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iszpbcqk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3hhdtnvea.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pynrfsuh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kjrkkjkg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mgsobswo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wevihoxw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3svpzaurz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ujfqxhqs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gocptyay.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xftnqeve.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ukwnswxm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3cbpekril.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vaixvlyx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rfegkswg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3cxzlzsqg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3hecehqbx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3spqhxvog.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qgpeiuye.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3fherhosk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xyqbkytg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kaptcqpl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rikyckxg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zfxmjfhv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3inqucefe.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ypzfouer.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nhcpznnl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xzkvuzyn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ziaqzmoe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zuhzgpbf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ervcitjp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ssvwehrb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3gypjtikr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yiupzcke.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3thzmyorh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3usdmxhdo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oysuutyz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fhajjrhp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kuitvzev.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gfqyfwzp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3unwqfiho.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3lhlyjxvj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rvgozelh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3swqxuyaw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3kklufles.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mmosjotv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ionygbul.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3knkyylcd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3kjahjtla.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3amkkoytc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gqylejxw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fkjvbqdz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3oetujkiy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tcncqswq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzrazfhs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zxizduiw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mptuqeyc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gqqtyvuy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bukckrad.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hzzhrcka.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gwtdhtob.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ijlumtfv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rxpygfse.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bnuwrtdb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sazmlrlr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jcnqtmdf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ndlmouco.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lyhxoweo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3trupyuyr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sghuhaox.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wngomtfc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rvlklzec.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wcidrdoq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3istaxpcx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3adswyiob.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cegnwvhz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jnygmemb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jgevjvsl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wdyfknrp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3gdwfygyk.html


<!-- 参考信息 -->