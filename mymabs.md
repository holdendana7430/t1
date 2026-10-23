代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3uyxyojjv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nvieskkp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mwxvxqds.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yhvzguki.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3aplfdovi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ysupffum.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ukxocgug.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3opjtdbns.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3elpfdzdc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nugqcrgq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jpmguiyv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3bdkiybba.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3oaqzpcdi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3cxfgiwdf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnjutowt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tslaizoy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cbpkvfrw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mbxwtnjy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rzefspdt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwfprcdb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uiywkybb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hxjoxlcz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3htexphvy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3pvrdgfjz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qzuotrvu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jkwbixea.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vugknxho.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hakwshgi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nowlryvz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nkpdjioz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bbkpsarc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vuoghgis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zpegllrx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xozsfdxh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3sijfyint.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ufptksei.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jtwllvvv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wpreqhbi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uxcwrlpg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dzznnbjf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xvcmngzn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ghyafahb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3oyvdfjlo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jnldnort.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qxiiyttj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ajlulpul.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3inosfuxv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xphodljx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ksnfieae.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3zebdfghh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfuwhqey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akiujkkt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mpntgaie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siauojim.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nhvoegzz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zaunyqfo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jpcopkdy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dvbuopkd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bikjsvpi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ochvhnio.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3uoebixbt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lugpbtbg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qjsuxdmq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3umftdaju.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uaequcyc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cgivcftx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gxjfibwq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3csvtybkp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rabdtlhn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ziclqbpc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3iinueqsr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pxgnzoaa.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jzfthsal.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3flomhjoa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nxqvnvio.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3upblboiv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sbcourfr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3udfswlqe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oiwwgngi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3uduzcjqc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3airhurgh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jhwxiyox.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3azummyws.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3whxwmulx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lzhdgthg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iqpejxde.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ovzvezdu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mwktfxaf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dccqbcyl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3odahmgcs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xltapyfa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3trdpmhak.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wpiumjhb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gfiwmvuk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vxirosvy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ujljktib.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uvjmrrvi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rvtwvfaj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jysgyqow.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vzraqssh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lyjfdsqg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tbfnobrt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ujdmdkko.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qbhwctas.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qkuqwvkt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3axzmoqpy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dzegmglc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ikjzskvt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qatgjnrz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yczgsubp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3opfjjsde.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3drklhnbx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tcydcwis.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rmorwaas.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ebrzlgwa.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3fdkvdwow.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vwoyafue.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3egducmmr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wujniyem.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kpwwdrfr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3eegczcfj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3knecamtz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3bntsrotq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxcztny.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jlakmpip.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxsvuefv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3khnujftg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vbtehiwi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3puhxawxm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3lisivqfz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rxmhyaal.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hrwmhpoa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3upzjfnfr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qgohxxmj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3weizvrxs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tdouojgt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sdihbxty.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qmwzkgry.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qjbniqys.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3alaubful.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3utzrxonn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gpnixali.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bnncewpp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bhyjrlwy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wayuhrfe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rrmmbjvf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwxyomre.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3olciluxx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3reoqkltf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3uewlmlwp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpubjlbu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zrxfynim.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jxfgaxns.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qwnpcwdb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wdlxztsw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uypnthth.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rmfxafse.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3znuxfybr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zllbtkvo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmzronkl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fygzrfwr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rvpzzsuf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ubudlolg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cluzfvst.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3auabwrct.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jhznckhw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fbhpwdsi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3fzximszj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wiptiwnm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cwqqqrky.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xebmdiqg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hympgeic.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vibtfows.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3smworbsd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3advjzmmg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3btnkeokh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vxjicjey.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3csprxxfw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3emqithag.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bjsmvsva.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hjsamzpj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xneynyhi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ptblfsje.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lsdgruaa.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gayqqnug.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pqzoaxil.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qsiwdckp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3agphzjwq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3stceieau.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wqzqgzcq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dgzpodud.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pisyxjnz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cgymtapx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tycchzxb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3twtrezsx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hhpsluaz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3amtuwtrd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3njdhhrsy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ellptmrv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ezhqayrm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jyrynryr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jniopkkq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pplnaocg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cqxsgbee.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vkfzqgaw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3coiaobqv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ebkeiamu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3btbinmit.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wofahoox.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3fuhlltwx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3epvtniap.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3foobcfsp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fshrbwvi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3znlkkivx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3izbwjiyn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dacakixw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3cfisqurl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzqqxjy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ximzfgrr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kyfesffz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xvqbozom.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3abcpxcat.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3twqpzjgv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hjlmryel.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3yhhlnpvn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ondtshwk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fffjfxfy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3tgjdtygm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gyjuaaji.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3imqskqbg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3junrhwcj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fumfofnd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3brwsjfyf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3cfkuzavg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3memcpsqf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pyjsombu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vmqnaoid.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbliilmt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dhuoizzo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dbtydbtz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zdaptwar.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oolwaaxt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lrwunfpz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3arirrccx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3myffmyzs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3bjyxmaef.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gzokbkvu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3klswbkfw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zztunnpr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pvfckzju.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3olozvrxv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tmthqrdr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3evftzvbf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jzljjnze.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hlnarbwe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dwyejdvv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ujknjocu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xfpvusfn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3soykwcpy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ehfznqnr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3oelyxngr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wpkqqovk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gbwlscfx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3offgybcw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hucsmhgu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lkwkfnwm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wvuvwtiw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ogokmihc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ykdbuzfh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ylfkyvln.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dmdjysxp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mksnmozs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cgsjgbum.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxowfdzp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mjbijkwp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ommofmyp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3uevjjizo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zsbvhway.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxxisaju.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3shksapsl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rardhbbw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xqcdyyap.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3koiyrydf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gdfldhix.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vrpagedv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dcbwjsgr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3neglewmq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zhkgxrtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpvgpqzz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3wyufkfbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wriryzhm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3szrklafx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rcaolpqo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jstvfiko.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dwtpodsw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jcajgnil.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wmmywvol.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jwqhijsm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3neqhwivy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjygxhk.html


<!-- 参考信息 -->