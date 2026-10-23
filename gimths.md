代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3btmlbnar.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ajkkmgwb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3asydohuy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dnkgnfob.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gifeiibz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gdsrdlcs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3wjfhecsz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jocmyuls.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pgshwzyt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rpiuhkax.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kvahlyao.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jrvgsway.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zeuyjeio.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rriswkuf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jpuftznw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cgawmkzz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dgklgpdb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zbzbwbvx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kifbtzyh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3acayyxca.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vruuxxeh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tovlfxkd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mjsxvxws.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3eqgwmojs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvqvcenf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3iwdfdqjl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mncscvqd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3thgqvovc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jfhnynhe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cvvduzda.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kazvutcf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3olqwbiey.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncueqykg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvlpqcch.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wlabojna.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lnqvlgju.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3oqneitqz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3msxqfodd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lapsopek.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3fgqfozrh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3sqycckmc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3iejunwjj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qoqojbib.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3csotcrhq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3albuipkw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bbaububl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3iwhgdmgg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3blhpcash.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3onbalxji.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3cregfzcm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3cxnujdsd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3elmvygkw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3juzvgwzy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pgdngviq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hucnwike.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ackctbqe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3cldhdzju.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cxmrvsxi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3dunlwelx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3jdhjrurk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vriiwtby.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xudlmgyu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ouqczqmb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zsibeisr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vmnlsnoz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3tmjrebps.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vicnlser.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nsxhqint.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3outkykjw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lquyuaaw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qlneunnr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ryemovnh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3svlqfqtn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mkrhrbwe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hohspcfk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rcrgnvew.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3snbewdcz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3mnrzqqof.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hsuwnprq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3axijwsqs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvhydpuz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ykhwqxrz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3omzecooy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3soxetiax.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rvvxhjte.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3blqkcnmb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dskhiwpn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nknhyvqk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yxqutmpl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivazieei.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vguyvduw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ivqyglco.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ovskyqdh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3yjqgriyd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3adbsvlsh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jfbjrvnu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qmjmjtnm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3eilafhww.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3aqsdggah.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rwjioodg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3okpfxlos.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rwihkkof.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqgovvfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3keapjrod.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ryubutii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttdkkhnr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3apieaiyf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mwhiriwb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fcwriywf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3batcnfwd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eagaqmzm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hqlysbtd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qxrvnsij.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yybklvnv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zvvfqbmp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kerafwle.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3byozjzoq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3cafkikcc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hpcmsmcv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cqrycnhf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ttemnqxr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3lbybuhup.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zrxefpsd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jejidozj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jpitpcnv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3verinfcx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wkeevake.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zpfmfprd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ybfolows.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jhlxorzr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mxiwjgpj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3pupykdfv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kmrkupcn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3doqhbxxl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmwgafo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bcccztkx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3duymbjsi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3llleppbd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qvmzvlnc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xbtcwhtj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgzqaou.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vfmaorav.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lnizuoxi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qxychfkl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jkhacndg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qkoezomk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zimfreow.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ksfjxdco.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ljzsmwjj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3akhwcemx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nhaxfdnu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uqxgddnc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yyxleikg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pbhvspwr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ppcitdnc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qujrpafy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mwsbnycp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ovcjuekl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bhgibygq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wtfmzwhp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3dahufbgc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lnxfjebj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3adusglbb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3okgrlrra.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3msnqhqxv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3petkamzs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jxjqhlfu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vxkncvip.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qqzzoyyd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gbuusynv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvjfcjz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hqfhwoky.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ogryiydj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ymlscire.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3syzyxgjx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jatcxhrx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rishqkgn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfrgjlrl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zwjhugwr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fielufhf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ehequvqo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3cfiuzjwy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jpzwqydm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zgeixhgq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eegnpvqz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zowznxvo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ncygdpjk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gonlbxzc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kiqcxqfn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3owrgsnsd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yqfiexfa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ubzsrxgm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3oqefmnxz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jntqsqln.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3udgaahys.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uoabzbma.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3getsqpjt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hkretvst.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qiosfgmf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3uonwqyvc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mbjbzufd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3etrbvlcx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddjtdapy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3htfdvgeb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3pwkhtxjg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fwkmxtwn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3izhjdzrn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cowzvkgl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jepjlzsv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hosthext.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fgcwhkjq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qwdzcfjb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3rdpxhoaa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qcxktkqj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xryaxlnx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zggsujqu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3bsllvrfv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehdnvjia.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aywqmpvz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hpjyvraw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3peakwzev.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xbfbvijq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bekyuxst.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qofdqydc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rcaadquc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3aljsvkhy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ufvnmwtk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gasdwbli.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zzdioolx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tprdheij.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ctakfgla.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xilfnmak.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gvdnbunv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gpyxysuj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ghxquotb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3boevpgjf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zlhtsfzq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yeyknmvc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3dmnmvddc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3dprhjuhy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3numgegjg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jcfmdfse.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gmmecigp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uxeqyaxp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ixtytfrn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3glxeqqtm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mjmkenjf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kalkalom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ntsnvtjf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3auctnaqt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3rtiwhcwf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jcyaepnx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3loqupmqv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nkhnspxo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rcjufkkj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wofsvzjb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bdsjyxym.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vexwfdbx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3egnbssrb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3khrpsfia.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xzupycfp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vpnvqrqz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3nmyqznky.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xidiltce.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3efyarkur.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pxkkipij.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3yeoobmfj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aunumubt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vepampxi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xiytrnzl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hotaacgt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wsuwndqm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ozeglmrv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3caszjxss.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ivpetsdv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fjehccwt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dzltrjsz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bevnjgai.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtuonrfo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gvwunbfr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cgwihkzb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yobrmkuo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xblpyjnl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zldrteyp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3scwclble.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qshswslc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3usmyfigx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yksxrahq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vocisyco.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxqmmyjc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3soijqghh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aabpjgpf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kafdxplj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzesldko.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdhmvphm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rwdogmcu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fefoepfd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vljvljkc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxccavhq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3orkikngj.html


<!-- 参考信息 -->