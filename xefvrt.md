代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ztaoeluw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2snljjmxq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2aogoaztd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fndvlvwa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2owoczucv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxqkxbhn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2yipaalmm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kiacukpe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2iwxynkfu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jiwppukm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2uqnqxxpr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2iyuwdrck.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghwwrfyr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjmqikaj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cdqfkjqp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2sipsrykn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2noumfznl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bqrcxsvi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzzkribq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2jlakcpkw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mvyuecyi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vyqdkggf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ywewawhh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nauyhxel.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kxbhthbx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kzyemsvj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ywqxqejh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wlruzsch.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hzufyeum.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2suxsfvdg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2svzpbnvu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hhtmlfom.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vjksdexw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fdvyehwl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xesxnkff.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cyrxqewz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xipbkpum.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2oqhknsjs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nynbxstq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvzwqfgx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ycoypike.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zgdasalr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yxeylaqp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2krmpqcxz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kxyjsheg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2prpyhzyj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rhmxpwea.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lrwazobn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wcpmhczm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzpjzwlv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkrbaefo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nnogvbgn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2bjqwybnn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wbrjwpqh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdczyutu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2semwybnt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cympjtcj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hkdmdqar.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2erlwzeyg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xylhzcbz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2adzelenq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2acrktbjm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vkduapja.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2utrhqxct.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hlvpbced.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gfuvmhpj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ptudqvlz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wxnnatuy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ossesxxx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kkynddzi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2guqymriq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2smykphzr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uavygakp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bcpunrwy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jzrkoxau.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wtczafxc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yuoobrij.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2qrulvaov.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2kiplrifo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2gtqcgndv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zowmvutj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mfizhknz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2krstcqbw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xqlyobsv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2owljwqrk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jpbhosfb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2opojppri.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2atmxnizt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jrfgmvxw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2oaljzxkj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tjqruuut.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2zolgreai.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rgowkxky.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2irqmkftp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rgnbebcx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iyaouqos.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lszpdwde.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pxxpsdpm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ntfotyue.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2unvsmgpj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2iyncknua.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wwnethrk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cxcitqqw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2egzkjbnx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xondmgiw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2prnrkbts.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2nokvuiev.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2prvospgd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qmaiudot.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2psqjmudb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2iisanxcv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lplszxic.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuqzpbun.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2smfzfisp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2urfktcat.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ejjdgtmk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hvtacfws.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2nzqsvuko.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2pgdgjzuz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nqqmnnmp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qhuzyfzp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ciotxzbt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2auasfmcv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjkayqob.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2pglknovx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2oluyccmx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ltnorduo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrypltbe.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ybwficzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cazqeatl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wpzjopvb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2fdemlslt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hzqncvtw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fxveqcnk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gfkwvuig.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kmlptakb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kdlxbjey.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ytepyawv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hrundqjd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2cgootyuc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2orgxfaur.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qccpqyyt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rzcjmdfj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uwlhonsz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2otkgscon.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uegblfrz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zipskjfg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fyfkpksd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pyegsezd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xfkyvczi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2sxelyeyb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2tmtesfqt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cxtxrwbf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rebvnvcs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bpwfzezg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wuqmwuog.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ompmevgp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2buypfodx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2inteqvks.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zkbiwiya.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2sslnxxui.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zrcgkrfq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mppvqlfq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lmbexfzb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fqycqczo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2cjfvgbbt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2csismsjx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2libiwapf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nchtvvaf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zxftnczt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2znpztjca.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mlxovvht.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ndbhwkwc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nglrgmig.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sftuofmr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2injujrjh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pmcvuohj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yxuejpks.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oinympfi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2srxtcnjx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yljcnhwq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2emdupzxq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ayekrkqa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fdsrjlja.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kmsbbztu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rthrtfsp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ysbnwaan.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xpjkfxvf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aleoyxun.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cgfrbscj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2thsxmqmf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zzddtlne.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iamtbouv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hapoqtmc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfboikry.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ocoprhkq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2aoqrdoyn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hikeggyy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2trtmpupq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2zcxfeapo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2iasxcoiq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rupwkvqk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ywuahacv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wppqbpds.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uplnucka.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bolbdvti.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2tylanvvw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mlggkytg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qpxwhdgk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2guyefkes.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xaivtmoe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cgdutnwn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2nhhfnsmh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2flmnustt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2upxwhubq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zfglqsld.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ebwatttf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2roldymfr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rxtkojvk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2oybxauly.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mghcnagy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2zwfiybyp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uywobovx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lrvasmwt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2csrnyufj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hkfuixtn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ljdswpml.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uhridnqs.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lkefxllf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mnnwbqpd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bjhnbyxu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hjmcvbdh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2aygyhtpk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xsdytxcp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gwblqujx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2svgvchao.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rqczenwb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2agnpwntp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2swdudjmd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rbiiymqh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kttdalsd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pyqplkrp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2duhjlwmb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ajvdvtoa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dvobjhql.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xzfmiskf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rmfmhuns.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xffguiwe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2prgxxpmu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rsifezgx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uekatzyq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2etunishr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vmttgyfs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uweeedxf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fiuwxzfz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2blszuaxq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tlogggxk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zegxespv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2mcrtvenu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tknwunob.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gmkkacab.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xksftewo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2emmfzdbe.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rauzlcxp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mphquqrd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bmerjfpe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cfmjdezh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gsizqtqk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mhkgfesf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lrtxrwfn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rqqhnzxy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2quwicztg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ngyixzmb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2jnayynwx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bumqcqwn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcnxirmn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bijewyez.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2afdxwcxm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2daexmjcr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xbumxqjn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jvjwcchk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2sjbnzdqp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xyzdwhac.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2upjvsmvb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mxgkkswj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fussenwu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmajexh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pnstpxiw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rmzryfmu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2adprtaqb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ekfyclmk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlrjesxa.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cglwbuyt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qcyggbwt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ptohskhr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mlyueeys.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nnntmavn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2churmveq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uipqirjb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2oxzvkotm.html


<!-- 参考信息 -->