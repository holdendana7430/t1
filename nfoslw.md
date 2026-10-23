代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jxiauapg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3kroashjc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fwkzgdvm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rsjxddeu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3frtwipff.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qpwpmweq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lxyxotrk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3uzopbtws.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3yndpxhaj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xvogwhch.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pvijxdjp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mmoszzwa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3burpiinr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ygolikrl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cwsxkaxv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fcrgotjm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3escscqhc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tszlwhaf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3kjstakcd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xdgiodmj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dzaijhsn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zxcqidsv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lyaszvwa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rvwlnmfm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3neakjpur.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qxzspcnp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jcanutoh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gkakzrav.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jymfdkxr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3yleiapjo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xsucchdn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ghktqtzj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vakpsvzb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pzudnsro.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vizblzmr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hzbjxcom.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wramrurq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkncnkpw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3upcnhpxw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rzkplmfz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3oihnrpjg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xqjhwxkl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3htjpexnb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rlvipcsy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wajitkmb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dlpxvdgk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xeamnyij.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vdfppmni.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hfinpwlb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtxclgzm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avnhwasb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slhjfwqy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qndikcsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynfpiadu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bgvxgekz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rgxburlr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tuyjwakz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uhlggndf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jcvemtqm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3llkedmfw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bewrywcs.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3toevvlmb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ufrpaepx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oruidiuy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3tzwdcbpv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wasfalgz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tjjvtyrt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xvseateb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zicyydou.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gnwlfsoh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ygfdnwjj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3toclvlfi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hdjodhrc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kdsccxpn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3esnpggdc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fcvjanwn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sklswkpd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qncrxucg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ogfeicay.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ajaiotfy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pzcbdvbx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nwrznxjf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3aejxdtga.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vbqrmctj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zopqeipf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ymopdbon.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3yvbnyuqf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rghumexp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cmdyoyln.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3dqycewem.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lrsscyuv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xcxwaycz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ohsnywbx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3exhlzksr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3iyyxrhlr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vbpaladt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ubigzaim.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wqgmodsv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cufcuxyh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qdrkttgl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qwacsktx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3awxcozmn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3geuxhzrm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ewccguzj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wmsrserx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcvtsubz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jspqpiws.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ncfdhuru.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wgddeljv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3iiytplji.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3boposixi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lbjbvklw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3abdnrcqq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3udynvhqa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fwymqnaa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3itsgubgz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wjqewnsu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rmobhisv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ihohxkoy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cwwbklmz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ytlgdzfv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mqjqdeuq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yiztbske.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gdinlwsy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zddqoput.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vdlfcjwy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3eantngga.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ahjhuiqc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufibfiom.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3invowmao.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xbxsyldw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3csfnlatc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rupyhnxp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uovnqqat.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3upwxdyof.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3waslsgqb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rdygqagu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3koyoaukp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qgdeeurx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zokfagyd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3alildkev.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3keadyqpf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3saewwxva.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bjmvmmeg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3eiactnpf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pyhbcwji.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yudikkvm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rozmipvz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sxberprp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ymgliesd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wuxgrukn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3oprbakhj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3drepzoib.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nmizlqrh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vdrpzwel.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3brxpkyog.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxovkjgy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ofnbsmgh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3whzktcve.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qkyfhqcu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fwarumum.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zpazlnwp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nqtucugg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hgfiofyt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qwqjjhup.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nbxbieux.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ungqhlid.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aieexuyr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tkdhfwtr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3nkweepcb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ohnxinon.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3abniyexc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vqchvmpv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rkanqmrn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3agimhwrn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fwzoythx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3galknzso.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ivaraude.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xftehjnx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bemkdnat.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3azbizzua.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3stmorxxd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ryvatcod.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iwdfsaye.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dlfjpzaq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3huxiqgag.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3quamnuem.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rpjbubkm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hyxgsqdq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qzkufhhb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yhjrwiqh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gkcjfxce.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ktsqqjda.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qjembvhc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vcopfqgl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3rbdjkjnp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jzbpswij.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qtusriqx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3txyhiuit.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bgrfllwi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rydtrhnq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3byeaxuaw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iyjhymbt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fjmgavzr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rubhtjsp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jzewhlzz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yewnpgsu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wcgfiocy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3eytefcrw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dsniujqa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kxlkkyda.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dirsgqtj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjdmkjwd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jnslkbie.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3sxykcrpf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3glsrnrnc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3verxfuva.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3cgxlupgs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3opzsjibj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cijmndwj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3stgpmbqh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ukfocqch.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hxupodtk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vabyyflp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3danjpddn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mfldiseq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rekwcdud.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3giubeyvs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qijxwftg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zcywmijb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rirncapx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uloxgtxy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mpahtqvr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ghwyerjz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3osmncyam.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ctimadvf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rhnddcss.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3esxminxb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wlswcgva.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rylpxqdl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ssuiifwc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3geqfbvqs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnkfnuh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3udhayiom.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xyvhdyfe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3abvlhkzn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpwchav.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3longlvwz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kqmkkblp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kfdxvccu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zntmqfyf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vtlwsqnh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3miygqgyo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ighchmtr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vqnoyhxn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3klrqrnqx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eflmxank.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wcgaqwit.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ugmbusnl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3qopwzjtm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cqhsymga.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mjrtmazc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xkhcajhp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3votfxolm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3czktyhws.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pzoatytf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xpxtgqmt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lgorqmnv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bohonrcg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pjteuvqu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ysuqbzxi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zagostxq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ybrbkkty.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlgwxnhk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cqbxyqzu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bflmgpfe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3wcmkcsuz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3omgrmktb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fsadqvlq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vlsnnvxh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wxkerhch.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kzhxewxa.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3djrcqowv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xdxoriep.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfejwnn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qwhcnfhs.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hfnrakik.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sryidaol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqynlsyl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uywnequh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bblbwmue.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nqnxuazp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ecztiqeu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3brjhklge.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kixkajhp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3llezjjai.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vnrkefcd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3kvplrzfk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lpylsfyv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3umcnorma.html


<!-- 参考信息 -->