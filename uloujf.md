代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kduayjtx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ireasfjk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jkgnhtql.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bpynrpku.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rkilcrpa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2emqoolir.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bbueamtd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jyzibbha.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2clnqsaor.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2glydbcnh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2bqazyzdk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vodliidm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lzgouwxf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2uncabetr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lvltkapk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zjjmrcek.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zfebuzqq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2raaqpcar.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2tdwisjlk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rajgiatq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ctawfyor.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lstkomok.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jddvizbs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kboutnan.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2outvcngg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wzywsxxa.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hqfbqrmx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kugdjlqx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qoqqkhzj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wyzkucbq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmwklqym.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2onocrlqn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wfpzjjxj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rqgemtmw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2higgtvkp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ocmqlzgu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mficekht.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2trdwjhjh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ipfrwdaq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2csohdcnm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vocqrlpo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2juadqydq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykstmysi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hbhykmtx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2huqziqdb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cfhsfvgq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2htjdjxos.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wfzderpk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jojkpsdf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sabqwjga.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gmoixeth.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ctaduezo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qdavuqjq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2stmbfxgg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wbgazizp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ctzsxrnn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pzamugdj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ffonwukr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2oigctqgo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cayjsgvo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wgyqxwfp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vkpxbohb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mjvcldna.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zitlafkz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ojxtydbl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kmptijva.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nolhnrmg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2yetjraoi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bxatvzct.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bsjufvzn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2lvockraw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vrsjpcdn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ogvoljqs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2abvjznxh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vtxttkog.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqjbwwjn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wttyzmxi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mptgarky.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lyxhrnhe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gyrtwamw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zfeawvef.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ynmzuwqi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mnofesbh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fruuiosl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvqrvzex.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2haygnftw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fefjksql.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ptfpzcwb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bhiiaxgp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tlkpfeql.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ikcjwoht.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ftsjdmkm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfvnkpxd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2pcjcrxen.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nnnqodcm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yaoekwvw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lhqfgicp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2smcelaag.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wobigsvc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uexrtyee.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pljgfrhh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2aplmdjkz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vlrbclxb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2njfyzswb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qtxkkqsr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dlpxuykq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nbbtvalu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zughbufe.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ohvlviqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdroaneh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fgsutmcn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2sgpfcxsc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nwegicyy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nithibng.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2weuodaie.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hvwehbze.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2teyjjmcr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bfytcwfe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tsuteeot.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2disatbzy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jhgpnuyr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2aoroxthu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rlkpoeeq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ovmswrtr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jmkrqfbh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nvsmqixj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2bqcyvktb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hnwuangt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ybdqoral.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2czogabjd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2toznsujr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cnridcqd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ohnfdcgq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mriidsig.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fubtdork.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bjqinbwe.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tqenvyji.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mboawqjj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ehvqsxiy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ohegspze.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2tfwurbxr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jdayreug.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kywmiffr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wemnswrj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fdmfnnfx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rvfxqrll.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2urdfznlw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yxarxnpa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wghfzgrp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rydjkfjd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mdstyslr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2hmgofhdw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rscxrcrm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kzscxxsl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kamlwzxj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zclgpyrp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tcitnhqj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2snybyaiy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aaqqxpch.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2siqoxlhq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jqyelans.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jgakyxrp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xazsecfh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2elioxuhx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2yydrdeub.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dvzmpehl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mdudolux.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fkukveip.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kgfvmhnv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zdpgntwc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vwfqghaq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2octknnbt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sxmjuudb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vlcheafv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zdonbkqa.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2havspdph.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ajugruer.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2anvspziz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lbetmeze.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2btcztbpl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wxbtwxty.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zijxlkvi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2oupxumdu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cibnpgok.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fukxlewy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2yhplenjm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nkhnypwg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wvobbxbz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hlsjujbz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wjudlvsj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cbncqacj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2afflregz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qacojhmj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gsenxudg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dnuirnzj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2chmtncot.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2chyootoa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ogqozyaj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pxpnlvpj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xifdndlk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2dsfiujun.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2hstvlxyw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2scitzufu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2raggmvkv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cvsmdfmi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hngogjsb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdyyzkwi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jzttsljp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cfxeqovi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zpuhqpgs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rrrpgxgo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zpxnykta.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljakjdkd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lobkuovu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wxzipznf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2roknurtw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fbtoznuk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lsrxdifc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2btnkqkon.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eamyiqbm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cthisnjn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nkstxuie.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2aimwpiuz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lrlapxbd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2owfcmzed.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2jrzhwupw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kbjxmexs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gsrwhmpv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rlqvesox.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gqjicerw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xcrnpihg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpvlkblt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmhxbcad.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uhzlucvc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ofzukcou.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uaivhgjj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mokpzhiz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ajufhypg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2aqzlzfyx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zyaepviw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pocswpbm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wfxpdnvy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jxmyorgm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zqmfayvc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uvsndftd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nbggmvpj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqxqvywo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lerjljwo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2swyjjnpu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rzkysxgo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2cybkqwdk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2idttfbru.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lhwfoqsn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rmiclzvc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sqfzrebv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2djxyowix.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wjmsvkyc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vyqaqaiw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2imqtszqr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pvaoiggt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivzibytc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qcqaxxch.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pzoulqco.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2msnjoumq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vhvkulqt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jswtxlwc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hnwepsrb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zufaghqf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2bvgffvzd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mcmzbojz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2onrnofwf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ycorriem.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ybyyhsno.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wmohxvvx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mluiarvm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2nrybavth.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gqxjmxsf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2hitxfqqh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2napbukzi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lxoeujqi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2unvfibrs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gabgxsbh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukdqkrrj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xpcjlkil.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ruxokecn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rhgbytgt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cwzxqkrr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vhxmamrq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2favlkjfk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2omdrriyl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gxcqjwcb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wvosdjub.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kylgkoxm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2euppjnkh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2psilryps.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kcmppxyq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mlonxwpt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2scibkuen.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrzyhcwe.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rqvcgaby.html


<!-- 参考信息 -->