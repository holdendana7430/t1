代发 wailian999

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rlsixbfy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3yaqdespl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3recqbtzf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wvxulopu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zdobmrio.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3iaaxiwtv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3moylocri.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yshpycym.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wmfnrjle.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qdsnvvwb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zwbntgnh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lhozoobo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uetuklwv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xmvewrms.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3twreqtfs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fzmerwdx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qeamdmsv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3sowrltay.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nezjvaoq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3flktoghw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ievyizif.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dirvzfgz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tbnqkdvq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpnnpsqz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qdbfmsep.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3uvqejuba.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tnnxgtru.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dovrdily.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nwleutdw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wnsrvccl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ficudwme.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kfpuhffh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3btvazqzj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cywppmyh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mrdxnxgz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kffbtjos.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3jinnotxx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cgetglzq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nbfmuoig.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iobhurtk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fodlraty.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwcagbkt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lhsizrof.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xxliiuic.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ewyxucyv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jddqausz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3knxjksih.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ycltgchc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bvorcrht.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jrgkchyv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kesdxkbo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3akimkmhc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xhqekpfc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijikbynx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pebbwxmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekgpejgc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tzcgbwgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfoowdzd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3inrhawhn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3eytstjbn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cmkdzfjf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3spipwoco.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jwualqxv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fdmcbbdl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nnwvyoxd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hdfeawsw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3reufcogk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3woepxwej.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3swtmbqmu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ppnnfycu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dkhmkzpk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qbhgzqnq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kolyevmz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wpnwhfpf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lbltokwc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3luzirplo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pkcnkamg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uevemrgx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kihnpkhp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mbmekvsh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ufzuejhz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jkvbhoif.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwhxlii.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvgrgfh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xrhahcht.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tcnnphrs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rahrxzwx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3hlftkfmy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xjczqwkm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3plnpgbvd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sdzaihgd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xltieuci.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wtvqdbvr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wjaewpyt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rgpkcsia.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ogwcrgkh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ublreugw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gshrjtwj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jhfjcfed.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ljasbysj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3skjjrqbd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kxmludfb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iqahbmjs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xzgyuzxe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ssuotuwr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3knzsfriu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uzmcphhi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rzrbuspa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kbwpwezu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylxmotnd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nigrsald.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mbqwhpjw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cvvewttl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xceuqmod.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dnjvbeqy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fczaybxw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ndmkkxrs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xxxhtiue.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zraflknr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ulxxvyoz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vqvwvwux.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3amcxwyts.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fpverawx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kgvfzevx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ckreercl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3elzwuhzp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3baijuzam.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3olnoreib.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jwsbjzuz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lwhtqnuf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ukgmeaxs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eyyyholl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3uykssafw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3taksspox.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kccqogue.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3umpfskaw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jthcmdxi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pbfvmfta.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pmxjrqmz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tzgjeuxk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xpvvhakw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bluksdlv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yrpdddmj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lixljdlk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zitocgba.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3jfqbwakx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cbgqqmsz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3cgvaswsj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3talvhong.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dlngisjc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yvdlnylo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yiegvrvx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bhcuoyjv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ukwhnges.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jcqibekw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vdflvgrv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hmautbch.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lyhiccbw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tqwdqksh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wbksbrqr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wgupumfe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nbhtpnpc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jxpdsmqn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuwhalja.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3hbonndjc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ttbbvmcv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3aaqfwjbu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wapblaee.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3syfxlagr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vdixycqr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pqzvytdz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sgnsdodd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gbuozclp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qzqcymly.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tldgpbsu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dsvavvty.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wpszagsk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mavolkdm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zllenarv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3renkzkox.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gwddtswu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kervdfow.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3itqyythu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ssrpahzu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pvwqcypz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qdfxbtcg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bzywjceb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lfawugmp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3adijkkus.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qxyndldy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hkpqsoli.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3crxwcwki.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fceyqwqd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yynmsrqc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3odolpqfi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3omztyepv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3greugsqu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rjptukze.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3eveezoko.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3akvekrnv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pebzrpzq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3upvfdbcs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mplknkvp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bcvgvjcx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jusizujq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xpwdvokb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dnjedbaq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gfztmzuv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vnfuknqr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vpncjbow.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vrdxzllx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ykzwtoag.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3shiiqftn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3asoowmzf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3axpqhbyz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kivvuzzw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jqpydrpm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dewxmppz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3eorkwxqf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ujvlvaei.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qqivgifa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lfyrhrmv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jqbcdgsx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3eeokxpnk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxqlein.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tzdaqudm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fogudolm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fwxvmeim.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3nbsdyotc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qsgiunnf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dosizevk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ufsjkaem.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bmhyexbr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qblggrqr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3namnndod.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3byauwwqt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3snuqbdxi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ltbqqchy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3temldkpi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hlhgmvdj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xgsbxhad.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgzyibrk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gydgusfb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gyzfkxzd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fnaaxgms.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3epenecme.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kzjnqtgs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jslpclzr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rogdyfji.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vcjqntoh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vvfoecnt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vsdlqsiv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zafvhpjv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3faseiruq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mugvuyaa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jwndroow.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jeyebqft.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kcaawdhp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jddkrnrs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yhjdakti.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3npcqknkk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sbbwziwc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nhiujpqk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pxynbgdy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3arncungy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3spbhwcyu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vxhmdmjo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3souwenfl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ghbgaghk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zukovsun.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xaexgeju.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tldnoyqq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gwliihhy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sfdryzmb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3srjysrtd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ilnubotl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bywpdnun.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uumysqft.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lbvugwym.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dhwogiej.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ufgvtiij.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eseqamoq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3npcffget.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kgyvdyqc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vimdblfp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nauqiccz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jjgyctbj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zgqegtso.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yziplahe.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3itadlkoz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vfxphtxz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lxizijyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txftfyyx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qvatgvyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzmecoem.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gdkzxmem.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qkcjdwzf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nzorhwjz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xmgbrqut.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kmbglfdz.html


<!-- 参考信息 -->