代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3togxqzup.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gnlfdyjk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3avwgywov.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3uvlzzzwy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mrtvhmul.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xmlaurpk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3iygmxbbi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xhxrydzv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ypixwysh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3letxoqsh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hlsezdcq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3orlwzawg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3pgspjela.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3msyhaddv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3kmmvhybm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dwbkxnas.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3edtwhlxj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qiriwdzz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ouolqmab.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3glcsjttm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wxwoxsid.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3mhneicwc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3obihmnzr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vpqfqlsq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ohufupel.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3srwlvkaq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rykdvefp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3szsknvei.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciqfjsfy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3semvublf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dnhjbnjj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gutaiheu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hboevsin.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pisqtdkj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cagncuwk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gvzmyrsk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3spkushao.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wfufqhnx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pkawkhhr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nbysdmzv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3kndvxqgb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3drcyxgwf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3agtywcaa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nzyctkff.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlwpcdpc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3sxfqeart.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pdikgioi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bauywehm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fphlewex.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3eflbmloz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fmjhtjpe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xvshzyvn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dxirzaps.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ofqjjakc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qqmtfuwd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjhlwyef.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lurrcphv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdjhisem.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zjtvxvre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgfenadf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kgwermey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydnbatjk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rzmnsdqs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dctjvupf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3phnhgbfi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mmqeqkud.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bicpesru.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3moqxgrkf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ixfymktf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3xcbubtww.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kqmqmhes.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3whksjlix.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mnvwueru.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rhrfchfp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jwalmssw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ayjfidwi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wmsjpfvb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3twsfmiml.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nenhjbxi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3drvdkvok.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3oqoskvwu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bsxhqxlx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dkrfkrpf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bctrjvfy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jdbpynhk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tublmltu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxlgmtd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vsnjtfgm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kfzsxoxn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tgffswab.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3awyugfan.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nbrnvfck.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ejdriijv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bepcgtns.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hnqadtkg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kdfbfvnl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lnyiguzm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3texkndxb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3carhvaok.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kztpijad.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uadulsnl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ufwiwdrb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wdixnjjx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lrzkoiyh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tptzgibl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uxfdwdgp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cgpqyvyy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jmpomzxn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eujhbueg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nvneqair.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kikwjgcu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kntexwbu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jhjfzhel.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dcpicwzo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3miqlinkl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vhyyygpg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wyfobwca.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ebditkwz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rxlrmizc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3usdfdecf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3slzlkfkm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mvbzallx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tjheonqm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jhtxmthr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ldxembwd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3komjvzuv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gswxsttj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3tsydxzwz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3pgonrbnz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hxyxynsm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qorekpfz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3cfbvgfyu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wtphtnsh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3euegrbiq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ldfiquab.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mmustfgq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nveovrlw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mdxxxhym.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3oskeqxbd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gnrhxzya.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qshfqqqh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fblusmxz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yulywoxe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ivykuuvg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lacmagak.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zleflfte.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qnsuzhlv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wkdsvokc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xjaqtgcs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fmfrxzjm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mpduuxam.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lsojgdsd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fvlbyxul.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mygypdub.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dtjjhmgg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tvmwyrfq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vwoaermx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tmghmtlf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iqfexuet.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pefljvhk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sfhqzeym.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pwkjmgrb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dmkfbzdu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cvshimlj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bxiufksx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rmdihfnf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xxjljofu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3whlzinbx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmiovalr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gimluboq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qlaaujhx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yqarzqnn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xvotzygd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hnbmemqd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zuksxall.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3znjjjlbl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3panrvibj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3anvcnpge.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wbwbcsvz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hzfgmrqh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3leacxvct.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmpjyoop.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cydhsizj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfedqgkj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fgsmvbvn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xxxxyhwe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yjuoemwl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gkmwlgiu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ahjrwqkb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zqdojezl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vpupaauz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dnsiccsp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cfuwctur.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3hhlhsifj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3sadgyxgz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lrnomanm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wvshpfru.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3efmzeutf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ybcsbzle.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zltmkypn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ttfebfga.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lpxjbepl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3sbhwfesj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hlvtuqap.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tlodtcbw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fvcbpfby.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ippddxsd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xlpejssd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wctsvoyl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3eqbnydbb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xxzeojbo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jjeapbgq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucppxgdu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vkczkari.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3gvvhckgf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3iistycsz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vewtanqy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kbcofhpy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3usiqyflw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tyuzhkcv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cpnjhrhh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vbmlqwxx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bjuchaeu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xwdbnwzl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xpjlfhko.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ycmxrmeg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gfhcqhtr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3syrhoshk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mqcwexok.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nwtkybce.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zvlcakpz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3sgxejsmr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3cfngfefh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mfcacnze.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3noogvnak.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kpsrjfdb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kaivvuki.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3oghrybjx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uafugjhp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rrxrnjwf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3udoetabf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wwkcjjno.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hjippanf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3iiqzfrkl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cwhqnwsd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wyrgqplf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fmdenvpf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uicouivy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yyiweofl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkjktdqw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgfbvrml.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bwpauoek.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3cdjyjxrl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3szhhudef.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bvpaabph.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jlxtnrdg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3lmfqjzam.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3irbcmlho.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3poopbsva.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3skthgdod.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3cjsiioqw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqxobhp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3yzdzvwow.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xwfxjmdq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvcomgi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3puecwgxg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hfwrrsfs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hhnpzedu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yvhxnfml.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ivqzhitf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jpurvinj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3obxtgiuw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3aponsbkd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tduinmnd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ggsociif.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ykyyiglf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fvttpsjv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yijrbvrj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jtfsfwdi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3araxtpvk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vwpmyion.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ndgixdmp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3zasrshzs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bokadkhq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rvosxdcy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kaydtvls.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hkdhlnoi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqfzrjkx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qcutvyet.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uiwyitwq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zamunqug.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cewjeyrr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bmvabvvv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ummochgp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bmcrjoxs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wajoecjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlyxrwbq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jyysbvjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqczvcmg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3txhzclzp.html


<!-- 参考信息 -->