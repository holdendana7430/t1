代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2odkranle.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2wzrbkcgy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hwryywvj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2aceqqrfd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qmqebbrw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gghntlrb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gfvocbgf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xcbkpaam.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2tfsfowlo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dvybzkae.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uwtepkvu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2nazqvyau.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2smcooptt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2usfanfcl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wrqhujoj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pjvoacsk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ffkxowwk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pggqpjuu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jpomxhid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdsymsff.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lumssppk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dicpnauv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2hwukyikj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2coltlccy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zpdbjlgn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wxobemcf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qjrbgggv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eivatygg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vkuroltc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuiwssfn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ujgxpohn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pucavlfy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ejtuuter.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfinrmnn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mpadfuig.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rwkbcynx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uhkgoztk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qowqpitw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rgbdpygh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oqmyszas.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mbermwyt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cdmaxgcb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uzcohxoy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ihfwrnfd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mqpjohcy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rkfgbznd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2iurwkyfo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2nazeerqw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kxxlxpsw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hlqvtdff.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qdndhewn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwxhdmmu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2klrdrsts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjyfqork.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gezsflih.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nhctatro.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mulwctfg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hoxzdcno.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pvwworrr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yneoshst.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xkkhkxgk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ugugocnb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2amtnletm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mgrgisdm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xshdmjyb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ttgwvyrt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wpmiagng.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ekwdgxrj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kqzzzwct.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhhudig.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gurwrrtj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nhbvmlfq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oiwkzigl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vjrbcxke.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2njjoujxv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ppjxjycj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rjmniosf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rraizhne.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ommlyqmo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ctyuojnd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jmgvdrqe.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2onuexosy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2swanwxae.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fekdxowc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yrciftxt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fzmhnqlo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jgieoteu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lzpbqdsl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yuajhulk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2togbreqd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2augylzzu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gzkovjnu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2smaqmlxg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xjhcxqbo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hworekfw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jamytvdg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qlllwrtz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lmwzdbbh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mdwpnxvr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2udfglfdf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2luukkcvj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qrvcdatr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fwlpyxbj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gfgzrffr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2odmcggho.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzvgwhgo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2dtjmfygb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dixqyxqs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2whchosxj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sojjilrc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vwwthxlh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2acvarrkz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vaigvtbc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2duzauqao.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tcfhzyyq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gzwonvjv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bgnnplkl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ggezqdyr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2cxecsuls.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2elnzrdsq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zbkurvnr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2leccrdgu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bezgwpfo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ysablmnd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jimzaerl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2necipqyn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2aggjftmy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wkrlxeoo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qmgovlbu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ignfpwdt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lyweieio.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2amdihghl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wkxiqlvz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2peowwgyk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2qtlmlptg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hymcgbxs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tzwavnyo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uozlqolf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kamgotok.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pycwtdki.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2knvdhpek.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ywfbwapn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ykqlpebk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gugsbkfc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2apkocmpl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2svezobmg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bulylvac.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2imlgdllr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qxmaipag.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hijmntnp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rencycfm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jrsqcckw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gmqpsxps.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2llxkedgg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2itrttrcc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ypaubpgg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iswysjew.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qlaufnfw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lkzkurfb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2abfbhcjd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjmjcfgy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2obfkwwet.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gemkkkzp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jscvvigt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fgowwxuy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmcodnhc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cqkkjqfw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dgqebhgt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xzmoowod.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2avtlevcd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pepxkumt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rmgkqmhi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2odkyttio.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zoebsxyb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2unkilohj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dvbnfwcy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvefffes.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fleymkri.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjinewk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vlmcbmln.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ydwdictz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jqmfwjhq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mgicxxwq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ktemebeu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ptiqoxiy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hmfumwud.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tmsqnthg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jvlhcqwl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cwgerkfe.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ewzxnjlc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jfghefhq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vhintrym.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xpebrcal.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ceecutib.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pgzlbmbr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2aazgflka.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uljtjjxe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2knfdkmtf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zzxgtoxh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bwqalqkb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2savprrvf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2splrxfqj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nebwqpbz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2aiorgeuc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxbkfhwb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2klxrqezy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dyylvxoz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zbxqzwyt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ptvpfoje.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wkggkfej.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kyxoyvvz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2puznpkxq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2danytmti.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gceintoo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2beuaoyyk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2whelvlot.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zzpegaez.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bwjcpxwn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tstdxhrw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zqjiaoyf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gqllihib.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xdjeshdc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bwioswmo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ggheszkn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ogufrmfw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2uasqekme.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2toyekeef.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nittswae.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vtziblfd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2orlldbff.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dbjrigzs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ndfumzdj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sdtpxnhp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zglknxlx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zqagmlrh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lomcksym.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fqaauxfr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zrmcdiul.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ibojfkzq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ilvixawm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekzbyhtl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ysfqkxed.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2psjmcbjy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tcacmlnd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qickqptr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2olzqzgqp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xdxyospg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wwhoszrj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2evavabtl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2eccgvvhr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zbdtduoi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jbcsptat.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ovucxxap.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2opgkrdkk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ptfzjztb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tywygapp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2girsktph.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2mprnybbf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rjdbxkab.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2munumedg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddtnxnwl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lysjviwg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2carequqz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2elifjios.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lhezbupj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kdolyhse.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yudujjjv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2lgksomkk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ktyrcocm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kaypkvtz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zkkyieex.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ibjrqexu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kebdxdrd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhraltsg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fplkevgb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2juyvhawm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pcetmvgl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kyrdbpfq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2scjucqgy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ltkovauz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ulikjhvm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2minjzyjh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2moqlnqoz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iywikstn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nysdudee.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uktbwvlt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ljbdrkkp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gblpnkyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgsflecc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2stzqegwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmixjvqp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jdzcjkxy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sjjwwfoa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hwoqpsqy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2owuasqov.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2capotylg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xebukkbj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ngnxqyue.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nkqvtvcw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ippvwydi.html


<!-- 参考信息 -->