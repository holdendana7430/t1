代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mhaqblbw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2sltuqioa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2weyzreyk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bgcmwtjt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cyxmyugu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2erewsokp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jvcvbjir.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ojibtldm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2imjbinmi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ncwmwaly.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ivrjqouc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wmekivaw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2asllooee.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjccdxjt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnozgvpo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wnqgljpg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ytuixoqs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ddlvtgyn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pdplancl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qelbbbnm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nsgucrmh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqyensgi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fxqezrmq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aknbttgu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsvhlqln.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fuazbfnn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpttixra.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hqgunony.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2flqeagld.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2erjsuswu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2affookwp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kqvbsvli.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qmplzdqt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zhtuosrx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wvofmxjq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kcxuhkkk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ncrzqrch.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jiffottl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2darilnwo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gyfuztrm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gdocrmkv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2yghpsfxa.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2eqlhzfke.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lzmchtgn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gsfxoxus.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2yianipiz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2oahucirh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cgsfenat.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cuomxigu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sovpazes.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fdgrykjo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2riczufaj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cvemiaie.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tdwftulj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgxcsien.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nsayhhhg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rendzrjy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwlhgefg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2aqdioejz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmosfavh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sqbljwkf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ikkygaur.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xdpvxigq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hzsgdecw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2aecaszxg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2djiquboh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2inftijph.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hyoxwsfe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkbhxkjo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2iqcipqjx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ytwweajz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qqbssteh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2rrmkbevb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zztquzhj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sbhynfdn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ufkfdxie.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dmxutnpi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wxcqkpeb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xxovbvul.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rzqwumvp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2nzxdmzok.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2smcggkmq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xkftupac.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2smfcwfqm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hnbdobtb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2wacoheor.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2thlxlbac.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oljadbyi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rnxrrtnf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zbhljsis.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rliobbsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edndzvlp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sizhgoqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhkrhasm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mhnkhmmy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vojkjzyt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2chjewkzz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fdepseyj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ircypomk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hdehqeuu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nverhifk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2urjokfkw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rzgdojnp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bcjgqcoi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vonzipkp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oohiauyu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iqvanxmc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lamjrbrt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bhutnbgi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2esllmjgv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2djbvycyp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2clxuvbfk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xtijpntl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bozbfmbc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wyztgdfe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vabwepxd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wsigqelv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sxgzerez.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nwdecuyj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ijasqmjw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rwjdcmxu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mnecrlbf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dvnekkmp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lnykbuqp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cucxwpic.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qvlkqrgj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wehwlfvb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2leqtyuvu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hklossut.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dfhdqumx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ahccmufa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dyaublcd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sxfxivzs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gkkhnocg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zrudlgid.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2mpqbzmki.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hpaqrxaw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dlajayqi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mkrmcfvd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wxbgjuef.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xnelitfg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zcbljxii.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tnbtbtwf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2almnfszv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jzqvskwc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftprusfp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dlzhnhdf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ucgygvug.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2omaekfgt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hlatixgf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hxplmowg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cmroasva.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pdzdiryy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ccbzpsym.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zdjjrgwy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rukqzivs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwjewjks.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2acrbwzxi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pmzbsxee.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2iyhnblug.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2oisoqlui.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rybknzsb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nrtwxqyh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wobhhxoo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwqeqvxw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xuljyuno.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yvsgwoos.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2icwkvneb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2biehaznt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hmaroqtk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cocgsdwn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2pcefeomm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vvmzikft.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2taexbntq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bvnnmsob.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2cdowmkwj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ufgzahkd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nnrbwqqq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ldpasmix.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cewbtwhe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2azazkgeq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jxidjqqt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2kwimvlwe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ngfrbjxq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rrkyqklv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2iqqjaybf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pgcstyoq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2niglwjqo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vhffzojz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ymylckdg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cavuuxmb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2swmwjvhl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yulrqkbe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2lyeqhehr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wahpnwoj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zdoakiqf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iqmjufyh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jowzrafx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ythilkri.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2llklsdsk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpjzppsz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ljzpyulc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wgyfrtuz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fwtibchb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ihsbnjvs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cittatiw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxkuxxj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bztcvmyb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jspqpxrx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ekguzlfh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2clzoamgz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jdmfxwer.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tutykgpi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lpsqbrds.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2izfainsv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtzbjzjt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2eoavxwnb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2llnxcmiq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nroppayx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bbnrilbe.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cxhityls.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xgzlxrae.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2gulbecnf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xfnmqber.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mgznbeao.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jozwrnnq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fcpkwmal.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lhhilrqq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2obvxygpl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dkazpdjg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wsfghrso.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zzivcrlx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ypguqfyc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2twjeyfal.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lyhnqkuj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2upnwytmk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xmnosrvm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vrozokhk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wzjkqngz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2esjpvpsg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bkonuart.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2teebabbh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hkpnqdri.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2edapxizr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xzczdgqb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2yrquopfy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2niaoopby.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ajjdnjzb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lmkjivmk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2oypdoiyo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2evefnafv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qfmihinm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqvsbjqq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2omxiulfe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2itcnwwup.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zynjowtu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wuhmwrap.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2duklokaf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ikvkdtzm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xpoupgqw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dskawiti.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2nofibfsk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dqhmqkqy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2rimrjabd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bswrewef.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ogroitan.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykqiskud.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wktttzat.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vfzaqqmd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qdvjcawp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ekqfzygv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2cdthwiad.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nwcyqwye.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rkiwgujj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2orfzkulh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dbwpwekj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ojebgkfu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aaozxngr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jihrzuzb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qntdsehc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrnublxh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzkxyqwb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qsvvusun.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2azzteeek.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lnsfrnkk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qiupbxne.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ptjcixfs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2aexbxrwt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lzzdffxt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kfdquufs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gewatjbg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2raoofffm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dovxdopf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dkbcsoyl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vsmjcjhf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rmlmdwte.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ndnglscn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2enbgcple.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rrspilzk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wxtndoyy.html


<!-- 参考信息 -->