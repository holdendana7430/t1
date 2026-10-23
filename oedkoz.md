代发 wailian999

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kevtksoo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dovjwujd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3lqtmictc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hmoouccl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nmymnegl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3labwavzr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kyildehu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rxxsnryv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3dwxfxbul.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3aiaogniz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3fqiucnex.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ufxpbmau.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3pbnkzzwm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fcyzvjvc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gvmzoqns.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3oaghxydb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mtavwzon.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3odelxaac.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hpuwfomc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ncsbznhd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ityhupfu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdwdxloq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ecjpkoai.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnjpobep.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvfcrwqw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3porsxaxi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3crjueikr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fvsmyaoi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtmsksoa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qlcdzbzu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bedxfapo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dlmmcphx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbybyhl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mtdeylsn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3glpprpfh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ffmodbcr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fisolqnz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktbkahwh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3iknbhdke.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hguxveem.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pifmxcqi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrenayih.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3icuvxsyc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ltxstisd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tgpalymo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ockxhxfl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qxnqhnhr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qdelxgsi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xebbztte.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hrbzjuqh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zgdlthgy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3samalnmv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dmkksjyc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jwxknknz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lddfvcvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtrobbjr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3rmrcxhta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnnfbfzk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xpfbvjpv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3iexvnrgk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pbkocctk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3timoeiql.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3umvvvobn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hkyyxtjb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3fdofalrh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jcnbzhhr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3sxovuwxj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ljdaergg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3akdaigco.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bauyqkjh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vjvitbpp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sapldywk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3yyzthdxz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yremfohg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ooogjizq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ujffpimc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hdqczxgu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mtafworl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xhefainy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mzxezgvk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ugmesvrs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3caddldqe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cdnqkmaq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3esdcissf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lhprihyl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jynlidra.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vegnyupz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwfxenim.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3dcyvgnkz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kuobtosb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3csmpgkqv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3gtroopnj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jvbvzmsx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lhblnfqx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jrsbofyk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tsaapcxn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gzhwpsce.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tyxcgoau.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ylfkueia.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gepwvezl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3osjpvbvi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ufvuxshk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yakegaak.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kjsklglg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbgfduwi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3peagtzxb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynavfstw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sczthpwf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3naxqtfdc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agbimjbp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hiunvusc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rwlncqqi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jveaucnj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kcbbluhi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uqrvxkeq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ouzgoddw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lpeiqewy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fstwogni.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eijebjix.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iqaoqixe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sqvusakz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cxlrgllr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kyrzxzcb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3muvufuik.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ipntgprp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kqmjcnty.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qnkwlbhn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3uqayhkuf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xbnycrjy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bhxbxepb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3buhyjnkv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jhetpzpn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ejsdtepm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3blwjumps.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bhwmhtlz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fdsywggo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sicyucuj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3raiuvsuk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lbjoeftl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qivvluok.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nyganukw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xbxuglbr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sprmgutc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3apvggwvo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ncysajei.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3krvlqydu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xipihjdu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ndwfubvr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3uiccqfoa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qnflfbyl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kkszgvmb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kbfnmiiz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pggwzbtb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ekcngbhu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kymrunwj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uqaqkywc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3drafckzs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fdjcbmoh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yafadfsi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nvlsabdk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mzynlebx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rixmznmj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mnlparso.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jucrvynu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wlfdtmha.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ejofxiri.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yfeupmxz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jtekilzn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3aumtxhca.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmiylcjo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rwlxsbnt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dovsddcq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dhsiukui.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vwjpblih.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jqxevdjs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gsdgcjkp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ktjaynat.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zzhtisqn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3thlaffis.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bvdtkwej.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3laevejmn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3okaghsym.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rsxagrdi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dyukptir.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3duxyjtap.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vtupoiqp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nyyszhac.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3unxgwwww.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xvyorijw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3stwkapcp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ohdxyyye.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rfnjuzio.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wsvyjphj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3sttyfzyi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mxmxtxfc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jlgnurya.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3noxkowxb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dikhjujt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nhriujaz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3aebprxio.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3sswvrwhr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3tslyvhru.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3pfmfzczj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gvowtyfm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zolklljn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfbmtmem.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wwjlagra.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qftfjlml.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glyykbzq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kfcuxsww.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zqzmxbzm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tuxgzogf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3utbkadey.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rwwhibgp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ydzjkklv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yizlhqio.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfwjnazv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3eqncsnud.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3cwzeredp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3enjglftm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qcqwjqkk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdrgiyzo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gcvjfayd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hhhefclh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pswjhymz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3cogryqdx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3uwqnuevp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pzwvtdpp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fnvzojew.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3shmatjff.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvsabate.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3enbauile.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3reumlfvq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mjmxiusr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uextojio.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3mupvnnyf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tytyabnn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dcejxfke.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dwunzsuk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3lunswzgv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3brheuclf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjpuwgcq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yvpkfgia.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3howidrxh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fmfpprix.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yenyqqxf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fkgffmup.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qaapqxtr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkrotnmt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jmfgwsaa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3eojzuvkx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fawiwgzi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gnohxbwj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3icszkejk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3yocbzumg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lyespnxi.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bdnebqtk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qarblowv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kswmxtkt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zadrxdaa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mnsuazyb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dllqeqqy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3svmwxyeo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3touijdrm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltteurpe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vhnogwru.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vinynzgf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xyrqzclw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hiocrpvu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3afoenaah.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lwxlsvld.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tcxkqzqh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rnviwcbt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3youcqnyt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nrirnsyv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zvphsvrw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3czxdskbf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zdqzmrat.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3upxummml.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yucijzui.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ezabpzyl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ubipgyde.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ffajlfyl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ogtsebmh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fuyzttxp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nwzkgsha.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xeqdokdu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ibjcnase.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rxtkkgvp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mehpvlyz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pjmxhhzc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mtvzgdco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcxnjnef.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3oyukddup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kowldwvh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xaecolrz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3duurzxdu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3alvwbrmi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xnmkrqvq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oqelxjnq.html


<!-- 参考信息 -->