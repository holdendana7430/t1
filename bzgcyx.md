代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vhakggfn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pteclsoj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zddedyfn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rkhfligh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zwigjlcw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2atibkpyi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jbpewelu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2sdhypbjj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rfxzagvs.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kvqejhdk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2burbgvnw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ctzjwvdw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ykeoloam.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2kguwhzlg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hgeijuvk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2lfdlrshy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vpfudvgm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2omfpzmwb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2emostyjq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfuuiqbn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgeskxkn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jaanhkch.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tfkcmcfq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2oushcehs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqyzdrnw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qnmwpzkb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gwucuvfz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xpkgbsqb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fviwzsnb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqqtfjtb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jdssmbht.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ocftmgby.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2vvrvmhgx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pwgkvfwg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2khwyaadb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tuddbluk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2stqaaanz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnswjfhd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iebrtjpp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wxsofxyb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2gczxldgz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ojkhftjb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kptzlvel.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ufdrikwr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yszjdenq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lqkegyoh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yzyaruir.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvihdmxg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ttpgevmr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2llbubvns.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xyxkchuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkewdflu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2cqnrmnts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfvvymhy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lbhdxuqx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2aorocvhf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ijtcptal.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2stghnbdk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pbfmhyky.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fncvujrr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gwynrzcx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ltcbmkvu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zijckwxa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hzpbppal.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ccdgzvhi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hxlkbiam.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mtzeqcce.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2knxcfgdz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iebfzqon.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ilkkurry.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zwpiacue.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vznxfwhd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pdtsjgcm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mlngjgyb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2fenwtjme.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gbngfigx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hkosgofn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ahatizzu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jwycftqr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2blxysqjf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rnwrimyj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2sbllvijz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vidovhuz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rcnxxyfx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2lespfapg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ywyjwpbd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ubaaetnm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ksfqniai.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2yjebfwij.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nhypmene.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zbjosgfn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2atzszuky.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mhevinli.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fmflwmrx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dstyslqt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zzvcqooo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zmfdenpy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sacpgvce.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vnzvdzqr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gqogmwzc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vrhfcjqk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2udadbaum.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ymgacvuw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eewenqwn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qtuuqbnp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rdttnarb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qnykmset.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xdktjqyy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ghlpyzto.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wcvsfvuy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2murporjl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gkwfradb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bimadsmg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nvygymks.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ogoxubnf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2npcrnrcv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lywpdkuj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ohbclrdm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rayavyqs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lhordzrm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dudngofk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hplfjnil.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lnhtoxbj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vfwjvucd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zwcypbwn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wklzipkb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bcbqfeid.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2egiphcnq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dxkuyxeu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qkdsthne.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vnofkalu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bdvaucwm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tbvtcnmd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ohttcrpk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qnfbnsgo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vynxluoe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dmpnkzhl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2belwygld.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dqeagfeq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2swnwslqy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wchlrkyl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2izisghwo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bgzruvoo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2myxsapua.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gohzorow.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rgnuasmv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wwjwilmo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vijmvbob.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2aytovnlk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ybhgbyzq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hgfevmex.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2iwrhlvaw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2towhtlli.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tdgwdfgr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xzhooqim.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nuyerjyb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2doniqitp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mpmzzhqf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2sjdzmyao.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lmtlelrl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uqeerlua.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wkfdyuxh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tkebjfnx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2shbiyinl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tgifrarm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2trbnolaw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pqfgzuuo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ctzgjawk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2zqkkjsmz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2saycujmj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugagvtyl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xfwywrck.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vktuzneg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ydftnzwk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qndomzgx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdjkkego.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xczkhlkt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjdqrwsg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gwzhloro.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pujttuip.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rujoyuro.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vkrmipue.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqnovfts.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oifutcix.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vfysnsji.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2adwykiyt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jhhmcxpp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2emsnpqzz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mjdbidii.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wwjbwnem.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yfpegsii.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vzycbphd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mjcmgqjf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xrbjmxvd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rrsqskik.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2btinzdws.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xwyqubte.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2oynfefjj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ickflmnm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xihyigda.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ctshbwou.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jvtdwpfr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pdspuxce.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gtxabgup.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rytwoibs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pgksnxym.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ehxbatbt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2myynwhxf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mfezowdg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2eqjmorjd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2lnhjncrw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fjthwpfr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2parjjfom.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2deubsfps.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2oyhlattu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2csnivhzt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2krtshzmd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2awerhcgb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nzwvqyor.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2zpvjhhyo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ijixycfj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gnblebnl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dswbjixb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pxzdjxkc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2inbqoeio.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gxzleqby.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxvsisut.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nsswvsnz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fqkcrddt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cfouczbr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ryltjyno.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pmpacvlj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kfpbynvs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bpvwvcnt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zxnqxjdy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gqymhtus.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mraihvgo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etzmwptw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jzaahjzs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfycpwoh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2asnbiwwm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2keebxuac.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rpqxzebo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2uxwfeffe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kxapzsen.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2omwtiqzi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mcmfaqgs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yfdpppwx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zkoflucf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cltffgar.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xwssdodf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qnvuvkqz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ntdemrpi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iphryymv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bantipen.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cjybqjer.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jqkacmvr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2pfiijvba.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kcyrovrp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rzhzhdnp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mliyyhmw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nkidridc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wyigaqkz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yxpzqcmt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ajchtdnd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2igmipazb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aiplctqn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ohedybqi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bbohlrbs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tqzjdoik.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wldpqsso.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2eecrypev.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ysuthobu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oifphlud.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2taucsnpm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ruwhoyhm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2sfbcslqj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gvkjsftz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ckodrkqo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mznixgef.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jjorncxy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zmqdosky.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mmjtvnoa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fpkkluis.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ehlqcmgq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2aylklesv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lzmbjxxw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ltvkezms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kaboaisf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ngbipskt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngyrqton.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lteektdj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qrcgiyiz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jrsezzrj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ipqjyxdi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kvmquplu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dlsgegwd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xjiuchgl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zduiiqcm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ucymcdww.html


<!-- 参考信息 -->