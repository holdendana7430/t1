代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2faupctmb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2nzmqwilx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2anqqykjw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2cbvwtbyf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kcofrvld.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gzlzmzgp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kznglcyt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xrqxqtjw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qkjqrtlj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbyaudxw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hysosfnj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gqiwddke.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2midglunc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hnxqsnts.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2noxdveyz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nenbaxal.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjhifrib.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjtpzqix.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2eijoeipz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cgeriiyg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2npieczgx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2fhsogzti.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2klldckdz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vpbflwrq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bzqgqkwv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ubfqdepi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lgmhglme.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rtmqjccz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2immtwznp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qwkeblas.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vusjdirs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2frzfinuk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2acdfgvov.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nepvyecq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tcmyzjsk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fudwnmjv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2irryzyou.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zsqoijxm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2nfsatscn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2yddgwled.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2yeousqde.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2rmngjqyc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2olpuwoup.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jmigqrio.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sxwdrari.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dmjtqlbt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bzpzboxg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2thdaaffy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2uygtzqxl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vlpvilft.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ewjijzgl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2zghsdzkm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lqxlaagg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zjlrrszr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2raxssqbn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sksvarli.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrbtzvuq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ajrbtgvr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yclcrqpy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dbukrqss.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2totqhzlf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2cugbgrht.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2evdzslda.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ywlqwkal.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pgnsqcki.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bplbpyer.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2gzxtyarj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ubsegdup.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ajfptmnt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dgqidiqc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wpsjjnfh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2dsoqlaep.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eirawbbr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuhpgrek.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2quutsbvh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uvhatect.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mmkhfofu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2txxxgzgc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ojozvydj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fjnqnrtx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wxighinv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2epprjiwn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2nqqnuwvt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vxeqcsuc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2njsiuagl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2iwplwblw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmcamdfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hveuscry.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pnreosss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyoranwa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2znhijfke.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hhnfbtei.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2komjlljm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qviodnig.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2adzjsnwy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2twldthfm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2nikpfrmu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2elqwbrfb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dxdbqevl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2cndjvbux.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qetcxedb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2chhfvoux.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvaxdbpb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dlvkvvqi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jhopyjlm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2txsldkcd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gtyiuzsb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmhamucr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wqqdjfkq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jsvgpure.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2slovonxi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gdckewji.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2thsskwmf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2spytsely.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pdpdxueo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ginkrqum.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2koiyzsre.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hhshmzqs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dvjrphrd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2whbosnzk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yexdlbqu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wwprljqq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2riaijvvv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2iialzepo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zsamppbd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nxkitkyf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lmnbqzuq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zexvhbsx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nglkifke.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2akdcptrj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2tcibfeqn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ktycugyr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qosdskyf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2abjnnsnl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nnvyibpm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qgwzxjnd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wszjeybb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jipfdnfl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cbkouwgw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bcurupna.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jiqgfzwg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqbfpdxm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2sbiabzlh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2nhoexsvx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gbeghzdz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vlzxzksy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vgxyjftu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kmuhzvqg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cfuzhudq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rghtatyp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rekwelqb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mjrzqewo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kafaqlgn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2piviwvjt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2afsiajsa.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ebxnomzr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zqwczwbp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zdppzlrg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gokfvyam.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2knubeybo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rzulbkdf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehrkghas.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2aaegfgxy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zabxmnxv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cqgaqfyt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2oofjirzk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hoeaqsmz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vowxqbgv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hytikisb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2prsjtsao.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lvfzbxag.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uqnbzfhb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2szhiyfxk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2envydyoh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2itzndfiu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mogmhaje.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tuitkkft.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uwkaqyyy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ylvlieua.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nqswvsqa.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mvsfyofa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fpwwkpwv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ogomdvip.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mswankwj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zqzzwfml.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lhrkwdup.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ndvyfooy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gewnfage.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tzxkhyed.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2eieorqjh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jrvutjkf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jntscqkv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tgixfkyr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zienhojb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ersijjzs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ywoyqmdx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2egafdrjv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2yonnihao.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2eewrbhjf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sykncpki.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nhjkekyx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xsuuyxxf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vxkrrvbm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gbjxoees.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2nbvveefv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ukjgdnsa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2elqtfvjx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mvvizvwv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jwllrucv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2syriyhmh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ulfcggtm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2shcieoff.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xfzovojn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tfbemizg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mbgyecsk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2thapvhxs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wtewhwht.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mnibwvnx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2rzczewme.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jyxchknp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qzstaskd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nuhmpixd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xnhabfoh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qjnnzzgz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bzfyodfp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sqpyqqbg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dzzyiygs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eigbjoqd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rvrshjjt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kdjbzplk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gufwsree.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fsgfcadx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2btxmxbgr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vsnmuwmt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2azvoptlo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhpvzebp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibcdefmu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2scibnyvl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kcnwgmit.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nimahesl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbhbpafj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2adveeotm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vayecriv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2daxwyeqw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cfweioki.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dvlsmylv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rkqtdnjp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pyjwqsxs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pbtrcqxs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yndtzful.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pzjctfgb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gpdqjqvs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cjarlymx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wogrsmmg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2utegocpw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ntiolqwl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2edpewnqn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fcvahaoe.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2cdvopgkk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rfhoqsds.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jcpusfen.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mqvpngtj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2yhomlxxz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qcshzxcu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2adqyntvj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ezlkgljx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2kdkdexbt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dtwppdxw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xatvasyw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2idttayaw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ynkgwtuf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2fknziiod.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nlrfxfzo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwxzsxk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ntunkjlg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fdskjnwe.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ahnnrqkt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ywuunpcj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eggnufgp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fqkehttl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ufecjiel.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2gtafnrpq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wcgahilq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dxnjfqjy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wqvxmncu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2sjploezb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rvkowezc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2olmrpdqq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ujgkhlzi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vafrblen.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2igqiynvn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zugjrphx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xzcixttc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qzdbfzlm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ythddpjl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jyxuyoib.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijsqydfs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rexvmckc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fbhiztje.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xbjmqhtt.html


<!-- 参考信息 -->