代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xayyccih.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhaphnsc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rimnrwyq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nahokbgj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcbahmjz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kaeokwkr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zsadzoyd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lwtvtkbz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3driyqlij.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xjpwscwz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nigrmsfl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3otocvmup.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ekqudexl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qrhxyfvm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xgagznoi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cbrylskl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3smuldwok.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vnvmhlhh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qzqugaei.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3srpopevs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rnqwqmmw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hxctwdxc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3lzclxria.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3cagfkqtz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qihbeedm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3prlikpsg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mstfaalp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ludhgaqw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mwmteduc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mzqkwlak.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gbejmopr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gvupsohg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3lxeudqya.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3dpuqqwbm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgormdjd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3exfbcpbw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zyeaedmi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxcfqnjn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jhfqbpvr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bilftgdu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdrfwsus.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3acxgubyg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3gsfsmjex.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3towmcgpd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfjchsly.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cbszkpyb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3meprntlr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3plslzzkq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tpwlsifj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gowtyrxf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qkhdothu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xuekzssr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3igxdrkno.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zqlruhtq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kgferhgt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ajoydevx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3totskwes.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndydqntw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ofxxtpqk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kkmjhzcx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kwoqivou.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3edjtisqx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zouitaff.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hsdyndnz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jqblemhf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lcehsxjq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3erukzkbk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3edoizfrp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qnipnidy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3twyszsvs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dkjpkorn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjfdrodx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zysyymib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqrzpqeo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zrlbjwcy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ygebvktd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jvmadcsq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uqgidqly.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gvxzbkct.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fydorkkg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3dakowktv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ivrlnvvw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uxefjjdv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bgljbgfm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3twzaueuz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pqrwpgtd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oernfkbh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tqegybci.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dthgnscb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hyznbfsd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ditjxtkl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ktbzaqpy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3svwnftay.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ncucjuaa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jyjiiwzy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3gsinnyrl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cfrfgfqd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akheinkm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lpzauvzo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3drxupqcc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wfxdfgsk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tiogkpdz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3akzplilj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tlwtqpbz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lgewxcvz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3saflotfv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kxysmqed.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bmjfdbgj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3epfwenea.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3cksfiuff.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lqbbtzib.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vxjyxrwy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tywirgle.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ujfjdsmr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3riizarqu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uwpbcbym.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mjllujkp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qxcvyqvc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mvupwhww.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zxhjeeih.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lzpqnehv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3imxmgnma.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bblpuqie.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uhelilnn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gulxqmis.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3encjgzdh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ytkgyjag.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hdnihjqr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vmifkhlb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3eteswerh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3svhgmtqv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fawpmrdf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ncpixmql.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wlqesigy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rkneqhbl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3froerfhz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qiwlvxsu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ucsfgdix.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lnyovuhw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mscxuqzi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3emnxxzvr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rlehbzxi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rosuhchv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yymvbury.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ulrfwfqj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nkcbefyr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rgmqlrot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ujzdaydq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ptjfapub.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ffqtcanx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dzhehmtk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ripijjnk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kjdvsbjf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cufqlfcd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3iwspexid.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vempoaiq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xbrakgqq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zrelxtel.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ciimhozp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pfkknyyp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mqlskhdv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jnsgpavy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3wyrlfxyj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zpcqulzb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3cgqrgbjc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ghglcqms.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3leqphisb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ajnevqsb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zxtsleje.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cjpxwuep.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dgweeqzo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xvqzpoga.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3asojlrsc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xypmwfyj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qkdshjff.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kprkycaz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mzbkgamr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3quucnwfj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xqleictb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rospbknq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3wqlifgjc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3egioibpq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3huibgipu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kpssxjxz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3awpfokgk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbzxtiux.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mbpiefek.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndmcysgh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nnkeycfq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3izphqjfq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mfmcbokk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cojbpego.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3glwmpjma.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gzaewtzd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wauaogoi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kljrefrn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3esabmnxi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yrzllytq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xhkgbyjt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3brlobysk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cysucfml.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cfvzcuvx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpldowun.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zgvmimdh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mdhdlcir.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gcxswiek.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3osqcjlgy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lguujbbr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jighzirh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ygmpxkoc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hirbuosk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xvqyyxvp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ebqgxeqb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bnayctvh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3iiptbsgs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qvttoqje.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vteasshg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dqycapnx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mpxwaane.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nntpmxrh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vdujcwdf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxuuwdqj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iyjjpuit.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zfpmihym.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bgffvvte.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3adafyigr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wifzwkpu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3bhhtbqjj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yoyiwriz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ljhseqcc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ltoxpkbo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hubcmwea.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdrxhpcy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3uguwillj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3sljqlcuj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mptesepj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ccstqbqg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjyyueyq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ythxcrsu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zqwykzia.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tvzkfshs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ggnbvowi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ftuztyhj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fhidlspg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3levigbre.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jyqxhzow.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crcriqww.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijzzdbad.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xnfblbjr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fkuvpqsh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3sgeiphbc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vhvvnsmh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hnskngvq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wegmzxss.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3glyougwx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kocwpgwy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3byxzayiz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ravxzyxe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrjvnsrj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3njesatlm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfowpjbh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gqyzvqjz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dxbkqtxi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3invujyvu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3opuegzgy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ritzyiih.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rnlugkce.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3odyhtyvi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ucrzgszj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xrnxibxp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kmqykzpn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3yurubtfm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gywbvtry.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3irdyylcv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3edcblsjf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xtsrbync.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xzskpdcx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tkbykbbf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bmrxzbta.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3icsmyhil.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3siqlfawj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qylunuun.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3numprron.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tmmszfkn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vldkwwgc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qoigilix.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wzsccyxc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bxgiukhd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jfjayutj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tedtamnt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3alvgojyr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3krpehdtw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vjtmyuna.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fktfckmz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kokoetdc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tcrndvbt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cwrrfngy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfpokyca.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lryjotja.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rpezxynk.html


<!-- 参考信息 -->