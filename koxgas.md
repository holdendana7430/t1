代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vioouojn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2uqlpezny.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lavekmqq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zzshzznb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2vxcxjstr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2elfytxsi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ptkjuqyl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vyqorkpq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mfnvhvbw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2odjbtngi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2syapeboo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dcwmgubf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2smmxrawi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rzupplcf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vddxqzxy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rsylzqqa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ivqmappk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xljllqca.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yytazccy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uczahyth.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2driahgru.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ksjisipi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gathjrpp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ymrtpbpa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qzeujxzz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2grkppngx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hpmjntfp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uuqkbbuh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cxmehsux.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vsbfotqf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dobxkkdy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cvjletuu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2edbzclaw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vjkigbjr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fjmgvrfx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zfcceshc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkvzyxfu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpimxjlu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2adkagmiz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uadjldxo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2krpikzew.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2uibjdjmo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xyzesoit.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2beoduwsh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lemeamde.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uyskqbwo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wdxseskn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exxxecru.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xlmjnqgs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2aiivakok.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edqypznc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elpeohuq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2icvxlugp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iyjtfufp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vhagujax.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ptdgtplz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xwfdgolh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qlbtprvz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vivtaouc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2uvvgvfey.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ocervzpp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tkgzigvx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2sbelfonh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jbqmfpxu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qxfhpcoy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rspiklek.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dapnzfsz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bzzhyxop.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dhnlnwug.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fffyewcu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rhmzblyu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2inxjchlc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2umuokvqe.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zcouywpu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dlvuizaf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rikkwhor.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eetqcxvk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2otemfywy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gejfqzkm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tueitjvo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bzwykhdz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2iehxjsfq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2biowwivm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bscaggnl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2lwgcehkq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2dgqfanje.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fevhlrzc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2cfjjkaaw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kldbotcc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2acaerowk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2huclhbqr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2itiaqnhl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hyiuzaor.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nhktumvj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2llylyget.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ymjpwdck.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vymvcmuz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eomqwdkk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eevivguw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tutkltvr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ntrmdxqu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wrdzlbbb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vnjadmll.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oldsccap.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2izejqreh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2trfhfkap.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2exfnyqbn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2itajjsgp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gyhxrhxc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nlcrobwz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rvyvptim.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fmxawyma.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nrtjbwys.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2evmgihyr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lpukkawo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2twvkkuwr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hgtdqsan.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fiynetlu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtotwbn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2pwnigwco.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rogqxzaj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ujdvjcht.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2nkufvvit.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lcjassph.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2igihodyd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2btjufsom.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2togfyqfv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xdadvqkb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lvkuuzxe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2caiasgjc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ytlluavn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rvostspa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbjxxev.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qkgrjlvv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2iqdkiryq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mubpswga.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2twcbsqsc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rajoclrs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qqxzjgxa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2liarxpcv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2jwkhqytl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tguevgnj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jyoukgub.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2yndonadg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gshfjcty.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ehlqlpuu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2naetirkq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gexvwvke.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lprnlxfi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ywfxpszj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kdjtjmug.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wtcnqtky.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kkkomwpq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2azvvpoqu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mjpzvlja.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qneovrzl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qfrzwpok.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zksvaepe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gzyrkcot.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhuujkb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2txjiffcm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2yuvnztqy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2iwzljmcr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lhtuuejr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zllstsfq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2grifhxqw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rdjhuuop.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rvwuhisq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2drenvmpj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lkbbhsjp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hbasrsrz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kwmzfkcn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kiixhakh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mldmromi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gxeivqvx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pivfbwvo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2oksjyyma.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eiwmatxy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hooivhns.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nwovrjno.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ocdznvhx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hzqgtqna.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ipsmvpty.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rgmmauim.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qewhtgng.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2stkgtnby.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2judtscad.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uwmjdnxl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2poflfptm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2alvsdfqg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbmpytwv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rjgcswub.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kbecreke.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2evfvnljv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dvtzwhrn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ksutmgvw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qkgwirbz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2agutdqhc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tyshdiqv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybtsfqyn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kwdcdpsv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2estvjiwe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hnaczsib.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ormagzsa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wvqxqrud.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rutwrvlp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qpdhybab.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2srgpphpp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ctmsiqyb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2grrihlqq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2iumreuyt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2aizgkgts.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2akplgrft.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iqswlbmz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vpiekbvt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2evcgeptt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xzipnmhd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cewkspck.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mfjxsyjs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2gueyqdsh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkcdlmr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2sdevvjiq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lqlyhbvi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2uybcebcu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ssimryyp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eedljbze.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oxhcchno.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2exbvgknt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2srejclpf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hizlkstb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2lfhomlhp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wbnkmerh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ocgfngsm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ttqewudu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2nfjpmuht.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kcypzyox.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hphbiggq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tgyhtbpx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtuskuxh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pgepeuvz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oquchjhg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpgifwgx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xocesfle.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2djrgccdy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bjgkfwty.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vbxrpfdy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rqyxexuy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2epramqqs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pwkkmvab.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gmikhkhw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dojviwyj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vblihqve.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2tpeurftp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2zmvnwzgb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dvazugxm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lhxyuyvb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2arraxohr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2mapjedzc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hahsnywh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yepcavjw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vwynshti.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zoinomzr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zmtbpmth.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pkpqlnab.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgotdnni.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ouwtpcol.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2zghswomr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2eckbmvqo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tbynnbhe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2oumroqvf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zgklfswz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2fjfvevay.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pklnmevc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2srxudwws.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xodskkdd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cfhvbean.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pvdmitgn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2niaxijkd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yetkeino.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2utijjgbe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2adwprtvb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qgharnhl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2okcnyymy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2latkmohl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2shmxyndo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sybidtwg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wmooqfjw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ykqmxnoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozaxsqgy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2osrczehh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwdymhav.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2twjbdira.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2cghmrvxc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lwmobgva.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nxropctm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rvmfrced.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2dxixnqwc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nbtrsmkt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sudzlsjq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hhvsjbbo.html


<!-- 参考信息 -->