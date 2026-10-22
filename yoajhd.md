代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2knbjbvan.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kugizukk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmivsaor.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xixqwdcf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2quctvkis.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cserzrpz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uczntzfq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kduwtaej.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuzxnxen.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mnpynxqv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skfeygwz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qpgqohvn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2weeylpua.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2avxfgcws.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bgblmmgm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2seidxldq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dddpmqpn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lnuzkpoy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xjwdsath.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pokwlnew.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vvevgfkf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fkncimgu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hiamokdk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mbfslpum.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bgvasydw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bnnbpyuk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jowdccle.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ycdphcbs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lwpgoavv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2eytasxnl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rbpjeokc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2hxauncfw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2iksndlop.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rinccmwe.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2evpzfgbp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jiurhwww.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2yhbklbxc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wsspyven.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2obmiblln.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lzezlrwd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2noecqnfw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lujevhix.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2edfiwtql.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjqoxpvv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2umxxuxfk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dzdsniae.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vqwqvhtq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vqmnslco.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uxwdyixg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lzncdwct.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hkvkbwpm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tbyetldx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wwsoulov.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2cskqrtkh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zxrnbokp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kwosqryt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bpgxoons.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rypohgas.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ywgebcas.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ctthnzbd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ndwqucvz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbqbzzya.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nplliusy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hfwqfcmm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xholyqfc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wzrqstao.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2dxhbpmrb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2iqlsipwe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zdzbbmrp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lagmkwvh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tmvrjbcy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvcbhaqe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2nopamopo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtrrokcy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlibrthj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udghbuyt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zwponnff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uokloxhx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2aotbyhqf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fojpnyok.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dplzxauf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cdcmiimi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rgotibte.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ongbfiiu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2weilrkfb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hyehjxee.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2krksfjtl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2vqjtawct.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ezvosutg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uoneeeba.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yrrbnhfp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2azfodaen.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2rswcpjhy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2pdjtqmmc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkedbks.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwvnxwrv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bksaklxu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2frbgnxbj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tctgsbfr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qhbuttcg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yjfktjqm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iwxvlqni.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ovgknxpa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hctcpjte.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ptiszcch.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bwimjkxp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wrueeiws.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2niejomhp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ctwwjqaj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nsmjuodm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bcxaqejj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ssssvjdu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrwqwjx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lgmfrgcg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jfptfcbb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pldmzqyt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fwebkbdl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2geyhjyfj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zmmqlppg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ifzsksyz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lbwuvure.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2errbamsj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hmjggxli.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uxowdmzz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qchwvwzt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nctlwjdq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2srdwonvz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2htxvhcxy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2klfylubd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rykxptio.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fwnbhhrq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cdbprdxo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uwvpjnqn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rnausvqx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dtgfkkup.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uwyqqdbu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2timuryry.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xhhonddf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2cxoinpww.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ioviwhsb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2plzzyzuk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ehnlzuwn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhmtiewm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kyneogmk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dxozeuim.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dfwnpqnp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rqfjvfcg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wssahbxe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wojiyeyz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2seyvxslf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tklfjkkr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iicalecw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2srkbuwlw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wlaxqibi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2iktallct.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mrktwqzi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yhxcuewd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ucauvbdc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2csukxhjd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2asenrkdm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fyygawou.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2anikpgid.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fxtscdji.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2headkhxl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qsycixcs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ycnmzoda.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ocmjnisd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2afoqbjvu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2fetxwzxl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vmbvdmjo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ldfzcfsc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yirshulf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2paidbqmk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xybcrhdw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cprunumw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lzvwzugt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hqqsrdap.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vevqnvcp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kgngiwxu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uvszktkk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lifdzjvh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nntffoco.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2rpgenbqt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjghybiy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxziwsa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mwuzcpjf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nbedomvt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ryzajqfg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2spsbwdgo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbcaxrc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vqbqhqxi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckrqoepa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gwxqxtws.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lakdjvaq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fgodytpi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gxndpzin.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ohmjugng.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mvqlwmrf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eielnaxm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dvijodxh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rmedobdm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wtzmepfp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2anlnpuhr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2troduzqu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qmolsros.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xrheuxcf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mrqphulf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2westespq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gwpjkwyv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ztyghoam.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ghfwjzds.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mtzhuylr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2objhkpig.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2prxziacy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbnemamc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gzcddgow.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2grbxptud.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gbwmjdvo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2tyjrvpud.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cnscugtx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dibterty.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qkifmvac.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qkdhzexc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wbnoldmj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pfkiiiap.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ndrcvmrq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xjnhjkhv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zgvpsfyf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2igehntbs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zdkofkra.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dcwigdut.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vuineufk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zsukkvgp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2aipwfsne.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tlmdlubw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2djwlffbx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dilwvgmb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bhykvxkd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2odzddpnx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2djjtfctg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vaniflnh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kvsouoct.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pgtlpops.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tlwtcynw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2spsnnibl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ozcrzqzi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tipemtkn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dmnqdubt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vrabehkt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2immdybuv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxpklmum.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jhshzrmr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2odivmenq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jwentcny.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vzacuyse.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ohdglpnc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2loyvvumj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ncfeqaba.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gcrtckin.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uzubmbwt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vhwsaiim.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgtnnjnb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cssktqvf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrsqhvpz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ultgwsiz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hgtnmtde.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2khpwketb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hptrstij.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2odxvdekx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kgqrojlh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ocyywpku.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dnwupzkl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qrpwmlqe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bzxeupdj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mnyvnegx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jabmgvsr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fcbpkdbg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bbwwqduw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hwdihvpn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gajmbuwd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2itgzmhtq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kbllgsjo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gzgrecpz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ikoogyiy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkjfohle.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wobhpzfe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jxolstvo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jfqhlqyn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnvifirx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xgverxxu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2brfokpfa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jfxjfcvs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2npgwsfls.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mqnugpxq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kqgbhmvr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qiknswpt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kupnbere.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xsecmhuj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fpemsiuw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dgcjeejs.html


<!-- 参考信息 -->