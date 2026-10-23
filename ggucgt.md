代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jxqtwzga.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3pggjoubr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qwkyweff.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pinycnao.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hkcsahcx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fcfkzwqr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mmknlygx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zcnnnmrv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vgifsgyy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gsicqhrp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3qccvouiw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lhivyfkn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mexenemo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3uorigzsf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cihmmqqg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3etdqcpnt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3faypvrgl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3aoylgtsh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3dqaepyjx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hbjxpnim.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mollggwh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cmqpcjvs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zzitmkvl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3shajcxvb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uhscaxuo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3alkvlwci.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3coqfncxn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bszohujv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3indbgjcu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lnpjmzzx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rmvwzcdi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qvknhhmk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rxbrjhvu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cbrmecgn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3czgzadwx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3tbdsleoj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynfeusgu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3toyfdanr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3othbnzfj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3trdoigkx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzrjdpaz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyzpmfoy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3jcarqxpg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kbulgfin.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wribshtr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3prjzinse.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3osdfhsmt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nisukdic.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ghwpexmh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulvuvpgc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3twuhritp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jqoxessv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3whzuwftq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jnialphp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3sbuasesi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mybfmhea.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lukqvxjj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3gzqkxxgb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3pfvpvpdy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jkeadhlm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3npajmazc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3euzavqcx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ejebpent.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wntybznm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yspnesrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tywaitce.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kzimandm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kpggkhpk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cpripimt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sgktfhxn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3iebsuzfq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3omllmneu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xyekbumb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pvzcgfmo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3twlklqon.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rhmwjczg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vorpnnax.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eegujlgp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rndhvcbx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ppdkbhjg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3npxtkuet.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3grgsdoen.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nrfbliuz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3paagbsrp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hafmznsu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yjaqpbxb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ygvfeysf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tkvegmum.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3spmhdpps.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rkvolncx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bwyusbmz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rmvvhcqw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rpsqpqyb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3riatmlej.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3megpmtzs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3sionfzye.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kyuzdcca.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jnrhpppk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pjidzlgx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gonrsrcs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3iidkwuoy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hkrybpax.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xhbzgtwy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3acokczzb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rvjcjaby.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qpozxhyq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vjfuuljp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xybijwkr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xqnvboag.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3conwzsce.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vkszlpos.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vmwupnyh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hkqjweqh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3marqidik.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hmbvxmmw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jemfszeg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jjfgraov.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fqxjfbvb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kiqxzdsm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nbvdsnez.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pkynpkyn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xoivsmzf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ivdtwels.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wdnhgaqg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3odnaccwb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gkmeffwh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3btfhrhyg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ucsycmhg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kimuyiee.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3gavkkrlu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mwqxjdcn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ucyggydo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cstlbsuj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kqnvdqps.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3eaviixhu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3msdaszmt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jduuzwou.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zmqdmduf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3iepcyhfc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3olwrgerw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mpkuzptn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jrijvinh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zhueobxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3twtuxdxp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdgogwac.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ofhmnkhw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3qwidqvte.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3lyljicxz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sypdlxlc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pqilqlcn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gbdlewql.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3edvninfw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jgdwcuhq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3owxjvfyy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3khahcnng.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vkahsfzw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fxofawbj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rkvqfkgl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzhjpjpp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tbhppcds.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gylbdwqi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3kszctsvr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glbswkvw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jgndfgbn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bxtweqob.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ribqrfxs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tphmmynv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkssoixg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wrqctsdn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yaqbmpmw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3buvzcayk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhbcigfd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcxsfgml.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kkievlhy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3iymossnn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3whhmuggr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gmfetdlm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wyvvvals.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wswmqctz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecsjgobm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bvylfkgx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sgmkymay.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ixqxticr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3snzemwmp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ecrpacnw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jeveovfo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifiagkaw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xixeftfs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3yqsknjcj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jhqonmvs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3blcivbws.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fzjsqwky.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lscybgrq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ilvipzmz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ozczxihq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oltrmagf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nzljxtxv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uzojppvb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3luavuato.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3rkolypqh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rhvpyriw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lnuliqty.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvnqwqy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3temdvvvp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vozswdpw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dagctoyo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mbattyxd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3dmbmypik.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qlqmmhrt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zysmfqsx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tmtgjgqf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aanpeqej.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hvmglend.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wtdbudjx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kzpgsckd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3onrfmqdi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3toudusci.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wimjmzwk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tdayadfb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nvexadrg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pkkzxahf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3clhevkwd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kifxdgmk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rzrghjab.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gidwipvm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3snjsctuh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3awoicfjv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fbkocoro.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dgirlgxt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmqfqvbp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cupxekvz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3yjybpjqt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ydthwzgl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jiphygro.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vjorpetm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rlkigqda.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hpjnhrdo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3gvshbuti.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtnfeptk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yqdfrkdc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cpvqnxyw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ovlfxryl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dtubgwni.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gbogpfue.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ulprygtz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ztzdaofp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wnyhdwuo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rozeckqg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3izjwwjpz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctgirltk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnagrnyx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3peuezazw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ofbtzdyu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3scpjgxxo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjzozuf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lbqzcutr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3rzvmadnz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3muvnpnmq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nkqmndfi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3tdpmznvn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qauoprrk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uznfpkkx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dkaxiars.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3exkautpu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3pkcojvlz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zyoyuaiw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uamzllac.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kkumhsos.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3budvdkxs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bhsqrkkp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nsmvpzsw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3efryzxks.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3guqhiifz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3iaylurmx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zhpwcecd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kmssaqdo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mszsiljb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ephcgbmv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kxlcaoph.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lyujnamo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nfxnqtos.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mdzvkgun.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nobbquqb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3fctmtrau.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3usrlcgpc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3avifhvvf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mddqqbas.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3glwpvfjh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3izshbsge.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3liezixju.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3maqalstv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uwpcrbim.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vbxjihdd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3msxyfgty.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lffifzjx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lbbopszm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pboqqxgx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vqdfprec.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ubdopszp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rmelbtna.html


<!-- 参考信息 -->