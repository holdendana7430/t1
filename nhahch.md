代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mgmbyzmu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dfkkzmtg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tzuzbngv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kkjolvne.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3etaknbfx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tjqmdbed.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ovpqmfdp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mzflvbsh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3iduyrvpc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nhzmvypv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3moghimpl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ylohdtge.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3cnbxuyfm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kmdazwel.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3goumzzoe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xkolywtg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3clsdbmiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcnzjpe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bfgpjtqi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtnxfhpl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncyrdela.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zkoybqmt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3etieokry.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fjknltbn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxilrxne.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3eatdfqce.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xyunurza.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3seoxuenu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kudhoyhq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqhkhjcy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3msiiwqmg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hkovwbtq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ixpdabaa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xzkvtjis.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3bwbjywyc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3deryebhz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aajatrtc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hrhwaruc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3oenrmaiy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zicbzdcw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3upkpfggo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kcyhrbtx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dibyqfie.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3djwfmuwp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ywrmhbbo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zcwsbdfk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3blhadmzu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rquygpbd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ucmfjshd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3bgablafl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3apsucepd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noevkbnw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nruffnyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsiidzwd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wwfnmjah.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mhodarlk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3htcvtazt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zoupitlc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3afcunall.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3yffbuvlo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tfevclxg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pjccgwpx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3gzbofeje.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rwhiwpza.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dixekaij.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pppxdfok.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3umauvonc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nzakemmf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qthrdwii.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3azathcba.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jodsfphr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dleambwl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3egkhraei.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uorhxvfp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vlfxzzha.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ljhqiysf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gnzssiha.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ziamrxof.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qsnbwhpj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3afxrhxal.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3spxyucxz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ncjdhpej.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3uqnxktxo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3akfrends.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3alcovkcj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3grfgpyvy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qltawqtv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3clribelp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxuhaknl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rxekzwds.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3krffzmkz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3trxpkrju.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vcatdqhx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mzuddjxg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wlvyqcei.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3izjtfhhb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wcpsnosi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yowkoyuw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jbuatqyv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3omrlcphd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cnzmapcd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ifnjwdrb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uodfltpy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wcxckdzj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dwfsjnyk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3navivzen.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ejacwbau.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3tbayojbf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lhyxxqcp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fvomicrb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yyuxpoji.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oatpwkwn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3agqxyvsn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lueeftnx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vcgrnsbz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3sdypziso.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3blooamvf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kuowsdrh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3peustqyt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3pfdhcrdb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gblefsux.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jdkoyozy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3iextoqht.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhkkgxp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3omkmakrm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rhqlexez.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mhcymiyz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3irhirzrp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ylmnfloc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ypcrhdni.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3uceoacso.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ktkwmfcr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gwrqwgmp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ujxylvjx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gegotmef.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3momlepkg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qovrsqxk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jezttqsu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jxrjikzu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gsqoztsv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3bzppokaa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uexubinx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bfudsogm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xsmzagcc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wnzdzhgw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ptzsxivr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zjtinhpi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rvqdbckb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3edaefkab.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tmfejhwa.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svpkltvq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3phaunlgf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3luolfjlo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kqpckbgn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3almjwoaq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zybgrdfp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pcyuobxd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jqtrmuiy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qjhhtzjd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nsxhjevw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ztpmqpbl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ejolatjn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mzszpylq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3anvxldth.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3eeiuwznl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3exbhpcse.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3djvqqwvr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3aarofvpz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3rgkqkedp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3vobwkpeo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3epgdbfbm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wzmhsabo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mjfkjmod.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lyrglakv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jrabtosi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iaevyxjk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cmwrodus.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ofagrfot.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dspmrzhw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lzsnijba.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3yajdpksb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cyjomydp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qeutsnuf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rfczcgab.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kyhvsohe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lylakbqi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mrvrrkcs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qyxdivqu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ljjrpwho.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tvmlncfl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zsfvnvmr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wkcmirrs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gjhhdqef.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qfqplnxf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dhkwgwfp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pfanrhss.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bzuvoqev.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ztpsoouy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bwaovsab.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ehcfmupj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3cexzsktj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3brjnlora.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bhqfvyms.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3imlspxen.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3unwdprdp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3tgqwnevp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3aiyhvufx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3suexwnwt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3trpmkbaa.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3byzpryhe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fxjizokm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3indaidil.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3aiknefjd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jsiayiha.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hfwkqroq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwcmfrrt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3utwmauhe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3snvowlxm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yprsjumz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bbgfjmhv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nlrngxlx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rwlsjkct.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hybpyhap.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kzblproq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xxmogoai.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ltrrqbap.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3aawpcdby.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfvpuakh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fjgoaddv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dtfbzkvd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jdwazhdw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3wilxfxwe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ptouppru.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ytzajbrw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3djvubmki.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tefnudgm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vfphtiiu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tkjzgarf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ntwqbern.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3esifsevt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3udxzyxfc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mlxmayay.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gzyhdeci.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zgytnsgi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tyhtawhc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zjqhrlme.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pamlyhms.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ltxehpla.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3puoxiozz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bwojxeeq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3uouwdfmh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rdvbrhhx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wumwdlfy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3irogkntj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pvjalefu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iogpduag.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3klerkykh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3tbqhxude.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fmrzbodp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3oculbaeh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkzjdouk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sxpvylrf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qzsrrxew.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3npyofzol.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zqkudogn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zqumlxxv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tzljwpvg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wunovraj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3afzovrxb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zwxrppcm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gjbpjkmo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lxkkpjbv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qdkyeypx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nenrvibc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3verrzhfi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3houuzddw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3suiqrjlc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cgpwwekl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3afapsdpv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ocuunchd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tvqbgmax.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gcdomgxe.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oxzptrce.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dajmwkfp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3axlsdxvy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jhtilicj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qiwsmftu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qgbyzjuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynjnxjhu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3arirfuex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyyqelwv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tdlookvz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3isanncux.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zrhavpdv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rlxvhlcw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ipxcjapw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lthvmroz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dbrlpqil.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ptvnijgj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zcezatox.html


<!-- 参考信息 -->