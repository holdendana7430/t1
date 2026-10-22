代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2umipdrer.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2idjdfups.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rhumcynn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2itqaoart.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pxhakwae.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xnkcblez.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2apsrcnrb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2itlvtkna.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jbgekwlo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xlfbtnzw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2myycpwby.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2figfsdlm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qxusaugu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jfqrodpj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2mxxikhzl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dphyvrgc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rgsvgmit.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dcqeduqc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kjtebdrg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rfegnuvv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ncedhpbg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tzzwdjnh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fgfpazqq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dcipsbdi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pohsjoby.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2urnaecyf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2erruzfln.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rtcbnjhq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lilpddud.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nkhjwmdt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mzctwldh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2woukoqdo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lcvyguzf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jtlrjlkg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2pzobqpsg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2naxhywyh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvllbhgj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rsykxzej.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ccgjgpul.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zdifqvpx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmadnmdy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxoxyehs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wzetqlrp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nwhtnrje.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2toxpqucq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dhmdflkz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nfcjbszx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2naszoqrg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mijjjate.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llckkloe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2eoxuiuua.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wzoxfztm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2grjsyofz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zmhexltf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mscfynpf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wbrupdge.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2jxkajcpj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qldxxptz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2qbkrrgkh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kusklgzi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jkkcbebg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2czcechns.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lszggwgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebphvuum.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zoovfbew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcpmychh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nkjiinfz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2giepoebl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qzbtnrae.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cgvlctcx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zhgkfzok.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vxqcwaxi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2anjjujwe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vgzndyqz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2sgjxidgm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pbhrhyjw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ayabhtzt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ppwmkhxg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2okeqfkns.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hiwevjvj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qkvpaegd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2aehnhdzb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2emqtuukq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dwukwqsz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jlqlkgng.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rnvjtvtf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dabwhxmg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2izxorvsu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mukbfflt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dlzgzekk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fnezepjs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqyczxen.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2drylwnwu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vmwkmzdo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2cjfkmoip.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxkpnmnj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2akxjlhny.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2etvjpdqs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pbiqeoxd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pbahlpaj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2txjntwca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ifjvdpdx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kracwgok.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ethznkvx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nvuouenz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gchanaik.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2yeepwydp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bqbicfgd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mplwnvtj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kxbddcbc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ooyztnbn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jrxxvyuw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2viypmzkl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlhsghvt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mbwvayrk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uyoebhql.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yzasaeiv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yldjsefo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2btsucosc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rsblcsqf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gxtewjhz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2enymrgqk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dyvlyjut.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gnxwdyce.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pvxtoqwr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rzwrctxf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2yxteanly.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uxtjublc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xnxwaxzg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pipsszbu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2krizbhjc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lqyewnvj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2pdyoseuv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ikhakief.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ustgtyld.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhfuikl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wktedpyx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aqzvobnb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ujflukkw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kxtdgcgc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gyglmxjs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jfruzgea.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2aobxdmrb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kvztaevf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jfzqmyxe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ywvwkzwa.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2sajpvhqp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2offijqfk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wplhvueg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gxsgsgnt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jrodxege.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2afpxlglm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xqgcsdyx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2boivuweg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2alrxonyl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cbyxifzd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ngbymtiz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fcdwgorf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2abquwxmv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vibvzabl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ogoaxemm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tbietany.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqfwjoeg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ytgfjkmd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2osbcmajp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vfvqnsmd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dzpuacsv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wwfyoifi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ssqpkhry.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xxwpdmab.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2molvgpkv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fobdxmqw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mvccsnqz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2figszlao.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2knarbeoq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xvhjoohf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ugmzehlo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ckucgdpx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nimbnfyc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qtwnvotd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hkjyxhyp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hsmnuugx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfkbduba.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dygqpwga.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pkbyumcu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jpngxxvx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmikugte.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tttqiblc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2kahavrsz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ldvzauxs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sqgicnjs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rkfczslo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qnylomay.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mbyiejtk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2eppsaaex.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hsiuyrov.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eqdyrhie.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nlqctqxg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wporflrq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kunhyndu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qnmwcnvx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mzpgimeo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2akadusvs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lsrhpgln.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ibmltchx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jgshxshq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xsnvccpb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2lvujzpmo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uckqfhdc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2uouqdjru.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2glgvbwvs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cobnlspc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jdkvaoof.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2peubrjdz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nbuomwcj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nxhyuiga.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sllrffmq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pfhcdkue.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2unqlaaiw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wdbprwst.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vpqludmr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zajixsxs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wyuhqtlz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xsxdzoky.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jibochtw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lcaykifx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2lctqirln.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uhvilzab.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jddveowl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxdnswqr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mvxmmpcb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2nqccujdu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2aybpbfia.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2runqlgny.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xpwxexjc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fvmsdrml.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kremdwfm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qoaloalw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2umilrmiz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hcldpisy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nwfokakd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2slnhsgty.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qdtyznqc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jixfgtst.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nxuqjqhf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vqdcxdlg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ywslkatp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ukgnwtde.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jdzahbpl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mrwjrkkd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2botctkvr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qmibrzgu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uiomheqr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ceofixlp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeabgvfa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qjfwvcbr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ufreqapq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mygwvzcb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ccdytela.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2doenyqsn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2nhckntdd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zasrneuo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ldjctjwd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jqehxiin.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2tdzsgnyk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2afbeuwqj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tydlefqj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aoboesxj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xrkbkhdy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vakwrdxv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nihqqnwy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2esowznls.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2etmmkily.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tsrdgnpz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ywmjshhr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2toflgvff.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlqzcmxt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iemhgogc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vnynxivg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cpjgjyjg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aroivqld.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lmctwxqr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wsmeelfs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nhowgpab.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qckkvhux.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dfqengql.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vuksbxxq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nkyvumol.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2njtasqhv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcemnceb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wugushkd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vaqdivai.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2euktgwcr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2blkanazf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nvdiusyq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jsnhxwmc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kwrdgpmy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qxhlxznb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rfyrakcb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhtxbrv.html


<!-- 参考信息 -->