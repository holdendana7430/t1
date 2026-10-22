代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hyhwegic.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cxbihwfr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wlzwvnwn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2toipfkba.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mgwosynm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2roojirpz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ebschpve.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qrvggodl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tswwwafr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2iofkuzby.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gazjxbwr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xaoaxtki.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2negilxks.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2shtdxfcc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2oflnzmjp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tawbrjgx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2psmpucif.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qujewfyz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ulhxiibl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2slgdfehy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2whxzwcpz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2unooqalw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qotiswdv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qptrktfj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gyabeoft.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uinguewr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2metlwqzo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqexpxfq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgsuofwj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ddbfhrlo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vjtjlcbo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2nijfddiz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbhwapkd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ykiahlet.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rxkksgqx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qpabryjf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kzwswdsk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbqcyaqj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2znvnzekv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zmofrtls.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qbacrwql.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uufcrcja.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2koapdgtk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vsuzmcjq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hazodnhf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2gqdecljd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vezlqqfv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ycmysomb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jnhvtnfq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2oxjgclad.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nslmepsl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2alyxeoqt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2lfvrujxw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dtgnrohi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rczbsawx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qbceeuiy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2wovntmqr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vspuonmg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zclyiyxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxixxbub.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qxjyvwod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcvlsdzq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mlwboepn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2reqqnkux.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xzghuvkc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vneepijr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nrhqdrcj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qttngygu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ilkxakyn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rnlnwmov.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2naprqmlh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dqxpqlyq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ggkormse.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nkmudlcx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uxyowriu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bmjwbmyt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2sgyedwml.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2anovukgg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2xaoedoqd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xuqodcjr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2iczghqmk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tyvmpdyx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fijpwdub.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hajdtlsk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gmpldrpk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xhwphecu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qfzoqdei.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2paygxlcu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2euphsnxr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2yuhiffgq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xdgeixdb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2onlixgjn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qsdeyezc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2plqikinp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2loogyrnl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pbypskwb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jjufcwln.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2shwplypi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2autmcoeo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eevsddvd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vrawrgfr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ruvbqkto.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2exydhnkc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bdekgljo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nrwvcuva.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2igzprtdn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pueieqoo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iwrezdmk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jlmgbdcb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rfjzzryk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wvcvajbq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2eygqiyze.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2marwtyay.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hoxvjlin.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2urjizigm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dyarlnjk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kbtilhuo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vhiypals.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2immpscvd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cxpezntm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iuinllzh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ouuqfile.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yydjcgsg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tkhxktjm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cfskrwmw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jtdwbkkd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tjjhwkgt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qijjnhuk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2cxmzvxnx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qhbjzizi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jyluzyfs.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ertayzcz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lvoyvzdi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mxsyiecc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ndvfvxta.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zpkrjwob.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rmuclsjs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pinhzaab.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2roqunvui.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2unwgofsu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2izpwsbyz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qxenlabd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2scgmizzm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rzaztrua.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mlvqmpfi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2beakkxbf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2objkuccd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2majpoptt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2feyvaial.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zapoekgp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jhyzyqjr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ivwauzsu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2eqxrbtqo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kngaivja.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2giscwnte.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2hswakzuu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cbybmcpv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zfzfihab.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mfcpyqjs.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ykymbivm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2txytcifd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qhrtwnmw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pjajyapm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mlxgcnxb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tnnmvpqn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ececjdxs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yvpdlfhg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2txfjmqfq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qmlpkmep.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wbbxgflx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gukvtkaq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2temvjzlu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2snvihmch.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xrmdotnl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2efxylrkr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hvbuflpp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2velnlhvq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bnrmpfob.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2quelbvsd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2iqfyomdh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cmwxfasy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dzdgqgyh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2egdzuxob.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2aproqbbs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kthlsyqr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zznijsyx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bavfxebx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xkypbuph.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2teeiezjm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iyorzzwk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zrrbmxgc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xpzxofcy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vvfmoemz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hvjujyxv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2otfabfsg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rmnowagg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwaeminn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2iryhhmyl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pheynfsl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ssqbgepg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gravgunx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xevdemdo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xxflimqa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2sfcfnpda.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2futbkizk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2psdwhyxp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kjofqekw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ssyafwws.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ceofghxg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2syljwyfu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nmvhppfu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2raivjkqx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2equvdefo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tswhytsd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kpxsktlc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2nmskbzkp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sfblvwbh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fxdcvmce.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rokwnexw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rrptfvmu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2itsdcogv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dhyxdnjj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dzgbreti.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ghjaqgte.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ofqoyrth.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbzbatrt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ruvgcsvp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gxnbjqcz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kdblbypq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cfdlowxb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2sdapylyk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xuhrueaq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xsvnsiqx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ygvtacue.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkvbqcqc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rycrjial.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bkjoaeok.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wffmgiuo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mnojsxcm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ibpxjtio.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ojpivfiw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nrmvukpu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2igyyucov.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qdgedimr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aelagolu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hoosnpku.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2druhpjca.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pihjcgra.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ghghbnsg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhaqkjgz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2revkatde.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qcarjqzb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2eitkvlpn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2btbftbqo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qfgqvkiw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qvmufjkg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2npemanwx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fruuldbd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2iulcxuly.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uuolgkya.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bywcdaad.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2jzrxmvga.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jsqvekpk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xuktnwed.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pnqkckgw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xfglsdwa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wewfkref.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2renyvnke.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zqwsikdf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2uifpabcu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mywuzdwi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sitsuhfb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2iyqcvnkb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yzhwoazv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ccwqzllh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qbmuulhq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2lzcfppru.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kgfevorv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zvlrglwl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ymctfklz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2woubhzsk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2azhozxut.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ialzsitq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ahbxbemk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mrrpxfmc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fxkwrmlw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ehzwynci.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2doiudcnt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kgyvdhum.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kutqmkap.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sbhhzccg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2edipavfl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xqcrspqh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vywnskfb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rwsqphkh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qlmyntit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggpeaujl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2chqjmfae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmwembqw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2leajzryg.html


<!-- 参考信息 -->