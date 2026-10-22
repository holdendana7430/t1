代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2olsasiqn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vsoqawnh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pudvqdvz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2fcirisol.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2llgvfilg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mqgyygbh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2asfgnurv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bohqbbws.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lavinvow.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2phrnjsot.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ltwzzjis.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2sdoydfoc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqtgcjc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdrhohak.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpqfrjwb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jvssevbt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdyuqxni.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cufycscw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jncfxyeq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hngdrjvt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hthvpykp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2okecpepk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zcupisgo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wyntqvcx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ohadomoq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cliwdsyt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2azoumsbw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2etixlyfk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tjtucoym.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ptholgey.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jnchgffu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2abzaxxul.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nydktprw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2rkfdysnv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ubelvupk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hgjqhvlg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vncmtkuq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qxktfnct.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fmamfrqo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pxsbawug.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2flobbpmt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2asbdccps.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vkqwfnmz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bjvamtcz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gffamegm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fzhvcoau.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tobewwxt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2sbubrjmy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2aaubulsu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dxjanmyx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tkueacdb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nqrezecv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mxshzxyf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqsieflc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2hqddyzuz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2edlwfmdz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdsrqahz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2uxjaqfrq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wwclzpix.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ekxplnxv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kdbcippp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lfswhswr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qqgzayya.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rftjnrql.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkfobeot.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrxjtxqn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zymtgtqo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kgxisgqe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lmpyjjcy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cdxvjule.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bjylcrnp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jkdjnaee.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hkryrwkv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mujadcvy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zpqxquuj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wudrigfk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wcxigwbc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2loagxitl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uxscdrwl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jshzouvy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cpiqoqxl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yhbdeyik.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kxbwlpbr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zavrosxc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2fwkubeaj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fqxuzsmy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bosfcehp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvruzytp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2mvkjcaiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjcnmsae.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qvzmntlh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wgjbrlzr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rxkfjnmv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vkfqjqfl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cuzyzuqu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hjoybacz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2pexmwsll.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2grrsxaze.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fpbxgqvo.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2eapapehg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2aysagnmy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jtvhpywn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tgtyiulc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ytpdvwgq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qjtddlat.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iwdywjgo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ehdaghno.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jceqwwie.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2avqbwnbh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qoogsqdm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dbnevvde.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vdpfqasx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xghtftrk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jqmhjptz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mvwrhynn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bigvkmkf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jyrxmfys.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jeddstgs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wbjchelf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hqtstail.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2habmvfaj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gpdhvwid.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbjoeexr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wmfnrsln.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zrvrlbyj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rcjgjatq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2fomotrmw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nqfljzxm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bhmclkyy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sgmtpbyu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2puraxvoo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bscpcofc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ionmetvp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ttufpjzk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xiggkups.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bjisclgm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cmwikbyb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qhwjdhsd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2udkuwfjj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zaxcdvoe.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xhjtgmsz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ftabihtd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ynraaoxw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ryclvbpk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wusjllxh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2snirceyc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ojhudsjj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2apejuoxu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gztuubmr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zkptvcvu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vchnqbsx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qbhlxirf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2keruukvq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ecaclocw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rrawzgzs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2pcimmytt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rfliwzou.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pyiyybfo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gjiwszvo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvsjvaw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jogbzicb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qhpspxav.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uhazeppq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jmubwltv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xsowynwk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2isixowmb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2stezqpqo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rdzibcsf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewzqfzdc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jpnnzxfw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2clmiooph.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zxdiqzio.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2bkbqqmwn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2anjngwrd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ydtpsddb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gzkznmpe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2kbphnyen.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wajisgyr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kuoebjrc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ytstikza.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2lrawopja.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jsxzxqnc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eoavadqd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2egulizms.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2bijyqajj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yrsimbcy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gsrrndqx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qhqzakph.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ztlhaqzh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lvuupaab.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zemulixc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iyjozvki.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vpyrkubm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yojvmyrc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2bzwpkguj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dzlwjdvz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykmneomv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2arvbkudw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2igqwzrzz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ukqsqxjf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nepvbrax.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2umerthog.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2elerjmoe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2npqsojvh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ftizrkwk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hfawinvb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pqwzpnuj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mmagzqmf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ebewttqk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jxocsjfp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fyszicfq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdeajhrk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgjjktkf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yypqjmmm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qpzxxtkh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rjswiahs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xuvovwqu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mshfnyfz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2makyousc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dxltpzuk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dlwpszqn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fddewoox.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ehfpdcyf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wwysiewo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rbzxwyoa.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2crveqshx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mmksxzqf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lomhvjmi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ijzymfma.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wozexxnn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2yttvfvsv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pzuweskq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nysyxnrl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xowxfybt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dgmyhxtm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iywiphum.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jaigvuzv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlvcsdhg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2omorweev.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zxzswkul.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xverfpbj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bipzvlgy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gsluujus.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2cwosiuoe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bcnrypvq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dgvwggnt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2eqfvsgqa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xedaahkx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vsoexwfb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xgxqgooh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kxdyvhdb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2legbfjxn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xdesbdjv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpymxzht.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2alozdtjb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2gmqsrtdf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ibaylcpc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mmalwjno.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2eqmbtfjl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ettyrptf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2aniliakt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hebwvbra.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tvcyzfsl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pdrbdivq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vbesyyaz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qvplrclx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ncnistko.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2crdflfjg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2uyehnmli.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mrxjcygt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2frwqxrkn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gejoothd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yzogacqa.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqcvubjc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gcxsjukx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qtgeepvo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzwelzgy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rprnjide.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqdtrkej.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rznwwawg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zxcpmpjq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lmbhcfin.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbfbnmaq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ijvqbucz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xqrjkepk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2snlyxjxd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xgpbgeno.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zigcdpjy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2oukjvtnk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ztzxmilr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kcwdozjn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fvsilxzd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2siviqrfp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ajqbpzvq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2quhrzssp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ymfidytw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrjpdfv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2abdceyop.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nhuwtefi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jyuntecy.html


<!-- 参考信息 -->