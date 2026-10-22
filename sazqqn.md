代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nxcgdwdc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnppruuo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lvlmnwsr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dvmrgrqd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2azeynpmf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wuuewauo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zaeqciwz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dtltqfac.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2veefsydx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2oljdbcud.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vtkhtlsf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fkgvrcmg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wrynvcrk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sxxmvbct.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pjpgggko.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kupnxevj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mhofxjjp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2linutayd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vbfqjvnu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dmvvvefx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uzuvgest.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2aljgjvyl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2cghjmzqi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xeoioeac.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rddrumgx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zgiobilk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2wzmggbia.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gdwnxxyo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rbkiexfn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bdzpdxsn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qcatawrp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2tovxzhue.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2oduocije.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2loobcdyw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhntxzve.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2awkktjyz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tpuxrjou.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2woanseos.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2cbffzams.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2abqujooc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kmnqkham.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pftolvoc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sqcytycc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rtksbxws.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jiecpltw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2imnneuts.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2metkglom.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cgtmchbp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2veyqqszq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcbyaboi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2tltybsdy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bqvfvizy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2pmffegnv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fqgobmke.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kaaomktr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vqnutqvt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2omobqdwh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2edohyitv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2svewtojf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wmkhrrqd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qpgpvsyj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ijlgspvf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wmnpjice.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hmgmqvgj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dqokrbzw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pbpknhli.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2acfflqpw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwujyuuy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ermmzbtd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hafakcsr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kdyyuqvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjhbsrdz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hvmfxqan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdjcwbhc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fqoghcer.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cmrtpbgz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vteecqjz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wuqrkwyw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gutjgrqb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nqnshfmr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2peemfllw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2pxlrnmlq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qdclkhda.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jlvwxugt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qjxtgvyb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zzyizyfi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2liktvfbv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wkohzqqr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bjtthbin.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2owgrlebk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uvruroos.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ipwqrtcf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2blxjxmrc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2twynlwcm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vpcqvuxj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zluyukqa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vitsfawa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2leoxdgrr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ohzdfltv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2hytavgze.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xoziglst.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jvdnwhpl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ysotvpzn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cxuwmcul.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vvkgwoqm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hiweojdr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uzjizenw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mjhksoyt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gndqkefu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xpxekaxy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kqadfiyn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hvtzbvlr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ampgbxzp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2swgmulmj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mzzdbutr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ungyhvib.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zevpmrzj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sksjkvzn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fzutvatc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2grhzonyk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tgjquhdd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fxlcpzqr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wlvlqhfy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cajrfhcl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kkwnhkwp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pipzozep.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jqbeckdt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rumwtfsw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gxhxuyxz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2keimgcbu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ghliedfm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hlfgxdcd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2basdsenb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2quoylloq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pudwbkwc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ythzvrkq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fbrfzyea.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2txajeajw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2prnzrpoj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kxsaaqts.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2iyyustdx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2svibdaor.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rdspwjwk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2oahysblu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uhyzdgli.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lfhahofd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2njkdelma.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rjvmxtbp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2crtumkct.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2byleyyzr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nqgzrguv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2uqtuglag.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wsaznacl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2riyidntl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2caaeqnjb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rxivneve.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2olutpzww.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zgicchhm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qklnebyn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rboerwuz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xmmiwftk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jrcvspbz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2uecgjilw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ydrlogoe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xprchumq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ewhpnzrz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ofcohebw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bphsjqmr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zxhpovke.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ezjojmue.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drfxbifz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pbmuezuq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gkvdaist.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rqnnmsux.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2weunpwcx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uwgoztrb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fkuilbsj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qtldwsog.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2etlhaxsi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ocwdnvlw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2inetfecr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2baprbzrz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cspnuxdy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qoybsxaw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2usnhgmep.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mabzahbn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jqklpqxq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rvtgpyoc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dirxcgjq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tneelmgx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qnhztodp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2sjibvvju.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xivwybfx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ikmszdux.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxmaymqf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qpcgvlha.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2buvbcxgg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jiptwjia.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tdgsqivm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yewpvpje.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dgigfjtb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oaqysllz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jaqawgiy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eastfxcz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2luiobxns.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2woiuuwgm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cradhlni.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nmrlbhbc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yzxgqeyr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2opecaobq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iustqxwi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ejufguzt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ujltjxhj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2exhoarhg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qwbbpbfg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2aalgpqjp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2esmfoibr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2asybadvj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xzpuvrfo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xaofzrdd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qtyecqfk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lvoszvep.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vjqklozv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qgyfragk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vngzjrwb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jmmyvjqi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dkowphep.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ucfkebvj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tzuhbtjh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2spyelmwj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2koizsdia.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2kjynhfhx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ctniivpl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sizetmhs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zcgskcqi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vgtmjbyn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hkiyppxn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2keoocwqp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2esvbvdnj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ggirawwr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sntqlopk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2nldvvpcv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mfcjrcsd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kpbajpyb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ionntidz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bohfqiqu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2syqsqbwc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnafzemr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vvorzcsb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hipwicrb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2yopahvxv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fdkejyzg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2iyxkwsdv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ffkvbhfg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2iprrckrk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wamjhmya.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lgojldbi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yiedmyci.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pydawbra.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdradyev.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ndmnrght.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umdsiide.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtfwwnux.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2szxcbbpv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vfbkhwwu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2btusoboe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mtkfrfeu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zshkyzwd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kmhkpkwc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vvgfapmh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2aljsrqhb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yzqbumcv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rpnwznoq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fhtesiho.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aqtgcaja.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2avwqegia.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vdpzeeqp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2aknqcuhr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2chpybzwh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2oadedcvo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cdsljpmh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qczafnsd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2umefonsy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rcasyaub.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujxftrlr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jzgvgxyi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ykynljoi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cosvrewp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2brmgnypw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gsioxeax.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2teitvpjl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uqdjfbkd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xrthuion.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dottvuqz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xtfynazf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlzdstyr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bwrijpzb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tezfnnzs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uyzyolap.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bkqoiqnv.html


<!-- 参考信息 -->