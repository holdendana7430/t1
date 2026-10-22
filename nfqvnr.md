代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qbyzqzjx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hvjloavk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nuipavof.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ghnmpbon.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kzpivmmf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yuyphtuk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2einskyep.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wlrkajqu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dbhfkxlq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mlpgvarm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bjmukojm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jayvqfgo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2nqdnmuvq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tkfpagyz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2cchjlzbn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2txwoxkom.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xdrlxzgg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2monppgca.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nsalxknj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2aezuwzqw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hwljbpgk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tdpdmvba.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yyyltnih.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hctixbtv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yxbvngit.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktjgoerc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2eokihwpb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zdpfmppo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2csrwxsoq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jznnlyqm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lkvgqyws.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vfaiadfb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnbznqsw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ijrljukk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mkynmhbn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wmblghok.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vexxscbe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2njsxfuxx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wlfietnj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fgjhicqw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2mizflsdo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2divwwqay.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bjkorhft.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2pnabfdie.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ybbzmfpv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yefhrqkt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hxhjgour.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jroqilso.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pljjaxfk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ahmzntry.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2futhvjzc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2owfzwzhe.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ouffllsv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hkhryvry.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tyyioxnn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2dbvmglvc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2aioslhlr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lwlllamx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlmoudpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iflhceiv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2btfevrwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svsskclk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wsgazbfx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xonoqkky.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qxtpufnj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lqvcnrmg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fkfmzeyg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qmfwrqva.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ohazhous.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hlcsxgza.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2svgditne.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ttuumohy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ntwlqazg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lqsuxlax.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cxzxfhyg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yxpvblbv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ccvzrhme.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vfbedfni.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uwfrdxoe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eqsporoa.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pvmezxjr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2abchrpel.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lvwzufpk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rirovwea.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qxkrzqqu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iayupogk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qwivlcrm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2noygbdnc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lrirmrus.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iecloknh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aefuzlfd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ungbuxqv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yhntmefh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iwbyeyjf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2khwvugbv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2pakmtajq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2agrolriz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ujgtjhpi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ubsiejws.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cvabkqtl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qtxsewyy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hlxhekmj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mwfnrugn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cxqjdekl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tkgdakzq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xnwoapiz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2baketybq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2boszqmzo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fftljxya.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jqnauqrx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2phawpbvy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qsufwnuv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gqyrdacf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2layfhrwo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2iwuovznh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jvzyicqn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2jocvejxg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lqswozfn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kltwozki.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tbijhopr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jtlhzswv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oxeysrbi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2tmmwtsnl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2bqtfuhba.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cnqwnzjo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vfwknxqz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2cqclwoho.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2iupooapw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gxqhdbuz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lqxhxnxr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qejkuvtp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bbhrxouh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gufsmmgi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2arxcvmwh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2peaetcbp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ddjdirsd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wmqkmbsg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hghpbvxl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2fjofhsuy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ejtwztak.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bnfumryb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dsfomoxc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fntgbgao.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ihdrsboa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2aludxhtb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2viopxifr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tmutefsz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2isxydkxc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hyyzneek.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2etzovevj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2efghhehu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ebkchfhs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bldpjhyo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tdznvldh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fcybgjjf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nelqgksj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qgeaqwnc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wnwopsuk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xrlnqqjd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rriqsswi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vwmmfsdn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2crvgnxtb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jkxbgzuz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2czbwcmyj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hywlspzn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2husxskgl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2idmrglfi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2anozwyvp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sdxeqaij.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2yusdxpki.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zafbwhxt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vstclytj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zuheihoi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qrbepylo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rjuldxzw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gotokjwd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2eyqwvjcn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hnzwepxn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nxbvmmlc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ftktopzi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ijolnhvj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hvldlhgb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbxbacuo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vrcdjctk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2siqhbxvr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2slsgdumc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gatiuktu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jhvuoopo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cbcrbpcm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ajksoazo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2saozhlxy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pkvsrnsi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wkwbfjbs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cwgiptdf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bzbbgmyj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2fgizsgki.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2buflvypw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ksqpsjaz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwchfhph.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fmqcjkue.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pypybzsl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yxsjavkq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vvwxvhlj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2uagwoyig.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2eketcfzu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2evmbikrq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fwoayekn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jnfomymb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2udumvvvy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kitanear.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2khwdwnkh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xmxoesni.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zycyjosz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nlaqfwvu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tmdzbboa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mrqxccmo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cgjdtvok.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2kdozbyzq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yivdaenw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mitrkjur.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rbtdwsoe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xdqwuirc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yfskcdxm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wufsswzi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2boqfbzbd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2aftkzoxm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pseodtda.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2akvrevrr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2idsodvwe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2mtunwzrr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ajlkealb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2smixzsdb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2obymqbqe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yfxyfggs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xjecnslm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gkrstwsg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2brvsxxao.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ncbsmxaa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nfhgtkmj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jhyghtup.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lvlbezsh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mjfbguyu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2xkrrvlrz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yxnwzzwo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ugcujlwu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oxdpkbzu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xzhvlchg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kksyfnkm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vvauazys.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2svufstak.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfraunge.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xyewvnyc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rzwylaof.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fpjbirxs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aylihcvx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xghuppkw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ofdhorwc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ueexmffa.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dlzpenib.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wpkxlenf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dhnkrazu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2thjohnft.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fqlbcotj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2conmxius.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uyvsywal.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dqnrfbzc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fbcsnhgj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2akuibzgd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tdjpflwc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zslhkceo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zxmhgubz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kktqandi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbixsuoh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wqslnjjr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ngzbwbwt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tuvyzlud.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eytnvgwn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2aajiiepj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mifzbzuo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ooflcpip.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nitkwsyg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jzokcdiv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2dtiwiilz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekkfhosx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pyuizfse.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwbpmgvu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vwjuozun.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2elqfxnew.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wjpewgep.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bdijbylo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qtkwdtav.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mmefcdem.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qxdbcqlk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bbfgposf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mccdntmu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuqcvor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olcoowmv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2myxoskqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmaoicnj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rxwkbqqr.html


<!-- 参考信息 -->