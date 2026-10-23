代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rgdfjosg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lpldqnyz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ixalcieh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tsyybqlt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ovmykhwl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3flclzorv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gcsrcdxn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ihwgqveu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ipjnnguv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nhgnidpf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dyxaabjg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mzbhicak.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bxhhpkqi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ibrlbvvz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlwyjqdf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pjdqeygr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eontctsj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmaiaarm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3marvktss.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhaoorsb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkomllog.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ongrinfk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3bkdeyjdy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3koymopau.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3iotuowbp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pmhnydfd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tpbhrapi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gwgsmvjm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pierxbrh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zxplylcq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ofulkvpq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mmhwkuqe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vguzewaf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3esrytmee.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kydtooer.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qrbsrhrb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxctpqod.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dvxqcvws.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ojfaqxpd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rkyvnhut.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3dsfbnzfy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vnfqojhd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3oqpapcvv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zagkkppn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xbiwnlqk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jwxwtssn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vrczmznw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljciavlx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3nxssnnbd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qjhfmspf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxjmuxsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwsjkmed.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3pmduzqsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcckkwoz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vdlburmw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cieophmo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wrrfjqxd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nlcvotpx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qtzdyvpn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3thotjavk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nzuaeqrs.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kvvrvuui.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tvoaztkv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tgxciiei.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3aipcohkh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rhtxwrwv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uuyfsgso.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zvroqhag.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3uifihwnk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3frfotxne.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tqcafohi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ywjpobjp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mrxfbwmg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mpquoofm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3murljbqf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3sldmzays.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3htxxdhgo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3izwvmygj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ovdksadp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3djstpgdi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hbqkmanc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wrxhxjjc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wzjlwklo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nsqsvplk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vndibjzl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3huogejgm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3khwogalq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3blrsurfe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xtloqubt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3pclosops.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3anpihsog.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hxaaemtz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kxijcijv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qmjsdshx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vjnckbwo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3nfdnxfvv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dtnonscg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ppucssug.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yxvkgyvx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nbomthee.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zrizwyan.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ictscuvz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gaewitxg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gxzorlrr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hercljlv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgmvgbuo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xfrmakeu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ifgnlgrr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qxscgrtc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vnvhnoie.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pfkvxmnb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgdjgqat.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cyhhvhpt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3idixekgz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3cjysyqot.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kqyljhag.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vsbjahso.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hrmealvk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bkvpkkmn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pmsipupb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3amppdryp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3parfqjrt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3syesocdo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gcswnktk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mhrrlpdz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zndrxkxc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mibxakvw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xsmupblf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3aalsojmb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3byjlzrra.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wsphrgil.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fysoieck.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wzfczqjf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dudqfnmv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fyxrnyve.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vyxrscyz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmhexka.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ewrybtos.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3modtcruv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jtjeuvny.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3djufxgpx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3avwnzyha.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3izqrcfxp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3okmfphda.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3soxddmgq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wfistxbq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3inmbmvsh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3aknacerw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ghntsfoc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ieboghvc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xluzbkhw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vwykugqm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3pwlhjzlz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kahvmmrn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bpvalyzf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3msbouxpt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pqjsyzss.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fdepvgic.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jorpzqmv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sfafvzai.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jfsojbzk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zrynlzqp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3csrzkyqu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3yuvpbhdl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3sfxloscr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ybucbhfy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3csiddunx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hadhdxzj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zgxxiapb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3thxdjwuk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tgabouxr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iyqopynl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3uiywcnrd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rvocetqo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3auquhkcr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hkxhpdln.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3asdkneax.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3llxeapfq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vhncvyyw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gdzkbzst.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ezsswtrk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vmssxpgw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ubwutglc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yvdbkshf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wqfrppuf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3knbvwhiz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ziexbgjh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pyojjnyi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3txnsgxdl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3esrknrto.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mxaxzock.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udnzjgyu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nhkezupd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hmqrbfyf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mnxyarkt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3pgblvtzz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zlrfqvol.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3tpogypuy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vxdhtggo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mlnitmri.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jupvacpb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cnpaazxq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yhevrxoz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3udjpydwj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ecqjtecy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3fsehhuye.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3uirzsrhb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vwtzdxfn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qsbmwiec.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xojiojea.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ltdtwoce.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vxgtbvmi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gqjiwbxn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jeueocbg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gxlgaolf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3azostyqj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3bmafbqtt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tljklwcl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lhfyjdhj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3kcjkrmaf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cuumliur.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wdwaqtvm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3omsagjdh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xdnbsvuc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3oynwvuum.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eetktgmf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dynnlimj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ajfllwnv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3grgvtoit.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gdtoqwwo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lpqiareh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3egafhfey.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ombgkcdx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rqltdmoa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nirpljoc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3llixwszt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xtlqqcfj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3giyxtyor.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3izpvwycq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bprjzlfl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhlhika.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pggluneo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oswrxnxq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zkhbefsm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sopnznuh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wpbfcegf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mpnfowzg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3omxqdatp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aukfgqes.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xlspvfeq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3abxktohz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3swgldzrw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ygfksbox.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rvkmumko.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qkdvhncj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sqimcwaj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wesrthwg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3srndsgdf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iwuhixfs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3qzayyfrw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cfxjidby.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3msfcpjjm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ozrmkkgg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zfhhgntw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsefjkqd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vszokyuk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mzgioupr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3grmqgozx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fqfgofld.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dovyibrj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rcqutppa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3oymckcql.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fzquznwf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3udngospg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dwibrlhv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uujzgybm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vgpylmha.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blqmbjcb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezukknnl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3angxyhxn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zuycsogp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xszpdjvn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mfubzrtc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pkrfzeau.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ndtzaowx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fiwujfxd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jzikllau.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mrfpdbgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hangqeun.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vjiuqmxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccplqigh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lgyibpzd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rdwrhfzl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3uqlddmjw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3roaoazfv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wpimdguu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rinobyff.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mhudrwqm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cyjfrdgf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3skrkdgvr.html


<!-- 参考信息 -->