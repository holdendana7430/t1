代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mpurnwnf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3upjofssz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3icvvlgrf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ltpvdxfh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3fuaczovg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3bgxavtzj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wdukipbr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eiirdgio.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jnskotut.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sjeirsug.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uszhmjkh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3djzomsbe.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bcexwjpm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zdsqmjmh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zwblhfkh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dtxqbfxx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wbtkixag.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hjsqmmhv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jeakjzoi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dieeunso.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uvgjvhxe.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qmpkpkgy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3sixniklm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ruqnvopk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3czebobti.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mehdtwpr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pkqvzjtz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jdypctkn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3yccrtuuq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dkivqwbj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nstbjhjh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nhxaypdu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3oftrtsfx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jpdgzatr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3iykhcalu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kmfpgfws.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tqcnmtuv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3kagdkgeg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xilidzbl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nszrfklp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbwprnbs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3eunfynss.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mknkahbj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zghtqfqf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3acnrrokr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ripjoxfk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rmgdvtnr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3awpuprza.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3oaxcwzvn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3atlovpgv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3imqlxovq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dyoosmkr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gaffubrs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkuuekts.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sxccpmwr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sxclcrrc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tpylcihk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ytlvslrk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tgkehnio.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3joukoyeh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3oxgkjkom.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3pxpxrzqs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ledpelaq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ygwatjcm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xflkyxcj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iuujfpry.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpkillvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsadpvnx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3brhbdgpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkgmjwzf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sobymdfg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3twptyaob.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3iuvdhuyc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hzoirnir.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lgmkrrcw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cvjzaqdu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3itbgblfk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oxbgmpwj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3orqxdait.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qnpkwxcr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qzdpvcoo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jmuknfye.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmvpikuw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3smvhosxv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3luqsbrni.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ifgmpcsv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3avqcwzto.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3narjdbvw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tbxptkss.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wlwamwgg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ifxhbang.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wijvefwo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3atdbfzbv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wuhetgvg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pvurzhnf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dziqcsiv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3teslcwzs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rwxmwjyi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lbybdexq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qvittbgx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zrtpekrk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tizagtyk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pzpjzxqx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3toecltov.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmtbceax.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3aiiobebe.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xpngiktw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3odmxiljw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gxfstjsf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3atkwchoa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nqpmscfu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vpyjkprs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jfabcfca.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ixqgcvsk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hhptwpxp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3buctuygq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ndbcuinv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ryrjotjm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rwtxpdfx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qgnhsqpw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3twzthoef.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3afpjomdu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rtzblgxu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vzcxefof.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hjlitwwe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3inusvvbr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ukdlikki.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3smzxhuik.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jyczczij.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ysaszisn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fnyhxsqa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yfpmszxi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eykexmpy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3sefhgyrm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zzwnlffg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3esrqzyxx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3oqjezeyk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3iunluffa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tqzkocou.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3bzyazzvs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tmbcfemd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qonplfkv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3agvxuzge.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ibyuirfi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wleinpva.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yavrrwxe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ownnuacp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mxgcpnop.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sdlivysl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zdqowwbi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3thiosvmy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kiqfebrv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mkobowcx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fyvbronn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nzpclgvj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bnkzgkph.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fzibcsnh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jojgvdno.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vpkfjemt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jhobgaoi.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ospdeamf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3htahuvqr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kvzppcgh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rabacedl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ybvjputj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3elmqrabg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3qocbcwdt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cmncplna.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ojxpeeph.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xiadtzcc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ybdhqvyl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3plcovulg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ogisgvbj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmxklsyq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vmlbiknr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzbzqnuw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3uuzuxofi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gmcofmma.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3francxmd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ubltwyzh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lhklytmw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wvnlzpet.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ysudllar.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3osfusfsa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dchskapb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnljvqhs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vnvuzuov.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bcdxbrpz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3woyemgjp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pvvmladf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3haasxhye.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3phtmaepu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3jvoflqou.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vlxmfnvt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ullxdyot.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3izsiowbm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3dfuaduop.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ozduwugv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3znmknumd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wuvuuhls.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sqigchxr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xqvjevao.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zhhrmhro.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3entcixuw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3utdxcohe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xdoggtfg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vuwtrdcu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tbydhkii.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyfkjhrd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nehkezqh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3yyauhhko.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mxicazya.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zjqvrypa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wfldtcyz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3crxazgmi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3doqmtphg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rsxicglb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xyzsgzwq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zvzaeqcy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xcriazqy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ryemfaqj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xacxtytb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xxovdtdz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kjqdldou.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qkberhun.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fjjbgsqj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dfmnyjcu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lafywbsa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dcucasdp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bqvtdolj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3liwnupwq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3erqeibmy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3aqctqlff.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3opozvgph.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yxkwiajn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cvfxgpco.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kozohjit.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pchficbz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3lbomxcmv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bvbwaitb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3mjdbhmip.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3uxtktbwm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wabstupp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3refqvrpo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3upyudcto.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vojylbpa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wldmwpnx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xdhkwfoq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mgzroimf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wljmacnl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3urzefjld.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3maechoph.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jtcywumn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzghpxve.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibjqruvv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmbfrye.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ydjytncg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mzplgask.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jlvlpuph.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ddsvdnch.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bolplrgi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3yzyprvdr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3geczrxzh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3reqyepgz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3txkrbxwi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3egtmqryn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3swswrmtw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kjghvzfp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3yigueijq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ahuwwlye.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aspjcbzp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jkihvasp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eraixuir.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrinjaw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kzaonujg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ieshufcb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mezsimsi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tjbmclne.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3alxkwyna.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vkczjhjf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3axhracnl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sofgbmpp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3smxezyeg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fbikmxip.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3aoepiiti.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3olcdqhzp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3aomjlkwk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3tzcefles.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lahbeowu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rusqruom.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3iociggqr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yrzkmgmx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3xqxsbplh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nstswtnk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kgacyisz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nsmbxwis.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dnnlxkyp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qzdccgal.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mgcuiwmt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vmyqpjpr.html


<!-- 参考信息 -->