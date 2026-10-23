代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3txtninbd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mawpplnt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzldimfw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3pegzxbvv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lhrratyt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mfpirayi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3eowergut.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nznltydp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xtatzspi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pfinmtgg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xilkruxr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vwzwwmio.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kgjjodri.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jzwyrhzk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3risxhdmw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3vsvqtfeo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ykwialcn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3reduqkam.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3tpwgxsty.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vtdrmgtg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3oienmsgo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ogjiirwb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ghjhbyne.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3eaqeefoy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3nkqfncgl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3teqtghpl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hxvzcgti.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qvlbfcla.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rksgbevz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xgvophiu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bnkjnioi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3btwopmyi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3musjeglr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jovsefnw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zlctlgbq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywkhvbwc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qlxahkvv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3yhxzacnv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vqmvfmsx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rrlueury.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfibyvah.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3olwefmqn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nzutgqee.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hefuswwz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3idqzxrad.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xpdqnqnx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3aswrbmgq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xqdliqlb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3cuuuglfu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ognonpro.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fjszxrnl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jgprconv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hwhtzunw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yphjqwed.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kirnejfv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3psofcjtc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ztspzklv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3puiwosju.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mzpsjghj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qlatifos.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hpmjyyla.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3fjhmgzqq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gkzsdibp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cdxjwrou.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mwlgitlv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wnkjlybd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgswxvix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgnvsuol.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ftupumeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txnuumwb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hczrmggi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3viffgmki.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3woighmfc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xqxoiyvw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3yylfnigy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rydfnqau.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3bzhtunnm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3opqitbas.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qhuxysrh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ollzbzhz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gphhzvye.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zoiuxfsn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tgmbtslm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wuehkego.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqejzamj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tqzmytbd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lcoedpao.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nanvwrvo.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lfbuxtjp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wxslmixd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3edigkbqq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kglrkdzb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qzphauoz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ltyabpwm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cmitfhkh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vbuvlbox.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ljtuweva.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3szoacybp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mlrspqok.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfwohedo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vlqvbpzh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rwzoseme.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tpirsckv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3akncglwv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ohrboxau.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qyixdxnx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kqclbqxu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ifztzqes.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ubfinlsu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gsumrgpp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3abwpoakq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3nkneczrx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3iwcovszk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ucjkazyg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ksxmafni.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zycaiqai.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dhkfebit.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kqrksuau.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gwnbhcxc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zppqadws.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lknoucyk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3deuwoeef.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yikzrswd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dvyseibt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lhurrvtv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3iahglmdu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pazjteim.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kjsboqdd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3coxfqnqd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3enxaeele.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vfyapfyr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kbcpbyjl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ezonnujj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zirhvubz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dewfvdks.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3owolesnw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mmgifmyn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3cyijfvwf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3hwcxowsi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qzoeqgfp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3sxqoddfs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3avwqgynp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mahodhdw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bqsdaupq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kaqgjkky.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kfabdtis.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fxlrwayd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kafpvqzi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uexpebvp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hmrqydlb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hxcizqmx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3halxsgkc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3sfyclihr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hllwxlnu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3uqxrpkcb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3flmxbfyz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3clqyxeth.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3etlwescj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cvajgiab.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3shfhtxmg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lpmgrpai.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hngkrlxm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3chcocfba.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hrlsvanl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qmcfsmsb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kxwhaoxh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vzkpjbyo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pwvmmrby.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3kbyirwwa.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3vqvwdtdi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lbkpscfb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3smkgniej.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sahdidxf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lietheqq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3errqpbpr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bxzrwicu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kienpxjv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3vajwzxdq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ezyoduoz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cdnnvasj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3heyhqiml.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mtpsonaz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qyltvdby.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ddplqipw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3eqrtxbtr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dhgtwtkf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wphpdkdt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3falmzhtr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sxsrheeb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pitftbxa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjavqlpa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfwsehu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qwihdwkw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfojwgik.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hymmansu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qkvqbuqg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ublhxery.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wojexcoy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3alwpcyhw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ffiuijyy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dljskpan.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3aekuvcnu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3nkortwna.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lrjlcsja.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3arnzfylg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ezgfhlmm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3licprqet.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mlsgswva.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3anznccie.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oqrnoupn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3lryyolyt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3iujmvwkd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tovcnsow.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mrkjmdpl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hltltofp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vvvnixkt.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3nyjmicqq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ysdxafjg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3uhzqyibg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yrfxmapx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3oytkodrm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3feeqsamo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3dzbuegio.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yfgwafym.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wdkmdduu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3uebxdqog.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qbyuoxsd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3uxxhkjqf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ttzbigpx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dbzudzmr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kfhjrxkh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zcmpvbse.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kdqyzpxi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jybraoyv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gnurbqmn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lxbgikvi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vwkjmqjk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qtqsywxz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fzcsvjym.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tfzbzops.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hvcrofvx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jswgxkev.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ucaskkec.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fnwfnzah.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iglmwzkw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cjhcwrcl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3nknwwqak.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3cbnwcuhw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yzpoahii.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3eckdcnhg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ngbssawl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3inobzstg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tniuiwxm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ruoxixwb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tysivycs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3brscapbo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bvfkwcjt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3byujrjln.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yzgdxque.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3htkasdhc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lyrxebvl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3iyrqcoox.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zsmwbncf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3yafjqfyx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3icrpiewa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qyvoabkv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ddvevurc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hvthwisr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lhdvfdsq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3skknsito.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bomsaruw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmjubmg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tjtjfmzk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3oihbffiv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3smaomhak.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gnbcraum.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rkvyycrh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ojsodzip.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wqtqrfbo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wkqhoyhv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qggvotqv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cecseptm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nhqniwdg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jmlhdpoi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3yqjclirw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mmyhmpvr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3tylfcohm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ohfacpbz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lvznglws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pakvzjgs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3knszzcxr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oklysraj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zujuvzoj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fpyirsrk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eiccfgrz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ykevglca.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yxetqyba.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3prdgphyi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wugtdcbj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ysyumnnj.html


<!-- 参考信息 -->