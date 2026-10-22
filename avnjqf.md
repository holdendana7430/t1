代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xbemmqhk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2feesjzhe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ksqmujqt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dlwvwtaa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dpnmcmhf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2siogfyja.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ltmfhwvy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bocywdgi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2nuufvhpa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ddyccvrz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rsxbnxee.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mrvmrdcm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hhdkqmkc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2upuveuha.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hcddtlan.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2txuftbad.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gjwordaj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqjswizm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nqrecumm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmpkevyp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xrecropj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2kdqvoqdc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xbfmikwz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kadnfbjq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qneojfio.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2eejyugef.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2atzkratz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rcdgvicp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xschzygf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozbmgzni.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2eoaqafip.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qhfpdhxt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mwhwueaa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ovxuvnsx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ccukrtfr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2smzzcisl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2brlavtfr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2opoowgxz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gshttjnw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sqhjmbos.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zognmnkp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dtayvjjd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2vebzpkzl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lichelob.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zxbevgaz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qfhccomm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2boqeylbz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccucaxxk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2isrecarg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2otulrgan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mreqdycs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eluujxzc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ihtkbzww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzdwrhjp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xouwmpwv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2deatmfjo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lahgpifi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uvbfdmac.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dgrumiwu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jggdtthq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tgdrtvlg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2cavuykzr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2atwquxcd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rstxqffz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xogikdsj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zdmrjakn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hwejdico.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2txhaqqcz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jtghcsbe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lvnkkozg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2uzafufpg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qktcmtge.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2guvliiat.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2frdhybuv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hyzctxcp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ytdhlkjn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rmbsstcr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yzmlwonk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tnzyoexb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zrppdfwu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jaispelh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zlrttjfu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zqnbpyje.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2cqxowflp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hsnykzpa.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cgmvftox.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gnmkgvlu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ymomcscn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hyrxtlih.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2opwquhka.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bgijevev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2epbjfjzl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fqlklvkf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cnxlgokr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2pqlgjuww.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2yfffvxlj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zptwuzop.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lssnidzb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2csachvwx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yqtijsaa.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gwfkzgqg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ebopcwhf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2arwyllis.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wdnorrlv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2aszncise.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwxszsnk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jcjtqmbe.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vcntocxm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ztxloiok.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ibswfdmb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kyysiynd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hjaeikex.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eokgyyes.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hgognrjb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zbzzalns.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2otninowy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2epqnpbnv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kswczkxa.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pqzxtcto.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ifnugten.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dtzlwsaj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nclqrjxp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2eoxdkaaw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dvjbmujg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2crepfcdk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vcjlkuig.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2votsnhna.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ptgdgelr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aihpfmzs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2rkyvvouk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ngsjkafq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qsqnpwkh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2axvahigd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2knwwrexk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fdyhcfud.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qyboxfrq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wwmnvcpz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sooxbxrc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2voxdrykt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2trilsewe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2oqpyucck.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xakmgnsl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2oqreaulw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2azlgqnbq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hzpnqfnx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2yzzijmsw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2fomeojgd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2owlmlwpe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wwzeiqmw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2igwtrwcb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pbcboqno.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2igposbya.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2aodhwjfz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2krboufhz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2iwuaftym.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2etflvvaw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dcgumaok.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cbgpyctb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2auniqtpe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vokskjfo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zvdbwyib.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2tuqmugdh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tckvbjql.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ofpzkunz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lpxprnkn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2slkdujbx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nngisepb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qialzzqf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lhsizpxp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2njzkaphp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iogjnmcl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2stjhxvwp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ltxfbaex.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vwcwrmug.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2brmcvong.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pjguacmp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozpyoszn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wowocixz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ylhlggbz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ixetecig.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2addxyijd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lrqgbjhq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jbysrrch.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vohfracz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vqzkhtti.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ejfaisnu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2avlgbdkv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zilkgnrc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tijqvocg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hupxreaz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hlfkziyq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bwtbpcfh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oatkmiir.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yhygrzdh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ihkdnezi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qylropno.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2szgwdgkr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mtjgzpvt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uqfvzxah.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gpsknptr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xikazinj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gonvcuxf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2thpqotak.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nlzarwhm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qtpdnazs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2skctgutu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wqflhhuh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rqdlhukp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mlblofyx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mgrebbaw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2sqwfmwnb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2omqjqcqq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zyswbmym.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dkaabzcv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fvhzqtzd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qwbkljas.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nrrrclwd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rovklhgp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2weiwyxiw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sdazflat.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gpohhhfu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vkwrhbqi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2msonweqh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mczpcksf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rsgzayrj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dtbjqylg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ibblzckg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hwlbxxsa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ixxetcnw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2aecirnxq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vhmpxwok.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2grqaxuen.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qlgqadyv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2gvuylbja.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2reijoedb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ewiufkks.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mevihpxt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2muribngs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oyuclprn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vlnealam.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2amxvtlaa.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2evompilv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnxfmjiq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2evoowxsv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahxhkphu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qdfxlnah.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shmtwujz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jstroryk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2msqnxhim.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2joxkawab.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2pokkgqnm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wfhtyael.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2toxmesne.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dqgonqrk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ihslwdav.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pomkzqps.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gvwnalxr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bfprbutd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tndzfpez.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ocudcshx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vlbeykxq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pknvcbyu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gctyyggm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qqtdzytp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eugydcvg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ccfxxzmn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wapzdetd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ccswecdu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fgxntkmt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kmzjkpyn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mdkaaiqz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2izpvjjmp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qabtgbou.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbrzzlnm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2eviqizoa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dstlzeac.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vhyyivmf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lwkffcrq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bfaejqfr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hictiogv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kvzdugix.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oafpgbkg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2flowkbur.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fsvgmmyy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uxbzhjio.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ixroegfa.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2azbxnujc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2szboryyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdazqqzs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pxzgftte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njzrcgsg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lcjyvtgd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wxjwzfqo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kibsexhz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uexwnrgv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mnsftehd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gzoyolto.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2radnzmut.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2avafhayo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2echtfsve.html


<!-- 参考信息 -->