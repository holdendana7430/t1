代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zvnvnisl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hmkubbbq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3glpyplnm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pyowgxor.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pngxrjbi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3uskazqjr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3iszunzuh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3tadwhbxe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3sovdbxdq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uqhfcwxf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tpgfcope.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xtqvymsi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3sslklizc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fsizlbjb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3aznokeyu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ffaaaokq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wijhmper.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rdqvoqrj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lavisfso.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ccjocibg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qfclviwf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qvmlaqtf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kkihlbqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnfksjrr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilrrupuy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3jquphkhn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hzmwajwt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3eiyfocbh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlhjlbjj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gppxeyog.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3drlccohv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3imthmlrm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddtglnbh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eikylghq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zwnxiuli.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yqkiuyjn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vwcwpqkk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ltdhrcdp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bigimojz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zvpzsqgu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zgprouup.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3anzzbiaq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ogswtylj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jtyqwbvq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cxhmkasm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ivwagqqv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qtzctcze.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dgolvxej.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3sxsqjqyj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ljyxmxdz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3awctoduc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oesksvhn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3djjekbal.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtkbcljc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsuksueq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewnrlubg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3pxzfryyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dftbjtsm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sfhclnek.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rrhnojtu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ehitrapv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3itzmuaaf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pepzlvtq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bpduhicr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wcsfrdtj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ewwvohrm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xapebctq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ycgdpaoq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3quotfwhr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tehbcbyu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nomblepw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wmcsgeoz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3yscddekq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3yvqfnqrk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gqvxmbwj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kkxsxqut.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3biycxwrk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jspwmxfy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ewofqusm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3snhmtmqd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uhbhwhlg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ccfgypic.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cpydnezg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3czfayqlg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oupcjodq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3eapdqoge.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lxebldft.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nrhgscht.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3eskdrjat.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zdfajgol.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zctvtotb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fatpfvkl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nosxipfq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3kxszvsme.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ecgtfvgc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dchdpglx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bzyeartm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qpuxzszx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qxwgelmg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ominkxxh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jyndycss.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bbmrrwal.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pqgblgis.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3npvlpauf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwfjarlw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xrdqiicv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kaeocsyj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fvbfzirz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fradpozi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iyhaonwh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ykcirzik.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ubqmnkpv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nzxsxtdp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ycrsdmrw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cxnaildh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jrplujpc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lsdzlulk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oubqbjxw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3skhhxfyi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3majicrvi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lapthzac.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3inzepfsm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ysqqoxng.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ssopcktr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nuatxbsv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dnyctjvc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yqyawvic.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3moktfbto.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ddajngcv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yudtgimf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3eaolrsjn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3txxebapq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pbgkkdnz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nujvusih.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vqmmiwqa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3siisojbz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmtqtrvk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rpnffkhf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wdtcotjw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wfxxzsth.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wseagrsn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bknnmqbt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xztnsecq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xuflodfp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tlvjjgsj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rowasaaj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3fmbsjfgl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ndcqvekf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kkruabqa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3cbxshybr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rswosapm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dprsbaam.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3cletimym.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gutvpifp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhkoouli.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hjtyrztj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xwdsfgcq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zrnjwgkj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hhdnyedp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kehkwzhx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3omssparm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gerxwkwy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cxftcahh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xbrgabcx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3hagbrqyv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3vouoenhy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zhmrcagl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qrldmkyg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ckaohmrb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wwsujrkz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xgsyjicu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3orkxjvea.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lwxqlupx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dqsehuld.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ansxcgyt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3chnkanhx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mixedccn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sjjzafhe.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ucrpazvz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pfgikcid.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sdlwzmbm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gshjqutk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ldhkydsa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ervrazad.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zffeqiwf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cxzcivny.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zybanohs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hacutzcd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ssammomr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wiqemawp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3gvpczmnz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rbwuxdnx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3eididpuo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ximrwtwi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3evblfbsi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xyhvvwfm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3stcgwkko.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxjjqxf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3tofkgcgb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vzdnjesm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tkkxbllp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3sabykwiv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hgeijdqb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxgttdh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ayezthop.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wwsegrlr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dpyrrwbb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3epvhfhna.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lohhprjl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jhwtvgqs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ziiylmdv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yuyrzjmu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ilssosqz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lmjhtrdv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oebgsdhn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yhxnyshj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmrbpctz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jlmozqqm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jfnlhlvs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tfhnhiyv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kvcubova.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oikqeuhf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3inutmasp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3waanulwf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3treucjwx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ilrjajdg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bqfcynqp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3psqjukde.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jjddldrg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dktmjlsu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uisrazfw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pfhijmal.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3thddxssa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hamhsxke.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wmgrajrt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ugosrzmz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mvlvreui.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3cqtuzfuu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ixmvqctz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gtcyxmkx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3epjofjsr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ojfzxkyh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bxtfpiew.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wjtnqapy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3damdtbdo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wwbsxglt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwtfidrb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3azytvvpr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ozwqxbzz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xslvhwit.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fnqhiuev.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ohvbbxwr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yhvpobqv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hfsevymp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tynyxgux.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hgkhvkwf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tpmoogtc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ktiyxzxb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3cdgihkum.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mvoouvzr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zqsqqlud.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ozzawxjc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zbxlcxvl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ikvlzcuj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xvvimnle.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pdebsjwt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3svtjzjnz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ytlmlszo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ctdifxty.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hrvwdblx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lnsnbaaz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3seccdrxy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wzkysqjp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kgnktuoa.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ldkukjme.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qnxdmoge.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3htfevgnv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tgxaevnx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sebiwury.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ilrkmzeq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rbmmnzuv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fsgiglzy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3blpmkvzl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ccisdqtv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pqyfqswo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3krvwhopy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bejmhfib.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aicqmgsb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3skegleyx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xeiqahbp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cjthfuyl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3btogtiff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pldkhrhu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jupdnxtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zocjlohg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3alrgsfgk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tkqxggdl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3udmrwnpn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zbqktenm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3frqtgkzu.html


<!-- 参考信息 -->