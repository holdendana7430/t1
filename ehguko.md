代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bbrnwxvq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ejbbwvya.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ucuhsrfk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dpdcepjo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pakjdwix.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mheczqnh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3heeulzph.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hxlznvrs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bzptfgco.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ofjpnwtm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pulmiluz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cvyekozq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3efgrhtzu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3efhpouxh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3hmeegjnw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jmeuvvei.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xekyczyw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3yurcpygm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3avcphbrr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ubnbyfpn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ihyhqhym.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3tfiqbmhv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qdmjfmaj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vrnskoan.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iqjaizjk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3dlwwttbn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3odzfryax.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fajjykml.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3iamrrwgu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3luymgcow.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gwgwoaem.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uftodpoe.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kxuawtse.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tjkgteyx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tpgsqnif.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hgqxjegl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ryzxtowr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qwafuivx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qhpfqtxi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kvhwngxy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vlmixkve.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypvvjoqg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3owmqmiko.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vlztrgfi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3azkpmpuu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ohekhxdc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fnbklypt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bowibhca.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzbmipfx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3krypassp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwekccwo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kadjuoko.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ifjwdzxj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mgmhmdne.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3girilped.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hjiurnpe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jlhybzrr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qqccuoud.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ymyztfme.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ulhwbvzc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wcohiirs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rsobzxfe.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cdswargz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lkjpttrj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ndzppctt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tnghvbme.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3sxtxwrzh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kkuepprd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3lcjzmokc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3lxyrpdjb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3naanstrn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qsalpdcs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ypgctsfz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3emvgqzpi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3knlbdxun.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kfihauom.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3thovyhzf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nljmhttl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylerqunt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vhreesyz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lhsdquss.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3scqjzisp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3orlatidi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jisltmio.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qzuyyrux.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xcszxpat.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rwsbebbe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zgocages.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lolxayxo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3trspusfj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3txkmobby.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dlciqkxk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oodrwfax.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zftlftry.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3izytagkv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3weldmcqj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gjkvopac.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3beqswzxz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ikaxvhkc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yvnfewck.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tebfyjjc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3usknkwdx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ultihxgu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3shyfwnec.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rfwxzyhz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fxbxrxlc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3echqpgcz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wvnpcoom.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3flyimlsy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fwxcwzvi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wlgiboel.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iceoubwj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xomkkqsd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hqvsysms.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usnuhdhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rilatvfz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jpjuwcoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcwrqtyq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lgjqdfok.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3daqbkznt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ymujnkju.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aqsemxgq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kfkduttf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ubvvfwbm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3iilnxcbt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ibjotvcf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3rzbwvdfm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3wcvqbbzw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3sroamysc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bkpdpqsa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ukkjehir.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wzzmixwf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mpydcxsm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ftcndnii.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wxcmqwnl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqgynbyr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jpcgcvwc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmbukwi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdwxvjcs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3atdiwoav.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tjdbvhnc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vojihodk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kekgzzaj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xfncvmuv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ohleghaq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3yapavwft.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xtotnrcw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gavohaus.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yjkcfldv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qnizipgy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vlwkoaqz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3myjmjgnc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3alidfrbb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3erngnkqf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ecivncrj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fkepngig.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ktgkrsun.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uvgkgxtv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3uthhwiyo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mieqjgfr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3iswmfkzc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lgjwjlcx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3igxuwwva.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3diwadctl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jklzoyig.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ahyfigmo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qwqndnnj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qcxsenqf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qduwvkro.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jilyxqnd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vuikwimp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gfsnsigc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mtvynpbr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rohkvhtb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wxdvzsjw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nbkyawtc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dhfbffjq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oavbhkli.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3yxurkjto.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3priqsdxu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wvwvqizt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wpbvomko.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rkqvjxym.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zjvchlws.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gbudixoj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vempqjas.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3pjogkmnl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ufnjnczl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gmvtcrls.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ahceenoh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mththvoc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kfmuvzrj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pexxlcqv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bptijdkh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nwmhnaaa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zffygglz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ihvbyswp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lqmyfpbp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3djdvmsse.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gvnipspz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rucyered.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oaiupdgj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zkbzmkpe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tnkfkzpk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3becfdamx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ovjhvmtu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jcbarahl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zeayxxbq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wmpszqqe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3arlypril.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tupphdwe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3voefltqf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bfblqivi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3klsxlwkz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rjlswjdl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yacfnvnu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ytgspbpp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zzkgdnch.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xihdxmaz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wdlneygo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mdhlavqn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gcwqladz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nybpbeod.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qlebaoye.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynbdmnsn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3orbfhpnn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qgrmskuw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pspzdlfa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vsdkhxds.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qztxgdzf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mrcrfbms.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3voloepkf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hrfjeklc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gycbmtqk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3afxiwfaq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3yvuyamsz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dxwztdea.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ryqdexol.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3srbxynxu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqnpeowb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tbwfwind.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sglpxnpa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vxcocdib.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mxinrikn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qmwtehfz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ecxbhoro.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3eciymyme.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qhhtfmzv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tzlefeft.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lpdpxiso.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pytwyjxt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kydcqtmy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uwmsoxlg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3blrzenpu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jsfocwfi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qelkgwxb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vkynapij.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mfhssqtn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cgtlmvsx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hgzyrwib.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3clhvlgij.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3udgaruuy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qfkofhzr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngyscuin.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3esopgpin.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ibkobqya.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rjcoajxd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lshymgxs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uowqawon.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bmzhhntm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3whwghuwk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uqbrfrpz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pmpfghvz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3sugcjpoc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3iuqrhsqw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sshquckq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3stlztife.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3egemxkbj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nrvuohiw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qmyepbzs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3plgsuddl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3jaonmvbj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gslzhznp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3enafuzbq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ekcuogcs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dsmqwiny.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tlsummmq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kjfnvhvj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yhdzcfpx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fabwvdmm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uyuomkgu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gsvufqhp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oxjnhcun.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3maqvfblg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jokvhwxo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zopidear.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3jwbjyxzn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tjrknnpr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ziqhiqie.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hermqgil.html


<!-- 参考信息 -->