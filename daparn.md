代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jxehnxdg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpnuqdyy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3klzwtixk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3crytvalu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kkzubnua.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3liexrvlb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3guiudhft.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rtbvsnbp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nhcmxdnx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qmgnnijk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ruqqjctw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wetdmkhq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3efeldrzr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qfknmlym.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3isbmbwnd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hwbrytvy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bygnmzqv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dkdfwovd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dguvwosf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ugdtgees.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3pbtyufau.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mpgxrwjt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pxxsrjds.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3nthecgbb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3urprkzrd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gfotwcyg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lbpystvt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dpfghhhu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qqvieoon.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ihsrxkcx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tlgjspuy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ftzoqweq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3peswwjgb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyxtymdm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tqwffsfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lbfhzrrt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ylbhdprb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ecowlcug.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pvsbvyrw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cotlqken.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3crpuvasd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vlpmcdji.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kpkviido.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rgcdpqzo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xezxlrdt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyxnohne.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gklfnwxk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3apdegyir.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3yepucdht.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qjdukzfp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xccaehgo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3jtogsgdx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szvhzgpb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyobpnco.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ydfhwipl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hnbqgfmy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rzhpuugi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fwoookmr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xwzwgbpk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qxemcitz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3njlhtyrl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pmwqldiv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jftmlyqk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qeyqezbc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rbezkxyc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zhligwfr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fppihjzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlctfvew.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3voscmdxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnmcizxu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yfpqgfwb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mvibmwko.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kehdapxo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3grnpmndb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tmxavhef.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3btsuibjn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3oppvwovm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bgfvsehb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3delyszth.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fviavjvm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uewveguk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ztexycis.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jblnsqmd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ftimdmpe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vbwsddfc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gdtouieh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3eukjxwcs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ipqjawbf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ihveqrww.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3putrsclo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qcpwmhqi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3cydpndqo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zypeefmm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wdhprpwg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kgrrkanv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3bydovbea.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3riolxjbb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mmdmadlz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mcyuwezy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3agprxtrk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ikptfncb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cmgpcbex.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hnljkmif.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3orywdlol.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qjyevrre.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hceafkiu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3dlftuybg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ewzqjkop.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3knogqwqe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ktsnziut.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pnifnbui.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mmblgyzs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mkfwhztp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nnzrhheb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xjwufqnb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pvrnzrkx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ydhybgfu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yivnkmps.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cyymoxsp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3skifoznx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rbupbagn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nrgrnxty.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3epzptdka.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pnxurrvz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tqzhqrcb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jkjrkanq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ikeintfx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jmbnyplh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3viprqeaj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pmcvgzxa.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3synydwxd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3oeokvppk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3smvfxibb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ntzmckvl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3fjoudwwx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gvcohnbi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cwyeljyi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kgotzqwg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kwnsbnwv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vuqdqgbo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xkojdehm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ibhrdysh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qzdgyxnq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ssykwyfg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3dvhnfnzg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3acwxhayr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bntjweia.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3oazcjlpr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jixdloim.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3puvrsrbx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3yobrnxwe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zggencqq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wtockmyr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dcncpbxh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gctgwign.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nvelwmax.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ytkxeypl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pbgdxjzb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tdgskevo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rwjyaxlc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3owskfmox.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iqjyhqxf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eoolthtl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tofkdhuw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3uoqxpvtq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3aqdhpyax.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3tvujxzmf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dhqkvrre.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3sbgwgrte.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gezbxkyl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3evuizlkd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kllzhuuq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bqktklae.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjqgszo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ichbzwzu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fqrvujxd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udevvslt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3coqbjsih.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3srnetgwa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pcyhbegv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iabfrvjq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xumkeknp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjslhnzf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3plztpfgj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3iogplbkz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3lwnjnmpv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3znjkfpgl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rraahlsv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zxkbbmgf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3loutzkzf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqrswsfc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypcplxza.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iznucqsg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dlzvfhuv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tbjhwnve.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3urtjvqlj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rgjhsjec.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3stahwiru.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bprgfque.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3luqumwcw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ejrfvawa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nsidouoy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ugcrlkny.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kahrckho.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lasntxky.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xwcwiglz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3osdpihik.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3olxjwfxz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eiefvcya.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3scxczkyt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3okcgctsm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pxwnoeko.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bgershgf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dbswmgre.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3snefzenb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dcgilwda.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xfephrxq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ddqfmaci.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hrkbrhhb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3uadpxpny.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbnhsrmn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kduoxfkj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mnqunmas.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ovqxbhzk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qvqjjbzg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3jzmfxdaq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3yucjqezc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hinuvtca.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gvozghjx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dniverwi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lvbeojcn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wjxvdoap.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zawszweu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3bawhmllt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uzxunebw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qqthxjbi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mjkrapjx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zlabqbwc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3thjvccev.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3icyywvmn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hnjppqpl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jdfdgnfn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3raongovx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xnhazqxp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mjtqhsvc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ctcmnxrd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bbkvuagb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wbmokvdo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3phoakdkb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zgvmhkdh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3axphhrwx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vbykhlzu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zknthwos.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3isgvzeuh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ifuzpwys.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3inhyazqc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3whnupxkg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ennwsucu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkofkakr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ouspxnng.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gmjtgenr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fuwtdvny.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmztyql.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gdattlrl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3eroemlug.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nnysehsv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qjloczjd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kssxtpfz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3rcqxqwlh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3raamxkav.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3croxfeyu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3czuackmy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aanncbzo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jdppsgqo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wxposgin.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3endwoaan.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tvnhwwaa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mptoivaq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rnlfoopm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kytvvdnd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ohbnksgc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hnwacisc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bjxwrebr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yggqftjk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dppmeapb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mfjjmhjb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3oiglhcfh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mdwdoiwv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hfqfwfly.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ljisywws.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bqdimgbi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3atagdofl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3idrrtygf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zvwohxjr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3iwjahjlx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3mircnmph.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xpumoqfg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rjxaffpf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kgahvclx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iyitzphq.html


<!-- 参考信息 -->