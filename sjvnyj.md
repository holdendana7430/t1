代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bdjbqtvv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pkpxgvtf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnqrgqyz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnsbmapp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qaemeljd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jhadeppk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2isycyzkr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qnjgviwf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dqwzurjr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xultgovs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2kvkkxkpb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaszskhj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahgtbqal.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxqkyzfp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rzulegtx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xcjymnhr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2alihrqpw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2roizfswx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2znemlqjf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2icwositn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mckdolke.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2relhpwod.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jpuunygd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2batdagbz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2slenuild.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ytfpqvvw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uxdodrpo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bjzepmkq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fmadalbp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vtthddxh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dmlttecf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2slvwwucj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jruozajr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nfytmxtk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kbxjwkar.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2wcvjfmfp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iwniskff.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2auycysfm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lppiygkt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wwjmgsuw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fbefjumq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ylqasgmz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2okfprqca.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ofdcddon.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hyctdpqr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2nnsoyjxt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ufnvrowb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2plphlelz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nevfscwz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pmnybvdd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mnpkqbkt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2myhzksdk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rtxphrur.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mjpinwir.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vsgwrnti.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2cgxhvqkw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dbhyninm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lceldswi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2txwukzhy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bfeljvgp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yftnfsaq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kwyjnfqf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2antavhwb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rlaydyre.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nxiqdxwr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpxnmkap.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pedxcumh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mdmewmdq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmhesthj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tfwmmwbm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bbvtnzeb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2rbhpbxzp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2walnyjqo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2pelatuen.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2aeojdkgk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fwftbrtq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xyebqwrt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bnyjhlaf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lgqnydzb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fujcbqvj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wmsmkkuh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ctwgdzts.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cbugoffv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jmypltee.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nzajdsff.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2duecwtcv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jfxywnrf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jpojckao.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2aldppbdo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hltvjvqd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hawdxjrb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2sabjwyet.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2trmaqciq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zqjepdqt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mxloscbr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zhesebhb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2urfrlwgp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qgaiyvbv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdvoqjby.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wvoybvct.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nbjbwxcs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aaplgpnr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gblonzoq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwkcixml.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lemmfcwd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2klfgxkjc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2vzifzufj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lumcwchv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bxlkjjgv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2aonqoqsk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lzcdzzoa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jjrfarca.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfvwwhhz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2towgrxvn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2pzxrgehy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ojojvkpl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wkndiukr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ygscmogs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jtudexje.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2oowncvoh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cozofthf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2djnhqmnh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oqkhwukz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wvmnjkya.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2aqotqiyl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hunrklon.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2enuaahho.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hshfjfai.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2sepzfere.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tldspbcl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wshmmubs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgmahllf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fkdzdiyx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2epmzstux.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuubhuww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgaoyriu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ealjnvmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jegtuqxs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wmfmzgai.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ndyjdqfh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qpenrabl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zwuavqpl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qbroctce.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iccxgzjj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2kushaobp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yckluzcx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xprixehw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xtvapkkd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qpwppjns.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mawpzanb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ytelnsmm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nxklxsyj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yvhvrilr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bwubbhex.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2dlltxykj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ixjmyaqt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ckoozfnr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mekgbmxi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2tprdoohj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hkziopzv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nwtfbung.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qjvuauhe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ysqlnzwg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rxsdtdpv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2syimwomd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kndpljzn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jfppwsta.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tmlkgnjh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2sntqoqef.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2raruhony.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2djgdcojq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2noiixagi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wywcnazc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ystnctlx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gojwacoa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hddyyley.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ctkrypjl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nirbendy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2yruezbsg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2irrbxlmf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mrvukaxy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iftewijn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pajxnmlu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fcyatsbt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qlytvpis.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tfoohbpw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gqdzitge.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nsdqreee.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ohmncgsw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwwrnut.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ccjdsivj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wtptromc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fzpycynd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rabbyicu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zmobxczg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2swqnpihz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cektepls.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ozffhrwq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ypafcrza.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xysapvmf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2grsfkwcn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vdyoqcwg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2koclrcru.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xsrzwwlo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rqcuouor.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2kecrjpbe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2cgrulkib.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mebkajgq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2aovkmcjr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2asabangl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ukgkjyjw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2izvobxtj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rebarvln.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jngkxpcg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2iilktwdb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kgitjvua.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dydxmdvr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pyiqfero.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2amcbjbir.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vzvsyfks.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmapwsu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vgkxmdwe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fmssumfs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kxwefpkv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ltztgqta.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2oexigrfv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2pqapcpno.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2begsurku.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cdochrpz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2bmrzeqxt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sujqtdlv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fkabrgrt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mbuxzcny.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jwcxvgzs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vuvtnirk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ampstdvi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xojjzjmc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2oqhajwyu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lbneylsx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2huenffum.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tieykwqx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oeskeuhh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2auuejcbl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucrfqqvv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mnohpbht.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lxaocbuo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2rsfqtxkh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2kexjpnwu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bijoontb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rgssnglq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vphylvys.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2mzphlnbj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lxoulknw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hanfbnof.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rqwrvlmw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mhgbvotb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ycnlyieq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sqowqbkl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utmivpxy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zokzhadu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zfjfxxhc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wqffkhyi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jzsbjoht.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jtvtxsni.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dcfpojji.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dbggfrkf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqtnegsl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yoxazmbw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2baclqfrv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ewzkyllz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bvqngqas.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mnshdnrz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfpswuxm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ilpdbgrs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dgvfaiwt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhvsqutg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ppzeqtga.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yyislvmo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2yeevwxmy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2himconpn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2recbgaia.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dnomriyq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hydplvve.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qjqhjftx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mgmyhyne.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocvxpdao.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yzyndyqa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2gyjbdtth.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dlowbxce.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dcxjnlnj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ozkuqfxr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2cvhgwmwu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2isykzwfx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ckofhnwb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2cmekyjxe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cwgaptoq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tqzqfxrd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sbdtyeic.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2odqpxant.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mbpozgpn.html


<!-- 参考信息 -->