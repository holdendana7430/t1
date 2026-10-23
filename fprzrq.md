代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xwinfspf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3nguqvlqp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3zhmiezze.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jkcusqbn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3udemyhjc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dxlcyojb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xkfunytp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lxqwboku.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cdjyxifn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zhlgikey.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lquzttqv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nmbphlbz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tdduszay.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hgzrluzl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kycdzavv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3osmuvult.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3okbbdmvr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vxfysojo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lqsvwpku.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tndvsafb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3oxnabhjp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dyxvonsg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oeiphexb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3suksifsj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vdobrsvq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3npltnlym.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sxazgwxm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pvcltgxm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3najkdfuk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ocjwabgh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cwholidv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xbmtvjvt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vlyzgkwx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3guneuwdo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3fuoajyjy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3acjirzpd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3loltrvgo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dnejottw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dprsjdjx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hejozqpt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3syofpcrh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qbnvestg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qgxuwvqh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wnakxxha.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3oxkzjeym.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3guxaroav.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rjksaznx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kfdmmmon.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbsfcyoc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbuvqxsz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nbxnxfwv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ngkiytzh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ksftmfbx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rlwqzrde.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lqwsgphy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wacnusdp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwlsch.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3inixqemx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tmgprpku.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yynkadvs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3drcfiqgu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3flsflsdv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oktyqjph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzewzyec.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zhzgrzqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqqvdtnz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sjxpnqrh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3aaormrxo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pwvuomwn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qorwblbm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3cxclvpua.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mjgaymbt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fxbcdoxm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3oohkjpqc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ainirmdf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ashirllg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3seddtanu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pohqjzob.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uwrgnhsi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ihryxsgi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ucuutile.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vhmecxje.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ijgyrjzq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qnnquahw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3zazsxsgm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yqerspvg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fydgoaqx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kmtkvhxd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hskyredh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3foiofmee.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3agaezlvf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3eaxiueci.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hrblueqa.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bcrtsxxc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vpbhvarm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3oapmrebq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3uomfnvwv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ebymwujs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wgrqyifr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zbpfpqsy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3idevymgh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwbcizxd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gbhupfqc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bpgkodch.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ulhiwezj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ijkhxipe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vnyzpicr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lomouvrr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zganabby.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pxsjgbwa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zbgdevvw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kdizkmxv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zccwbmuq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hfwjkhda.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gwhybabk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lhdeuosx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lkkmmwqf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwhwksxv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tdykbruw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3lagvyhee.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3myiapfwf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3woszjexw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pkdigxmv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bwfptadd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wgkhszbg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vfalncsc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rxwlmthq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tmeftffs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cdxhgsiv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3fyinaphh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xxikuzrw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rfveksne.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3yggtrbvu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kwmrkgfy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jefxwbpm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ywxyjyhe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dozonkds.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aifzbpll.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jahxuebh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zuyjmdnw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3dxlwsgwa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3yeltvbyk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3lmqnrguc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gldqcafh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzcdsapz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3csxxffeg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3bazlgmcf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3txlnamfv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3inodtcaw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3huzojcsq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3znmfgejd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tyqetpby.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fxxycons.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3onnmfuik.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jsjkvxex.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qlahtdfx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nyhvdsnh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pkxhdpzd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3sjotufkz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3civovjrj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3quugxtqv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3drymbqja.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zzkyzndc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ngfzmtgu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hqadqdqz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kesxrzrn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3sgswyufv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ymgpxcnk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qookdrus.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ciwwueyu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tmkhjhco.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3endlsoaa.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvhfssnj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jugmgfag.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3aeipxziu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3agkbzyju.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3inucmzue.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iynancql.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gyjeuian.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hzujlyoo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jjnncwcu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jssjywjz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dioogada.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3kqfalvav.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dyrjhwxa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kcczcbvs.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhjvdqr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yqqfhdoh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3epdlmbbf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fwqhtydm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vurotatd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ehentaic.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3yrewwsnl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sqhfevax.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwxbqeey.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hkpoqfcs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3akjztfdu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ehbdguti.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cdstkcnt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hlvmftgz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vynmwdti.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pzplqxuo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qdifqowi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mlttzszo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bqtdehwi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qmhynmnz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3yclrrmpp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fqlpttjz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3iabvuuce.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kqruixok.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3oxnevhpd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wtclzhfj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rpnhepov.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kvfnzcvr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3picefjbl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yiblqibz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nyjrckur.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3npxbpodi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ffbanwyj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ugkmaouc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3erwohawh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qgqfyupe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvamofh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zhlcpixj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3kybgmxrt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3isuaipyy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bbiarxji.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ggykbkms.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ivkpgsyb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gravbvai.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qpfqumoz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3myztdfxn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mdufiogp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gszyllvn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3klrgewpg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rdhfewab.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fjgzufma.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pvqpdate.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ictvxqum.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rdnbklhs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dvntqhbm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nqcqelaq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vtmanjce.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3dbhywmnc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3iizajknv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jzndqsvd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3mnysjrox.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yywdxlgq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3btphhvbg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ywjvetpk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fozpbmqi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nvyozjdd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljplvlvo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dbylduiu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdydoobo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3srsjwlfe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mdlvdvua.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hbvicrst.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmkowgig.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zcpibtgm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ymrtlssx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpcyvwb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kdvrnlxa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bfnfzsrd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kdsnhccz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ojrlspqz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3foyuiprv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hqlszinz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wuznwzqy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bkrfgxvx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jcdburat.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rplynxra.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwfssblc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tzoxxonr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dxyezbuh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xndmnmzx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtzvlne.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qwctkgdt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wzugzsph.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pgzifwoc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jgwsplfa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fadbsgfm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ijkhqlxr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3tkhuxghc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3emrgxpah.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3svpnugma.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bxkpafhx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fcybffmz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cmmfilkf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csjoivht.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3erhfzvfg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3brnwoabk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3afoqijth.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uyzuqgrw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vtfucnye.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3piaruzot.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zxcsyavg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bfttxgrl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mvijmnjq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3unqvkemm.html


<!-- 参考信息 -->