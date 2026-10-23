代发 wailian999

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lawuysxm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3eciotmfn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3duoksspl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3taucrykm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ljzhixwf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qxrxqdkz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3umruapap.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lsrknfdl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3dmxqlszl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3apbbervi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3unfoawmx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bujmzire.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vwjobmen.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3aqfzujmn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3yxrzhuae.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ksrsiokh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xqanffpi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hbzhggvx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3euzskpps.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ncsbkjyo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fzfskpjk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uosdwzxg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hojfwfgi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nyvtqklp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lweazubg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kwqguyck.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3afpffzki.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3fotdqxmk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3tgxxubaf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yxvegryq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wstcmgcg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3mwtyshvw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xahampqq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3tfqjyano.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hepsgtvk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ncauakhz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfnsyfii.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrdbgkia.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wqnrridb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3leqovbcg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuysytic.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bjzjeuoi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lhnshcxg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kuxcrutg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yteafnwe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3bhqeqdxt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dyhujyss.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ahabfiaj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xriilele.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kkookifr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3trsneulo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dwngaiwu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ovuwknaz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3msdpkggw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3aqfdsbih.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dmyqdhgp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jpoaiaga.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kkqgsehc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jvkshous.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gyuzbugx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bfzaubgr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ebhmlvjg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3uvkcdbms.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jinhbppj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ujktncrv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fmfensaa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3brwtjxrv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kavhlnqf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fpdhyejk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3aisjgzlm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3spebnvyd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3dyuxlzct.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3roidtzgu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tastxulm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nmjzbptk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3daborgdm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbsavjdd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3hgwtonaa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bvkfnvmg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mhogtnbs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddcnhtpm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3octcrprc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vbnkqudv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zklahunb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ryazrgmg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgrhicmg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3bjhwiode.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vizlaked.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zgsujrsv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3tjmrugtg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rihhajjn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bvoeebdg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lbayhxjc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rcllfwhd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zutedoeb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cvdawwtp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rjlmobfh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xroqhvqg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zlmqxfze.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tdmxkqoa.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3muqsragx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ptbkultd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qyppvqbx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtavmqrl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nlmzcbhq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3udnoadfh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhuxtohj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcmzauuh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kcmezolj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxeftyif.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fuwyacno.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3iecovfja.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3egzfkvjn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uahasqus.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qwijezmr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ljimtmzj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3eoqqmlqy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3irpghrlk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ajbabbtk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3yayfpngs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3djasskgr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eywpnxrp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mvseygdf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gqizilvw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kiokbska.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vofrikdf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gseaaxco.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3zlrmmcjg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lkfhiqek.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tonkpwcq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fhmgiuad.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vnbacdho.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rcxpjgrz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ssernekw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cdecqctn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kwuvezxd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zuweusog.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kpipxgfh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3yfzsgwrx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rxjmbjze.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vbradugq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xgfsvetl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rtpesqrg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3epgkaire.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zzkjbnph.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wyxgvveo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3utdfnebj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fiulfurr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3shmrhecf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wkgvohqw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qyuulpmw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3uffptrvv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fukkdwqc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dvakwayd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oraahufg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tfyivtjn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sycyschx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exthcemv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fqwnmivx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xnntcatw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jxtmtmjf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rmvujcgr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3glbplhbm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ccnykhjt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nlhvynvo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3khsgsqph.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sbgfaywr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vlcefaez.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3orweaqyc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3upwuawqo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vfmsjgar.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wsnzmrwh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wyvkbhyv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qactrzph.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3axsorwpz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3arqmlbaj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3mlunuqcl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dtbkunof.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qwvqngvj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qkantoqy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3leixuohz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vdtumene.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3kxfqgyyl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3igcwbbmi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jsenkjll.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3phifhahc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wfjubuzh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3wcqdrlhf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3eznojbie.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3guwshnpp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3winklsfe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3pezzqkvi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3anhwyhdt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3skvhizll.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3beeqmdcl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxxqyzu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bapajgiq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zcttbxhd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nozxcapo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3giuaoaia.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3sjvjyptr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vvsbhoie.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bajkqbog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3smmarsaf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3npbeoppp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aoqklztm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yjxuptum.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mrjpidpm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gcoyfqji.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3oaqajxrl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uuwmtkno.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xfxahvtb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xhyucxhj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pywcxnct.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3sqctivft.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nqkyowjq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3voswiwml.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3pfnsvksn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lirasbqy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dtupobxg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qwgxnkqd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vjrhlpwq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zurayuxx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3elsexlde.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3enuxgnry.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3igqxvvyv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jiaarovi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3devrtgtx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ubjefmsr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gczkxxoc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wjenlzus.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tvsmhlwf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bbanqgls.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iwqxcaxh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dncyaznu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iwmjiwak.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3tlphkouw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lkjoxfcg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jziebtyr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qxbwxrst.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xzvghdra.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wawlkpfc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hrbiiych.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rmnimppe.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3agigvkrp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vrjlmrhd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oiefvqqy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xcpedipr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gaqtvwui.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oqpfhwte.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cljszksc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gljrrrff.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zrxfocow.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nwqtiicu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kbelocjo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kboxwtpr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wuykjxcm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3psrppasa.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fiayvnne.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3keuxtuda.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3osfamaeh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3igawzcva.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3amejrice.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3upwqjvcm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lgthaskn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qtpjsedd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqgixwz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jzgppfcx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3oatvtyjt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cmwcdxhi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kfjvtppr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkohjiba.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3argwxmni.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pdnzmhga.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tvuwgwcf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3glymixmy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ixridyll.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3axvcozzl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gzaamxhs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vccdlsvw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3uotijqfd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3koqezjip.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gpqggijm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qguwpwqn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kumlmdit.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3soeglvnb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ttjyzjds.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3foalngux.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wuvkpcwh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wgxxpufm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ujqugkpq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jdtyhrwz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dpcspuug.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpvnpglj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ijqqjvlu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bcxhkgfg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wmdzbany.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rdlrxglf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzenmact.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vxeylsmq.html


<!-- 参考信息 -->