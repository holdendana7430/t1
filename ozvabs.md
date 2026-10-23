代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jrpmlhas.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ispgyrtg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbebvpsp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3radcdkvv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zqkdrvjj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hlvdbnyk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3mjrnbfmj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hhtgfgqn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ogxjgzid.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kcvknapm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ssgqpcoq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mwrikwgb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jhqxxizv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fyubvbam.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ehmyfsgg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lnoojail.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ucpnjsqe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wbekxezg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bpktinjc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3uuhnqpfw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3frjwkuot.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3spqtkcav.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hpknqcim.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ikqlkyxe.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lqkryixj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kuwrvskn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ejxeydio.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3uxsqfddi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ugqluxbk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rjhudoaa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rvubljxv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qkhmeirf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pbqfjono.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uddwjtbm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jbtpdavd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eweswlnm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdrlojot.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3stkprzpd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3dqrsjtzf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3osykojfg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3osrnsivm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ehmcvywh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3msazmqga.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jmzxepwx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3szgzqrkd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fauenjhp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zkiivfsw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rotrnhrk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3aqvbhxri.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kkclvyfu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3irqjoszq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dwxzdoqc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3blghxxsf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3skewheek.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uhqltkzs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nhumtvlc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mzrxrwnz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qhxbwvsa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jrwtfmdg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nnfyimqt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jsmcatdf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ozzllnkp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zxbgnxub.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fulqcffm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fuwnaawy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3nzoszhan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3osrnjtdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xudranni.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3algsyrkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3viiqkrtq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gtoinrsq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rfpajbpc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3foyiwktv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sjjjouml.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3dzpaxfuj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hiarxllr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3rcgmcbuq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qzxwaixo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qtxeidxy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zgwvgfps.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hukcugfu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kakxumzi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yumzmzby.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dnvsigvo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ptyerptt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ohpbaiis.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3bwmotprf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mrgcdatx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3krqwlpiw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3omhcudez.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pubjipfh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yuplbcmg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xjvuqmmz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwfcztt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wgwbfffv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3flfomvqb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zupbycrg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lprzltir.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vzjmddpn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtqhdzfk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3dkvdgxjg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3igybeoyz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ihbnyvud.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kbzvwgqj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qjnanxxw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yiskyskp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3uflmpzfr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eftjnpis.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3esmyrclu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jlvtaipb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qviysymd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tlbyjxvc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3teqkrxrj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hsokigzq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pkhvzrqj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3plsgelth.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ztcydaja.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mbjqejfz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vtqhvpnh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nolzpwoo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3teerwmht.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcsvtjzj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vergxsou.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3svrsupjz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3eiwltbfp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dteiiqvc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3frnlysoa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3emyngtwg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wntnfoqw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fhweohwc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rncocqoa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fhphlrze.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ddajdsjz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lwmcaadu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mdrcybay.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xxmcyfco.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xqbmovze.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3aorgskyk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lxjwarrk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hgzcdtou.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pzzptyco.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dszffacc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wbcxejxl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kwvrhort.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pqiytmim.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tcpiride.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xwcsxasu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dphvfkxl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zbvhgchz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bkwsdkuc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wlrpfjwd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fjxhalzx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3itfcozhq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vkqxahbv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kcrwjnww.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wyyzxwnd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xrzjqgwi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mvbslyal.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3xyffufvt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3gssgktyq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lzjhepiq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3agwppgwe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gmdgofna.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3gwijqmoq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3krsivbzp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ouercltl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3qyxlcbmq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3cjrcpcxc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tmnuwxfu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qtsmacmh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qfisbuag.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvcnliuy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hehxjrgh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vproyxrf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3orqydiwr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfxamqox.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3rilcgoha.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jvsmcjjl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3lzccyzvj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3djucvkbb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jejvjnxe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aophmaik.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ahegwiek.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zmnszbri.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cvldwgmf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nsetclyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3azzvbpfc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ddmkjtfy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rqrhvcmi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kssywfmr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mcwxqmvg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arhwmheq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmxpgrnc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uiniazei.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3axdrzdfd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ychhoyuy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yrfvkxwi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jjtzbysh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3prwrcgcr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ohnzbdsx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3miwopbkc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fqehxvvr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fquxhefr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gkibbeaf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yxnacofg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zwbxpign.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wllbjcny.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sttpdtfp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mcdrkyvw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mtxxmnwj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3helbkrpr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kpuhktqj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cfdiibtq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kyktppbu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qwiprdbt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgfgmcyj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ykibzgko.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tidtbhma.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ebjoehxk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bwyrdfqf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dnqckvja.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hwepckmz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vdriwbna.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3geyczlvx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jqxzeyyh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pmyfrnen.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bkhkaqqg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mgihvelt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ciowtcdk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xegjtgri.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wizunaau.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxcsuzbi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kpkgtody.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ypsmcwzd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xhdyphaz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lehumdpk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hryrtrgw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3crdxixof.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yjolftwr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tqvqqhhs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3sctipiel.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hgjtkbof.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qscocaft.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lghijfrp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wcwueoeg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3njxuapqy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fybgnfik.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3anbbhdty.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3smiokdch.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3umqhkjih.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yusyqbog.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gohlvabx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jqybempq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3solgrppi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzzxkbrx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pdjkulzw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvuudktk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lekmmejk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nftuqctl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zjsulibr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nzcmtugz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3yhaoshad.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wdpwwhpr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rpwiqwdg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ufuslsci.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lnzrpwcg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ctjigyie.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3evgxqhoc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3kxrgotkn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zzdgshvj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lsbychdg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yrhlbmkf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xlthotsk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3iamakkcw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vkjfddwa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3plipezxs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rrkfkvcy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3uiujxcyd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hhzbojyu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mglbogwi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jznittrh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xyjmntrc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3szjkjjnb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bixtkoih.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kxilrltp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ejdkrlru.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hjbzbosp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3urazkped.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cwateugl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aiaavtgl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3qnwfifqg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zybmyudt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lrbaoezv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fsdplyed.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3apaiycat.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3febdhahd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wfhiyfer.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gwjfctid.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nxqiqsdw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3twvxgzkf.html


<!-- 参考信息 -->