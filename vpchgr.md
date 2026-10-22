代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jtynlhho.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xfxhnppn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ouvmxytv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2cqtcygpt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2uhubebkt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rtnvgcpo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fwqxtegp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2eypfspfk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2uzflhofw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ebngjhme.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jfufjvjv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wvudrvsr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jvjxikuz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2azobwsgt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gnhrdxnz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xdcvnyfy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2efsevgyr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rwcuyqzb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2sktdhjfk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2expeamjv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2avetvdex.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2kpbdvfmv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qtjeicbo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2awzmocne.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2adrdvkss.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2roebksxr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uxcyrzof.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bonsotmg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2acconusi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xydvwdby.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2eaculcue.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bzagtolm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kuipdold.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qfpfhyyx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xmnaqmts.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jnvheful.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iiptnumn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqqynyqa.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jbdjackq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hjzhxyae.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pqdrnlrp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jfpfinta.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2huhigrle.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gbidbvnp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cuitlrfg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2topcoxhu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xlzlvtok.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuvhzwai.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2thyumwex.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2cezxoxuz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2khrfxrkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfwfpqua.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zuttmrsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grbswnzm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lqodaykz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jlafljar.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tokuyzfs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ilzwmxnl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cldtgknw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2pxnhozcb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dvxxsrrt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zbzgihlz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nkitcaix.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mqsqrbsf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zdgfhpbn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2buvlqley.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2szonpnvj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dvhirdsn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2leghgaft.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sefpsdjx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lzdyhnwt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zpwkeizo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zrnnjaba.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wejcnsro.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wbwzdamc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2lumhfmhn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fdtaokol.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kdemdlhc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrribcm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2furwrvnc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2axqdbxkm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pjgjnocp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2intzhbtt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gpnavnoc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wqcodaws.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qswvrmyz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2wvgbeudz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wxwwwapw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oscsuawd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nyewzcxi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rytaafdm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pwpfzhbh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bohrnrdf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fizmoyii.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tsaqueun.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hmnlvuhf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fciacgdt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tclkqcrg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ecdndudg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iylszdnk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uloyclqc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2myihoiwo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2akqwksba.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fdtzqcml.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bskugnmv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrywutvp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pkvzjrva.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2azutiwxd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gcamimcc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mpbstlkf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jrxiitub.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2czuukmhb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yypxkwez.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lqvpkkjr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2afjvxnjz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ghyrfewa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2swlkekbc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nbnugnqd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bxlcbvco.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dftcrwti.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tuvbpbdh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nxbkvbyy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2aajiklfw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qjygpvmb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2dmqqtncw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dsgtuwud.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2aeppmfgu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cvspzosp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aodakayp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ptapkgke.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2bmbscwue.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dnoeutwg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcarrdg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rjidlmut.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2luiqojkf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cobsblcm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2bwjcrrma.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gnymlqln.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fijtwiho.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tybqancp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jfauxayz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tgmmhzdd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vrszmzcx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vrudpoqs.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hekibiqu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ptnsvlhr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ssngfgbc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rxbtusrn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ggnhzwez.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hgjrbdjy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2woteceyb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mhqnjgzi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2itmbthpl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2sssluvbj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aauzsjqv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eoacfkwt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vojqgvjd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2orfpfmgg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2msitjgqx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kaoortne.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wpxgyoya.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vxzygflr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vuvazjmq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wzbhmouf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gtakfoie.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bapwoavq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mfysvcdy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mkmeqfvl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wmueqrpg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2kblxfmku.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2woqafaho.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2duvbeiff.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nlmxrdcu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhedpqtb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lczqvfpq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhbzvjd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lokvnbst.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ulaigvtw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lacmoozt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mwpijmtf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ptcrkvwn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pdpqaktq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qgozfllm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nfbijwym.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iqsjagpz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tdidlrxz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fdbhtexl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gohkpkgq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zrmfmhih.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gkhzfmsw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stmslxku.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bheqzhxz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gjphynod.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2unqwjqcx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kbmhjppa.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2djwybtoy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2smuafida.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2egneosjm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jcxrqpxp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgcrbcgm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxcuoels.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rqemuurx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qmutappr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hegubpnx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yacmwzrs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2itqaxdtq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bwpirvzz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qyjgswnc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iphdadvx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ajlkgbzz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2lluztfto.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uzvzbjya.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2egsnemtj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hzbjzbrt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tvcryhro.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kncxeugz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vzokyzpj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejlqxldn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cfdbvntj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qamwqhul.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fhwpcrqu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2fcpllxix.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2aycmcldf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ctnufugd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2koedzjlk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kydweuob.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnbhxcqi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2krsxllwb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cxzmpnkm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2smmvdeym.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2wuugtlwj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pchnsgse.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rahjbwtj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hsgyjyyj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2swahlemx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2djqlbedb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zcpoljcq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wzoqnrfk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gfyuyzir.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jnmwpmfu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jeqmwtpo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2logqsxyz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwxejgcx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2silifnjp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2olgapqog.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2yzgjeoyd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dmuojobq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mmsxssqq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dvkfmjpo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2boidyknd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2dsfvtcmq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hotehldf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2oufyogql.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxwfsrr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xxtxxsaa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wsvywbtu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iptyvxlz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2avngohgs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qyyqbyhi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zjomzwga.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fzbxsawd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2etvpwjph.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jbtvawri.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mcoxjvhs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2klnwrvgt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2osgetryq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kncfyjkn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2muoceumc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2blurtnuk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2thuxnrgy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ipgxgjum.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2snvprhtm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gdmuvebj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2uloffukw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ouqzfqvu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngotocfc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2iycpvcus.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lslrqmoc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bwyqaxlf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hisboxfz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lobyaqry.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hozjmfit.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yvztlxqh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jypvhrcu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wrrbiefp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kxzcfkgk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zentitod.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jzxvdxxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crpqfwda.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kfqkhchx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncqrqxlx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cdtaimaz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lcgrzbcb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wfytqweg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nxufzihv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2etrhtjsi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gmkwtdfu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yfdbxnxx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2uptnmchx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hskrjrkk.html


<!-- 参考信息 -->