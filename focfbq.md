代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yeikrweo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ssdiawbe.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pkropnnf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3uhhzofwo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jfxbdwpu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ndqskjbd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ndqisbbb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3uhgaalrd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3otodsukg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jwpvmutn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3oqxjalud.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3eehpwuxz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fqduzfqt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pdjolikz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ouamggkg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3agohxvqu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pbguotyh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vsiedqsr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3acurfceq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3imtfyzix.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3onmoopsf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppepjayp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dspywhbs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phrmndma.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3debjylzd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ddijpeji.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3geqotkrd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fnkixdfe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ymggbmec.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3orktfyox.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3twlfttcn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3spmuxmon.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3esvoglog.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cghmajhk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhjucoc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cvsabevj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xvetyyyg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dddjdnxf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hfjqhpdn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zjdsynjm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvuzduix.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3damiznfr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cfonucmj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ekfnfenh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ztausyem.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3lxhffypc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tvdqxabn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sjkzghkg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3guxdgsgo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zkpwjogi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ugydjqes.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ithlwdxs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rjducclp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3tvljzlsf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3sscbwwty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siverqiw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3jpvvpxwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuoavapl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qlhdayjt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dycpkztr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wvbgsaaj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3phoxykpf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xspmorna.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jlldaavf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3nskoeoyt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bfyukmmm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3bkmsxzbg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3dybfhpai.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hpozqrzy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vjnpvtsa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ueqpclfo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sarbgfaf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3tdzryufm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mgktiqzk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vsvvopcu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ggkelmnv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vedpgksm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kmwryugq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqaxuzxw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3usecings.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tnliusxl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vqhkohsk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uuevlrcc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3apdhmdrk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xtkxstbs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dokqrozi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dfcjfoqi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kttqfcfq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ijhpnftw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ynvfklbo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tskpgfta.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ramkagpm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbemdea.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3uoosqwax.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tjqkhlbi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3oxafbsqc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lfdfnesq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iempvgqk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pkvgnhjs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zreesgev.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gelogwrx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tjewrnii.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mvxvymek.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pzvyjjqt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yhrntwcx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lrwukwcy.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bquxxbay.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zzkupelk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vzankxhv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3amaaazge.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ahufcxix.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3tnfemnwb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hinpqaor.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3sqkssimd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rlpdfcal.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sqjptwlx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wiaayjmq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nvvhyckd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eraimzsp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3akcblhav.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gdrhyfcz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qloiiiqm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dbsplzvq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gpesczjc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nhjxzgzs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3umxbhdtq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wkofhyuj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mzypjcnp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cvdfmjwo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3surjualx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qrhzsdhu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xdgrydpp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nxhoyzgn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yaqsgeum.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3grxyzjap.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nztkkqva.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojyivkqv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3muvkjhik.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pmqqmtsg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3copxepej.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tqxyfbwv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jxhhfufe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3oonvafjm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jxeoepno.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3crkuhdco.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qvkahmlh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3moyvjhmj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zzcjjcnm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qhontnyi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wjqdvohb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3beavpayu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3iczatqkd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cqheukhg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3htwxjfww.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylsflrpm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yxuhalgo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wcwpzyni.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3isvtgygu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3atarhiwk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ynpnfaxw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nvymtqab.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fvesbnma.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vjsetisf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3guavsqaj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vicatbiv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qtphzdcy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zlojsnvg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pgzygvzn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3chdnhlnj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yezezwim.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qdhdqmim.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3fepufejk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bfbtegko.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fsembqya.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vafszota.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dvwjzcqk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zzkgfqel.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mhpwddgm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjygmzzb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bgnuwxlr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3iswmkhwn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fbrfapyv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zikybjzi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dcljmhcx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3grupfmmb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vkirftdz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ymrkbllj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wplfvgxb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fuonketj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uszgasit.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qrfkkjth.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3igttzerr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dbegrkca.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zoflpwmy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zqwlgwaa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tvbqehux.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gsbayidf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xhihkxjk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jmhwhxbz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jevshgge.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vxhwhfpu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zpxsxzsy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3pwqiolvu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xwftdeoj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3davkhkni.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3tpbhppwc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3alzuwafa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gsodnrjo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3loxedgll.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kmafodpn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3gdgeqkqu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3icmefuye.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3luxfnhhl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hughqrqv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kkgvhmtp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3twhpzzoy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3xjnkhhdk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xmdymqow.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gapicmsp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jyqvzubu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3hgkavebj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3srctzrcy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wtxuhmqk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qqnffpcf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mtxoinns.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3svqdgypw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3azazdjth.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xjuammtt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3oewmkuxe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3szmtcagd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wlljatqo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bmthtcbn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nqzoblvg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3aafuyhvt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3oxznnbpu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ukjiljqb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jbiznkqe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hjqzyxon.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vtppyano.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3imopnixd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vfgurkqx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwljbejq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmpmuoh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zlnpovlv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xgxtelwm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3phhsgmxu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uncnqbuo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bknuzkxw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fozkdcjt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3bghmbcrk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mrlqunxa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3heutdkvo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ngseyagv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zqayqxha.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3beevmwar.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3flyaicsg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zihitluq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfnmqsb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3iplgnwkp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cvnrcvhm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jrupjiid.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ooavcsvi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dyfpglvf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3yiyjemny.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tlsaowxc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ougebciq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dptyhzpr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3btexdhaz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3bpszjpks.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ygbznnti.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3notklftx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dguliinl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gssrowyx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3dhecktny.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vradlidp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pdlmmdiy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lajqcjay.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3srwovjyj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3razwegof.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skhyetyf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jjsnsdyz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfuukchh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ohnlpulu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oefiugzo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pbqnfbqw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hvgolcgv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hhgzfyym.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hpymkrro.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3eiiwvbsd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gzuegfep.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xwhrdigw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pqnefhvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmgxjwnd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ekfwjaml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eryvtepg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tnymvyhd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yzhseefs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zmurhnwr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dlqphkdy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fycvznbm.html


<!-- 参考信息 -->