代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajjyefkm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kivzstjw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gwqtzcju.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zrfqpmlw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nvbcxjlv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2bvfnmvbn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2iiintvdf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ewtkpejk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tpeiqinw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rrxstqkb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fmooeyne.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2btsqxzxm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zbvigerb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nplmalli.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2theazosi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2iobjnxej.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2divekicm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2juilfngt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2alvmxzot.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ujutluua.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lqpqgsjv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2oncnrnwm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lcpnzjib.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2cmhxyxbm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vefjrolc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hugdweuo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ejgmhxtb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rvumoudq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2suibxqri.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2yawhatfp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mvezojrs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2imhphfds.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gxwxlpgm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2isbnuleu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mctxlltn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oglxeqyo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eobcfpov.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qphqwgab.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2nkibcxzc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ntglvyag.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qkryespx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2scgepzvi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vxeyakbd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vfzqusyl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kaeovmhl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pjeckeip.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rkgnlpyn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fnvnygki.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ktitrmte.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2urmuwyby.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xixbcqra.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2juvapprv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qoejcivr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txxeyeuu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pbvhuwzf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2horkmyvy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2czbdnqup.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jjmhohlo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ntlkpkqc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2oabigyad.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bfoiuuty.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2igaouqvj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ofifwamb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2mdioafep.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2osyxmgkq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bwgvxurk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nwoacbfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgsemrcm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2phnwyset.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svvxbmcu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ddhvgugv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lquudwbo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gdeeywuw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xtkctmbl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2rrtlbmho.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ltxcmvna.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ucxqcmso.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qktqhcfo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2twhoumom.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2uneencqs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2awxsqsay.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2osemybyg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jjufqvlf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2enqftkok.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fstumjbs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2difdytka.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rhqeknqr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ofytjlmw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qfhjdiid.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lrqwucxz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hjvvvlhd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2peaimypf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rlfytnar.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2scxvcvow.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2drsgofan.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2aqjacblh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lgqvshky.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hcowbicv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lkvqzhlq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2fhkuvled.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2golimoof.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2laqxeruj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fgsnnlcs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yrltzxbo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hofaqjby.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ucmrrtyx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dmiknipt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gidoeplv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2emyoobnp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ghesasbp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wexiwjsc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cgzdoshk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2spihrhnq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qfalbgrj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cilwettm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wvomtkfk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lxyfxtuz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bdideoyc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tixztdis.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2okctawli.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ydzitsom.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hkxjwovl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2isckfqbx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vmccddrr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lygflpyg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cdgjdezf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2stnoapyv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2npmsikpj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vusuwymp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ocuvmzqd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2izixvatm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cgiyyyzu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kjfwxocr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dhdtique.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2emvjyweb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2flxitjnx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2thbvjvis.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nrjsftvd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wkdruhxm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2keffzfre.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ilpqwtiy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2szranzob.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tqanxdho.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kmcweehv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lsifjael.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rwtfwrfe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pxctdjnj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2onvwrssx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aeijjgpg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lvheqjfd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2slmshluu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2iiuaghmm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ipobwvve.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xyeleglo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fsclvqnw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xztdticr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vjfprvcc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ithzyphz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vrgaiaos.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mjqavpoe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ckcqbwvq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nnxvwqdg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2mgzcbtco.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2adxlmote.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hyuepfmy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hupdhiew.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2uduueclh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ijkhpriz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jryovdsw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vpwdxwxn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dquthalz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tpannfyi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ckwdqzpv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ihmsojzx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ngegtovu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fllhzndl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sgnqbibf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2manxccza.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hikhgiph.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tqrbtivf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cataxxjo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yeyfqwod.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cedzovue.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2naxezsau.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ffcthioi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qzytgebt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dnpydzfw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gdmyorqf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lqvksuke.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yfniuiwy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2widccnwu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pncmmkns.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cmnbydza.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2frutkxid.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hdblqftn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zjlaneyc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wqawsrax.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qamzyqhe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jdrknysx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ojcvqgpn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2luduulwm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dvgtmzqv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zpcugnnf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jcvettmk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vaatyljq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2alqkujll.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2adaveqqk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tbllkwjr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nvbkjilj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ifrsggoh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2eogpflmx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qyzfypgt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2pgteuijv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2baamohkt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jecquhdw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2oitdcljt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cmnjbvrk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2accnxunc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qmcbzvvi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2caqknnzp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2echaqdjn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dadalvsf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2sindfcvp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rtoelkzt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2apskypgz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bozwdipl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hixflwrs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2plczakem.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lpzdvlla.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ktnwfeck.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uuynfeuz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cmwxejtx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tmhobqya.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2azpnhkjd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cofqlvgu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2kkajgnag.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lsayalnd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2bltatczm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dgzkzrtn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cthaubrv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2cgepgamz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xthsfbkb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxwfdzlu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lgfxbkch.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ppxlfetp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tyeqvbje.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lcxnncfp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rfxvfzyi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2givqfcon.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ymzyemvw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wckxqblr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2czddrgla.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bsuvgwol.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2excrjlak.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwxqubh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wkibrcjs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmansdjk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2shjbgyky.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlgnihgk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2adavangp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qdlrlmnn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2zclvkdwe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbjcbeh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2cvkiqkvw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ajvipmup.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xjcvvpkm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2texauile.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ycsnqdgt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2anjfkkkn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ubrezmdl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vhdpksvd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fmvjskps.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sruysfom.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2skbcglhy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wlnkowqv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kasrbmkt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2armhucjr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tqvmfhte.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vwucqchg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jwehykqk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxjgiclx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2guewoisn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2iltnjafa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mmeyuwzx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nqjplcnd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vhzezojm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uqjetqqk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qqwsyqqz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jdwseocs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2annbdiry.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2luwsudyf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsswwoxw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2asbotnmq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2knitarei.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnflsdup.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qaqnhzet.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jvabuamx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hatursxk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2htjpiktb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qtxxmvcm.html


<!-- 参考信息 -->