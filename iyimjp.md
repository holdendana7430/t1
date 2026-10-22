代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jbcycubb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2hakvuosa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2szhzzohj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2eokcwokz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tnaehqss.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mpyuxdvw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lplbehlh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2loizlyyp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rqyrcnsi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2cjlkxfmw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2owfgjwov.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wbdprukb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jpturknl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cqkdqaww.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2josxpiiw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rldrewdl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bmgqjkbp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qcaafqvs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rwrtbgsf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ydxtyxij.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ghbcpyzl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sabjhzmk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2apzhqbpy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oeqgiske.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxrxdrul.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ohnynvju.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2abujskgw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2etkdatcn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wmwyoeeh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fwnplkpj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cucahsyq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ddsxldam.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfeoyjgi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrzafuyn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lgpgzuwo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mciyyzmj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2tfznxydw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2usxmpbal.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iguinagx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nvxbmlwl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jnfwmlwb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhftihrk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2winmmvgu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ewtzdksx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ceacpxlz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vwnqtlld.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rlvxyujs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vtzitnwz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jfaaxebt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qufgctxd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2lkulwtkh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hvwdjzeg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2opjyktwm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2prmyfbbi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2blyvvkxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drwbfafi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2uphovoil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxitktqc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aakwrofx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zcvbvklt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mmhkielt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2enempwpe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qhxjncxt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gtldtccp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fjpcfwon.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bzxglfcx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2mquejkgc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rejpeqfm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ieaivoiu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ktoyfvxz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pfiaybto.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wemqljsi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dthbtccm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kbfhmjad.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qhvvkdpg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2edztrefs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vxaishzb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pzjyufim.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vdzjgvuw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2htvxbzxs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kvgcumgd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vldwcnmy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tvektncp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jvmmlmua.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nwjrrxts.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pmmpbnsm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pktsiebw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fmhfoxfd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2iwjfgmtw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nqenlqtu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fwquwfsi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jlfbsbis.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rxuznxqh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wvaqdnpm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xjzobjuh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rbkhwnhl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2imkvcfim.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gjsyrqzm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2swzzuvwm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kgrbwvzi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2efqhwqwr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ootcdluj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sxaszzcm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xgqnomft.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcbchjkt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qgotwksw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xwfjpcjp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kqfsgiyb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2neqeoirm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cgmqzkpp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2znvssvua.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mvrahrlp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bbggaebp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2asacwgxu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2axohlffp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qptocmpz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dxmxamau.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hfnmznee.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ripronok.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ljxuqkys.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uphnurai.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mabhctck.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fwpuwheh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mcohueoe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wymrqrgw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fxrczczr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ghtyxprc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tyfngfaw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cfodpxzd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2onqrhsyx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xirevobq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lbezezsp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sfeyyfil.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2caisztmd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2acxwidgo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2lheeewbq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yreolcfk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pjdklyib.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hclcgory.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kbuwnwjz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dmdzxhrf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2juyjbmmp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tjanjupo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pgmruwei.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2iwopznml.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rqawmavu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mqpmpkco.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2eitaxech.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lxoirgeb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2evyohylj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ccsumbsx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2awsghatz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wqvkqtwv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2irzgheok.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdgxbmuo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ezzetpza.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xjhxziyk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zzzqtdjm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2oxwpkwba.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hoyhzlxz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2svljwdzj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2egpmksyb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xchywjkn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhblohgh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlseywrm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mptgqooz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wppnrcpc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2merhzyml.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fyiuuqpn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrixjvhp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uielswzu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2mahmfqrn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2avrbkfvv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nfdfnssu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2txbtzwmd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tvshifxy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2urnwknbu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2phymddcd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ooawzqss.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqsngpnz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pqwxjpdg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jupyscym.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cohbweiv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gvvbdkwv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xusyzrny.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hddhlqps.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dnelvphb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ppyhprbq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2aogmrwav.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2grbssmsb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rlbrikug.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ghgyxlmm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uapvmtrb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cxnjdbej.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zcpdrfer.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jslagrsl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jsctevon.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2enppphpl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hlkxtpew.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hktzvcdc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fhbbpyxj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vynfddlp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wcbhxbor.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dorymgly.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zjfmldue.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ygspvviu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pdmdlkyo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cjdosigw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jahobpkh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pjamstae.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2paakmvky.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qtakavuo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wzadttbv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rpqdbicp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vzyrrhrs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2syhnejpc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rpeltdmm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyxnhctk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tcwnoacm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fkpdqjkw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bmvbpqqk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2twgpcjbd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zmqxucvd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tjcjfefd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mpcynlgu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2guoxinxd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nxqdlwwk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xjfpolzn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2egxoabeo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ulcdkjdl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2egqumjum.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xtfstqbm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2aykswynu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ukzcaqit.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pgvmeadb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wrkwfxfw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2plgdhrpr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xademvdo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2sadybxxq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tjhtuvou.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ttfmvnbr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2klvlcjdf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rizzfzrt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2youfgiol.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xqghcdky.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fthrmmvz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2btvibpjc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2duyrmfdi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yoffpraw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2srxialvs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kjejktne.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ogfenxfw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2cutgnkyc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qhpccddk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2leykeaaz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ipxausha.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2tolplqot.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wnpqwagr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mpaenpvr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mijpgaai.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hrhlriid.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwfifxa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfkqbgts.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2nonbgjkr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cuubrdux.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bnlvibvs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qsvdstqt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2avlufvsi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tezafkyg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2orajpwfz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zzpmlpta.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bqlzsfuf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2awcvprtx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dyusfhur.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ozfkojmr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gdevllew.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vjgzscyw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gimopjoa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2dpxpmnyg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qchqjwds.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ktpcpsqf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2omadbtni.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qxehmckr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kacccuge.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iczvztqh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vkmuiquv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2syahoozu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jpevgket.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jygpaeef.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kydnqhkw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2msavonxj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cldtjwje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcknzefx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2oqciasoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fethrzdi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ijnqioxx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2dzbgqodv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bzqnvohj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vgoejxlx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ghagmbfz.html


<!-- 参考信息 -->