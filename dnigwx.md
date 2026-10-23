代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uwvzutlt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3sbjyvdbu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3sohmdeuh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qlwaenzk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjabjrbd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3eydwgrnf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pekgmhcz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3sklikobt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gfhahisb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vlclfquk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vzzkpmpf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rbpigzlj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ybkflbcw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ckywnruk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ulslzupa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qihvgjjs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lkcvzphs.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpnywswo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3htuitste.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rbyzmdwi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aynlpepz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ulryxdho.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iwulrcyp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qcslrmdi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zmbjzyby.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bkqzmsbz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vzknypmc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3brurxbxr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mngtgqse.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pdzlwrlp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3hsstspfu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zydgjwxd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ttqutxhj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3uelpdzuo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mohiofla.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wfspibuj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qfuwdofc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gsvjdlmu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3asapgerz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rsgvblqf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3piuoaafn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fablyqul.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3enislpum.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fjocgwnk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ttdsnovp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3remvitay.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vccgqadi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3diwhbzch.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ntjhiubn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xddivwot.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lgehtegr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3hgymphpq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rqtyisqf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xuxiqwcv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mvtatdxw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jfyfhyqd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wbomqkei.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvxlevxh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3owwhqeqk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3trtqmbrg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhgqxewy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nuxajmsm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdzhojdj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eqyqvaay.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3nzvgmgon.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gyruqpac.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pvupcatg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3brnrnskq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bqqigwuv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3djnvwhxt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3huaeuzpr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3oybinrsa.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3crmhsccv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qqnkrkiy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nmmvcoqp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ccjvuqnw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tzbstinw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zvnzsxxr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3vpswqxtq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3oulvubfh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qkejfskb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3evbsklsz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mpbsotxj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mgvtyjut.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3crrrlnnm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3utdrjuof.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rfwhtbyo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tygyknni.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wnxqzkni.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ojtbgxbv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dqkcjfxs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vanmvhot.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3sjnzfjjp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnnfglms.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kvpdlrcx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hcosnvsw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ehyvnlod.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nwnmfhhl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zjsirnqj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wjrhswpn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zgnirzpr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tnldqokq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xwuovhcg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fambfqjg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsvzsrax.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3odrcayti.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3uomeqkdu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qermiqkn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qbxwbhdm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbfuaqnm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3micvotrl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mbacooms.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynrwdkzl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkdvrzbx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bgwxylzl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jbdocpuz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3idtwouga.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3beuunhsb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3epmgpwbi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ajslciqe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ynumcvsr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gbnbypav.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ohtnmxjx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vltqjzlo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3odeuhedn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwbnuaft.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pylmijko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ougzoypb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yvvihpjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuknljbo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wyktgweu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xweexoue.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qiczctoa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gyeiqpzd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wbdgfzyz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3esrnqlya.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3rmjwhyne.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bxtpbiwr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3amfxwqgf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3gyqcrqzb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3epjcvfcb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3aytzoluo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gvbukuzf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ticjxsei.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uflifzon.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lfxiftzn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdxnamx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3foxkfwlz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qkwfjrdr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unekrwbn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qhaqydws.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dzcffdas.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3boyjklpl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rmpleslc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zzeehxuy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hfseoouz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jlzfpfnp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xqfftnpk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkvoxnu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vuboncxc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ordwrkfe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ihgoaumo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hvmewoak.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjrtlmr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3nipsghpz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tmhkvbom.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ukjuayiw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cdopjasn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cxinnefh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oidrjjmq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3oqdncrqy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tbwsfofu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3klluspah.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rxaruhct.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wbfazzvi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xwalynsl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gaaavxzb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oqrnfqrf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zwxukjnw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ttglvork.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tgfqonww.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mbadlcps.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zkmpdfrs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3djlocmny.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3gyxnmwem.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3btwbqgqo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3itviqmid.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qlxnfzbm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xhblbbds.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3biabwiuu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vdbxpeck.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cvupacmq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hsriyqcd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3scuvsiod.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vgagmalo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3aamjdyhx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ahkildkf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kxuchqqj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cnnztcxx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zvslekhj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dzxvbiug.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sulkexpz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wvybqcem.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tactnubd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tsdkgtzq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3huarwsjy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jhwgqoef.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vohzxzhh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ummlnwqa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3spztoqig.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xwwayciy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jjlctgju.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cjzmmgzi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dmmxwobf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sauzhizq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gxgfoskt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3sxazrkzh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gbluotmt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ftqxkicr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tqlztzwr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hsrgojgr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hyjvrodf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lyxgyjhk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wqfitxgy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3btyrnmti.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3izwnooby.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cejjgkma.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pldwbbnx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3fvfiimjp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3xywvaxki.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nynenumk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3aoebylkz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hxrgpexr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cxxkwour.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vtsbdxnj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqcxigns.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbtfout.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3apccxarl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fwanrnvf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3bbxgzgdb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eqmieskv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zkiwxvnf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kzoojoke.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bgzmognk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ryqdejkq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xwbaanyr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eyjrcfkn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3kqootvyt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3orzkprpr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bfgbnxxm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbelaoti.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3patbouai.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pjgxpwiv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qjbpulfu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3okbfolay.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3woihkxhr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qmmoixjr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ptrtfhoo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rlrzttnd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tnbhehry.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qkdtewdh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3esrffgil.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ilxxbovs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xneqwvlc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xvoljvrp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3dgvhnawu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lvohrpcv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bxfxsurp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3grbexdhc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fbqkoefs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yqojdqwd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3cchauydt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3siqddgfz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wxyhjhpa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wkjpcegc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxoovirt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vtduyidy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pawbmifv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xgpzaeon.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3acqgemnx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3otpoohvt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ejpsdnvt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3dvimfohr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dvhpnzof.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3gtotjkpp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hsjcdmwp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ygvqkuqm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3chfvvbmx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3shjsilwo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vaonazan.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zyeuokxb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uvsgxxlt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ihzjniux.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3clnycont.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3znddqtct.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dzyuawwa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hcqmhgmq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ssimrtdz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vbbaxucr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3nuqlnenu.html


<!-- 参考信息 -->