代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fhrqgcru.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qjachvwz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2yjeujfky.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lmekxfpx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2agxqzktk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vkmjysnj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qjevpdua.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tkzvaria.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hjfqfmir.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dtdysvyn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zzclbtxu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hgqafjzp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zxzmmdfo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jjjlgggo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2txnuxpuh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ugfcdxlm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2oqwlkxmx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2xievkzmp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xfqlctwz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jeexqlgc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zrqrjbkz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zqbtnodq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qvtrxilt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nnytpcqp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2snusczrc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2soayixcn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2narrhwjj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lkouycod.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mpwrgwvq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uawmyisn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zlxcuatw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2owdhkmmf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vheobvkj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2oycspwhv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2udfrakmx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jygmpwol.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nlanxegg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pxzopopm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kjddzrhn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dpkfyqvi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nzogdgoa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbimfmtq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2cchvuare.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gokibvad.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zxlqhjev.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vcrzifhg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2zqydztak.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yszpztdl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dwfxnpxm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdjweawp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ajioglbm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xprudezm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2yzmcbsff.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cpfcelwe.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xdkiwkhw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uwalpxqq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2diqpxudb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mumdfvna.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fvaaskyb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vywahbiz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qpbytuth.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bcaqcjae.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fhewrqvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lafgxnla.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2msnkihmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bejjcsio.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2itvpdumi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ajdzrfzs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rwxmxqip.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xfuhiwgx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dlxgcfdd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2falcgsmy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fcgcsfco.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bxixvkkz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qxieqbht.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tkerwovu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rlhoezjm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2cgskbenf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hcfgpdpo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cforyasx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2twhieecj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wgteihvb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jhmdfdpi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ofpvajkm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ftmzcqox.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ouqqnagx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dqzkufcp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2bzpjewic.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vxvguufm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qkrlcvsr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uoeduzdo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2afhlnokq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2afgfhjuv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zxmohvjh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dhdmaame.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bfvbdglf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pfxhutca.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2orusdoeq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2krnoddac.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wriktuiu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pzmbgxfk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dwdfqwti.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qrnodjev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iulgclki.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vhlnjplm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2myaipbxf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mqykfhda.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ubhurafw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2islwvqci.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xetdkexa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gnyfdchd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kedpnkxx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rqkllzgs.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pijedwsu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wuqyhyoy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2htivohpn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dkemgyqo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tvugblvf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xksvojzq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2njyfvklx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dwpnsgwx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tpnrvojd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ovsfowkf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lrpwcfno.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nkjimcrf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2igjpigzk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rqvgyizf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2avyoqffv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gzdsflon.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cmvemzfd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wdvwpqnn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pogavwef.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hfsxpllf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2sevnzufz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tbqsfysv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2iblftkgl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbhgufc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qxoggsgs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bsarydol.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vstutrgi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2weqgrzgc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2unhohjns.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2busjzbee.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ibatceuc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2citeqdap.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vfwgutsy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mfdkulqq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bsrxdnjo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wcyameyc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gkuqvsoz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gtoxgyax.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rdaqutgg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mfiezjbm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2lpdhuoeg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ypnbscas.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gmwkcsco.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ygbnwccj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2dieqhika.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vrsmiyub.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kbaeiqqz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gukwjhlk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fkgqaakj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2aujkebix.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uycpybhg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2icshoqaw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bwfmgwbw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2gsirtefz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dzeozpql.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ymytsesg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nemfulyo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jqlivjmh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjagneaq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aftaxnno.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gmtzgyqo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ufckdbgj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2obpjwibv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2uzlfbizv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2oxwrxwyj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jvjwsfhy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wknoomix.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2pwjqmduh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wscjibfk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ahybydho.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2aukzkqjx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2hbimvmvn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vdpcqrtt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkjjcxxc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pabmhfmd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehffxisz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uwfghoyx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2duruhsot.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cwfgcdra.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yehjygek.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pmsncfkj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nxnacxmh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2btswxori.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iudzkzbb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2kztksshs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2yctdtgwi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ltmbuwch.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wgkazusi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2doepcaxc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tptfopyr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qblkhzxa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gxabwgou.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zfrgagfe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nbjagnhk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2demhxogk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2enjscyvk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2sqtmnqct.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dvoudrus.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfxmpsjh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xwmutsby.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhzehrc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lzyrbyzh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2eowbublq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2duscnovn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dhlxktne.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2pkxhvquf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2oecshhzp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2swdozvvb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2clmkgqwu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yxachilg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2sklbdios.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hpuuchst.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hxzdynoq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dtdsqcsn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fpyrmqdn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fwsmgvbk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xwmabrbq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vqqxngfp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bhiuatfq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2iucqmzcx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2heelovxr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2mhzqolug.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmekcfi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vtyikmgc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qwouubvz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2egtcaxif.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iovxexfy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2koivomzb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dfnmtasz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2tognugwe.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xhsccqeb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cqmpikml.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lsjmjgxj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cnpozczj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lmkbnmdc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2idzqzopa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jajbgrnd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kixdeipi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkifnmvq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lprfcukp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oirskptm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sfkxlpkb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2szgnnfwu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hfbnalra.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xqsgvwit.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ctugllrg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rgpwbujy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2owcnutru.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nnyejtyb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lmintykq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2izajucmx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xekrktdn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qwazfrwv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2myhbwaiu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bzihqjwf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2amwyupvz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xlquzpxk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qvrrehbg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rxzhlvgh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ayjxvucr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ubhzevyl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2iwqdzdir.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ahrsyywq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skrhdedw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qsudcnnp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wxlubwsx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2katkynbn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cuganzpr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gfixxihe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ycytliji.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ymugygat.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2dkdeqhtf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hktzqxnl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2tqdzlsiq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2voyymwcf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vspkhvbk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvxtzrbr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2shfbmwcx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ajzjbqog.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bliizupj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vxbgvlft.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ggbetvng.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jfkqqruu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pubnvbze.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2akaovwne.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vchhexct.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qcublbpe.html


<!-- 参考信息 -->