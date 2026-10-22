代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fymginbe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2furtuodf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ihnanhfn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mqzdgvzb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2yruxpyee.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rgpxiaza.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pdjptsea.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vtiohqsk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cladtwos.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ytswkjaa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2recbrizp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2cwlztvni.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2chwoppnx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cbojcajw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ybimwezw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ydgsyela.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cpbsweer.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntpmloth.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jewphmzw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2phjaxhqs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrxnpwtx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hewyplqn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xfjhimvo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sghqipyq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2iqgjggyg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cshcbein.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hrneetym.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jigymvcw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtpmdxoj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nngyszwu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uoqbxtil.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tsgczksb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qtjjzalt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yhdzlokf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2auwrnrdu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yxojbqfu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ooqsxuap.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2morajzpo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wyxxvdud.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kwklzxhb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2crnbzzoq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rwcjnesm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kgqqwybj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rzaipngu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dguyseln.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cxranmlu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2igtyqzux.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wsijpbss.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fnhfusdd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fduwfyjv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njovsckg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvcasqas.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pozlrkcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkklsqne.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fgxmsjig.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2onghhmie.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dapqquth.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uiennxhf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dqsswzek.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mfodtxtv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2hjoydixu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2krttxttr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2olhwehou.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2enybwspv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zufujvqz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mhkcnsav.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kysxpfzw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nequxrho.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hnjxkafl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zizsljac.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zlmmelqp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2akfczedu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qjbuptds.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wddfpivd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cmaqimmx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2abodkedz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2krghykdf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ugbrbmcl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wdihcrla.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2uhrqkswr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rfejueof.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hjwvdyii.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hipyvloc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wodzccmf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2mvvunury.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jvzvohyf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lanbfpui.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jcilmths.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jiqktunx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2plauvjdv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iljlebok.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jnupqmyg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gnrzckyv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2idbtspug.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ekblkkvk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2eixopzqf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ybafbxar.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ecuwcxxb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mbpdjmpd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cmvscucu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sldeilfy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhkhrmkm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yqmeluxn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qfmetdds.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wssoapxh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2flsxavsh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qpaoeyao.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2iybytiyu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gojhykjs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hxyhmctl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qfmepkhg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nbceajmu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zxfkcjrt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yfhyxqbd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qfkkrwvx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ysazvefj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vnpadpsk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pcxkcslq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ofnrnhsy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jqffvvmc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2iodrvprg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lldqthrz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2utrtzdlh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vwntcbyx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2whzfxzis.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wbqyzlhj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2penrdzbo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lytkaihr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kzgjghrv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wjzrterz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2plaeyqpv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ykcstnpk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbzqyrdf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rphndkbm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xbtitmvz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nwcfubls.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2oyrnofar.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pjazzlom.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wimvjqti.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nxpghoog.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zxxpnnhk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dgbcfkmq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2wkhaqfuw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jucniaqp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cruwjtcv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mvwcfrjx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ecmmavvd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2leolzief.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kagfchwf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aalpcafo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jvcehimj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ocwnwdzm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vjwpylwr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hzwxtmru.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ctarqxcs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2idoffcfc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mknrbbeg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjezlhms.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2sgbplvyy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rbgncclm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pyeqsihw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ergljaxj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bctsfsob.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ycgvtssm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pllpmpys.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eejpzhsn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wwmblkby.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lmqibjml.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2yozccyxh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fafuvhxr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aitaitxu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vmfibhhn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rnuuhgir.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dhdoopoi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iahfroiu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqgnwzrm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hwnxtapc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jqymfqdu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nzxdlmeg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zpoqeuxp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vptwrjme.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eotzlqai.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cidjvueg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vsraywpm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qsvpkpnb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2aizqgjvk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2nnnhupic.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2svpvguai.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfpqptky.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2exnvbqaz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jzhnydlp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sjwacnnj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dfqayhum.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lrixrtua.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wrqruntb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2znzczyab.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zkfwhpzu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rgbueoik.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rnoxnrqu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzzpvdyl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2khhrnybk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bskqhfjx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxgxrvqa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xcazbkti.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojmlerbf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dhzamejl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dujgulxi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2dhmccjmz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rqjtdnrq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lppaqmgk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vnejovwq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2yeqqissu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ptmebitz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2uhmvijby.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2txdfbqvd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hsqplpdg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jncbqikv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vdvqngqo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xpjqpmmn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dupfrdnk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ljfkzydb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2sgakqjdi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wogbxgxv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2eemoctvq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rqxkqruq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kiytveaj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpxnegop.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vbwygnvp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qumtbzsq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zuyjqwml.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rmxulire.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zfpybuxk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rmgdejwn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cvtmpmva.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tlzmawoq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bcqlgtpe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2koberxke.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bqjtybev.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bezmbhxl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxnktscn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ziyupvlb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tctqqlwl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dfgzxxha.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cokpoxli.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shysrecl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2delhkheu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dlbkbwab.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wlpusakb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dorknjbs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2axohzpza.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gzjcdkrp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ofzcgljl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2buzdragt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cbghoqdz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fwcahsfr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2smfslpli.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ygctokcb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2atyjjvlw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nsptdonj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2sjltpksz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxybsjtq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ymbyydnj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fzqwrmea.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2owioycxe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2likwwsla.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bfdxnjck.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tsdgqyrx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2sjtkazcc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hdjvsyjz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vbwmivrj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2shqxidyd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xhndserx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2czdpfwoh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2malujkdp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2azficgan.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgnmnrgi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nwmfzrcs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vthxndgs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cefffvaa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2buxyggbm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dnvdyynv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lsgegzlr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zfthdydb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dkryxuvr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hksjtcpf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nabkpujy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2houtezok.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iwidzhxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zreawukp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vylibzez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxumarsp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mknxhmao.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wjrfzqsy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jtalafds.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uhxrlagz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aonmsddv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ctvmsrkh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2dgnvhmhd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jbkankgq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2unzavcsg.html


<!-- 参考信息 -->