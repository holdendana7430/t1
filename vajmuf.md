代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2exzfsppz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ijerbefr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xcjzquzw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rlssxkui.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uhvqfmtj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nhkzohii.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lfuddcxz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2aanuzunj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hjyurzuf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xsshrzfj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2awnjfyjq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zghbybya.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2xyqlhmbh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2isiilpmm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2nvheqzcd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2nawcztkr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cmketcff.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cezxyhdo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pujzndxi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pylovell.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qncuutrs.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lvyxhoyz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qpxhebfg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2iwhlhnsw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rjjvdsyg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gghjwpyc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2thrfffvq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jprzekxa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ownphlzj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2aufvfpvn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fetukvxf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ejytezkh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fnctdgmt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2htftrcux.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ezdobpmi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2igerapje.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hrcykgjs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2kmhqisrx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2bnsqcnqw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ofwgiclk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gqricgkd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2juiurdwl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ocvfylft.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nexwgdyh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xmdbmrvf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ullbxnsa.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pnunseyg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2adnjmlus.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cnwkqrwk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wkzpimsh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jkmebsvl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fhjnbzuj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2aciybrbi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tqifnoel.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tlefldtb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bvqwhyba.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2icwoajnf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ulaphnxx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2avuptmtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iizzqjop.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2orxyvntw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwpnvsuy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rcontfda.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ssfoyyys.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eklqrczh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gmnbmonr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2lbkzhyuc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2edhzkxea.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tvxhhmyp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zbkafcxa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2iuhtqycw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bkrzazbg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dktoqesg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nrjkemgv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xwhfeccq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kmqfkcsh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ysozkiqp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lcmcqdez.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kqoqilfw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2piuipngi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uwtzqshc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kpjfwgex.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2upnirjly.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vrihrxhy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gdwsmbho.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ozheffev.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lotxmyqb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqdsbzc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2atixbbti.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kfhtnvzz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gadtarxq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2zxagxeuf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mcogqoma.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2yxbcowoh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gfhqqrpg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mmkikbyc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2tjwbfkdl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dvohpnzb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zbffacwh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2raddigby.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kmumubli.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dbjbsptu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cutnfclr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2fwnyfpjp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vpruujlf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2unxgjtxj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dmbxviuf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2peornhsq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nwihifyt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hmovclwg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pfrdgvhr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2krbdtckq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2kqgrfcdq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yvgpxyoz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wzkqzdhy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2axnvulpd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2lyylpenw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vjhdenbg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pwrruqva.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gqdjibck.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mvcvxhcj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ectjsspp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ggframno.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mhztvpkb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2upswabzy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2faggtcuu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2canswjyi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zwiebfaz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rgtkaxwc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ylyjmyki.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2pcmyvoqn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ndspfqym.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jejpzedx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vjdnpfrm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mbyzbwnw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wuopiodp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2przyhvsv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vnasfjnl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2upirxirv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2osmkotdk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tctnifdr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zsrzswdq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xexacrpu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rfddugjc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jhocfopc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2prtewwrx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2binpwzgx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tkmeekjm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pgbdvsyh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pymeuxaq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wuiccnvd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kxdsvvex.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fjdwnjow.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2becfpsvs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2celjtvqt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ndedsepj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ltxxymwg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xonkapjm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2cjxttpon.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ozkcifzk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2odceibvz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fgqzgvkm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qwbbasaw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2meeroxhr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qzgvudfz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ouvmsdob.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xvnfaokm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cpuphnpu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fauoblaf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qnrbzdfz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2iofytede.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zgiswukg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2omknhkhj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nvxixezt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jqtxzmow.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ruqscqup.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ixtupflw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2elueqjgr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sunswfvv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bghfuqqp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ihoxiokg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omvxgppp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcftdbmp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2peainmbj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2khasddsa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hiehhauq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aamtyqgf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iqjlcrvo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qfxqjczi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nazpcwhs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hepryedz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wdlsnkhn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ctqrmpac.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tkssprat.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lhuipnsw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qmekchqv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bckxxtds.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ryvfojzx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhebolyk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jahbwkzi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmfyruot.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jskaarnj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2cqlnjdfn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2quzeajys.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2msrltkoo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xhpmrssx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kkmrasat.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vrxdonts.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2icxcdxtn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iywugexl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2luxfoguy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xyfpjjcz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2crrurqcx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2oijveesu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jsrbwimd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tmjnfmwz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vohneces.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2cwhbqmdf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2sucrgphj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ilghrygk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2pouukaxa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mebpvabj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hnfqulfz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hltscfry.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2aqfjqgsy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfwmxfwx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ihdkisgu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fzbwaaii.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zhovpzva.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gdjqjxlu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uhkggmao.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wqijhter.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jseyhapn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mzjccgny.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfydime.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwijaleg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ptzzscvf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ftgzovfv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rcxubvjn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ofaaprwo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2roqdfdzi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mapheuwg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2mdxwbfru.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2embjynlz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dskjtdkv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lpcxvmqs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2swakmmke.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aeikymgg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfhxtevb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwaettnq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfeqrvrf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wmvbqfgv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kjxpiftl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2yclucdmj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eclbkhoa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2msmlpatb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hdzeivpo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wqqecdnj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2aoplqzlj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ikygnyem.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2cgmqieiu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pwgoghry.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lntnmkfc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zlwofvez.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xadokdag.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jnfvbafu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yxjrtrnl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jbtugvaj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2crwjsbej.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fvuflqkb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gundwukw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jipaxyoy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gbhukzjt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pcuskzjb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2evzncixg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xigfirxc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2dusagcyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qwglbbqi.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cpyfuylv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xyfxxdps.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dkskqrtz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jnsqqgyq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2mtqbgsuz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjtvnzw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2klblfciv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bbnqytng.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2easbancx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ocqzgdxe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bhmcjhyg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cwwvsxwz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pppkyunl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aboimuix.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kfguwgvv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ryalkkjy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ndpbaqvv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zuirqilg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btatvyvq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ekxophhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kenwiqmf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nkyyufwn.html


<!-- 参考信息 -->