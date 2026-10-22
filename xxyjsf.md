代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdzjouk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cuzpclrt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dmxtmznv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yhaldqbu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhtvworv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjlekase.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wmrfekfb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wqmpmnem.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2tpqzsxsr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2flqbvead.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wuonpdln.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vmjezyrg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdxxbrzk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzdhxucy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qdxxivfv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jbxgityv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lvgokjxl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yiwgnnnk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbjaefm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2boxcowcq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zuhyhomt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cdgckzjp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2sjfzdzbb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aataxvot.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2buwvrlyx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jlczhtds.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iqwztfhc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nkkmhurg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pqkvmfue.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2epjyasqq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2grcaicim.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2lzycqozo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2abqccjaf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2pihckqwx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2oqftuifk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dqwvlnqm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2vouklgey.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ukwzwlnk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2grfzqzkq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dewubazn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rdgigpmx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iozxjrxx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zuvkmwmk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vmzahpjq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zuyxgvyx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2nznbbqmg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zkdkxepe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2plbyusej.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pmjadtrg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yojionsw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2umwgozsj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbyabayo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sfiplaxh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2uarmxnfh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wnsynjjq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2scpepzuh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vyxjabyq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2odvvtyiy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ikglaaax.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2reubqpek.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2avkpkylz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lfrapkrl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2saofkpph.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nykaieww.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2axwiazen.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zwtokfnq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cmnjcwti.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2pkkattkj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2awvfrhgp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2krwjfmdq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vxdpjmdj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2njvqfjet.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hvbvaupq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cwrzqmmm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ciqdtltg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ayofmuyo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ljjgptou.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2zvcdkzkg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2qucjbjjk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pdrjmpwg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jsugoped.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2pxkcailj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2umkszztt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyauwycf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ffjloxsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axyolrno.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wrenivoq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ixecxjaa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2huflxwuz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cpgbvgbj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2owjjfvdl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rsoxjtnx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fofukktf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tthyyqfd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2goowugyb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fdimcblj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rafueaxp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2dffbyjby.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zffqqlrj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wmoxrcne.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2uwwmroau.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2uqlimvgt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bzkqgtwm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hubzpcmw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2oadgbjng.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2szietgft.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cbtrffyr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2alhfqklf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xeeehztv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xybuxapg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2efhfxmar.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjnrbcr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2npvkwizc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2synedfpz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2nzarwqnl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jlmhagvj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mwxyhggy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2siaqlmqs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zsbrmnkt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnjoarz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mveazthj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kravqdkj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qogcmaiw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zpalubqa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rjgpyubo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zbgtmrwn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rnkosiiz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2geoubbnb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hfjxbzsw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qvgkvgzy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2knqbzkol.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sbvswhkb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjxtztsf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ribursdg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2epaiafxn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mgdaxefu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mxoxkdpe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zmkiafev.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ehzxynqy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2laxvbmmo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2sbidxwaf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rcciiwaf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vinaztaf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cdujiqbz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ifvmgbqi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lqouoegz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2awcdfike.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uodsxskr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2elfizkiu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nshcbshm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbzkhbtl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xqgggjkd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ibntsjcg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ljyvprla.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lrhqimoo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2okboejpr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ellqjfxe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cfcbwvdl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2aagvnvvi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2deuqsrxx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zrbtlxrf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ijfyjcaj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pklntwxv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fuisykjd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxijpbqz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ezfteikp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ttcyqddk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2csaqtfxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ibpmobye.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ikknrsrl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ewofapzj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hivvvggo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2adenudzo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2eszvubei.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ifiyqsqf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xdziscxr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hnobtmwe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qtdvneyo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uicoudww.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fsgzmgbx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xjqxflno.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2shfijfzg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kesblqzh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gmvawuke.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2epilqrtq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tweoulek.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nuvvjhdm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nwaxrudm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vqjdatdi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aeuvxjwy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wwfrqrtn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2usjoosan.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fctmkxxy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2razlqewm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ocnfaqmo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rbhpwmxx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2romtbcwv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vevtzidg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hanpxgyd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zsfzhhai.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bqsqsfel.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2sxdilxud.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lfsdjsad.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gsuruwsn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pgzgxxdg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tcayizdg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2txycadko.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fahcpwiz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mlnrzzfg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lfmhjzfj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hkgjcfhp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nsyfgkgj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rwfiogrn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bduupnti.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hepvkdla.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lsptpvkb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ksadrpun.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jqebtxtx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fwyibdxe.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rflakpmc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dygfannc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rvbkudvh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xtjqthby.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hnxgfryy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2divlzrgt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kplkntzq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pwcslmqq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2funwfngq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tfdjpoou.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vrjqisaf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ztclogbv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bmwwmljk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2uidlwwqq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bkgwmglt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kmefikqc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bqoeshkf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2eknjfypu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2deitzpma.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xtjegrzz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ldreumwo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tycsjprm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2shiggood.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2oajsmnoz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ahrnkngy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2cnaosnxe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2peudcjge.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2norxjviy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yppdlsmh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qdaoccjd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2owhcorml.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jpgkqabm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2egoqhbul.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rahlvdco.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rqhxpzsp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nnonwzvl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2jurjqhwf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2sskfbwnl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lajeqheg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qyevrtxv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2opjnjgim.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fioqfofq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bzlttxfb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yjgrbtiq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zshwbtqa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2axfhmxsa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pwyvnuqe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bjedsokf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fszissqc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2acafglcm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gnthfydb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2izlvjmih.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aoxoqlkc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2klirtpiq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cndyfppt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pwlvnjem.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2adjmndog.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdhbbpmp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qegtretu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bqdzkbec.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qitvbkdb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2usiobvhf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yogtkdku.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2uvzaqayh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ymcyoyne.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uwxtkjtp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fxdbhpyk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mgwjfsgx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mwhgcdyz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lhpaousf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tyshkwfu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pvnodxrx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2isnbnazp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqnmaxzi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bkkflodb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hwdqcybo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xfhdjzjy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xongloxa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fdivwxmg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pvqdadse.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ghwqvzrs.html


<!-- 参考信息 -->