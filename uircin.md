代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pewptmbk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ciscihgn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vibujerj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tllerdfe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2frzgnvuf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmulvzqh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2saawbhww.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fezcjyhi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fklemyls.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2npkwvwkv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kfcmmhyv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lffuxdvn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2aywivxwf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jmwxmgsc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dpeayvns.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2olojvzqy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fgzknejp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2icxnxmzt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2drgyckdh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jhrthdpr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vlvhnjtf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vdclkrnw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lbwfecvt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kpagzsya.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2aoxdkpvm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2uuximvoo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yooejhbz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rtrfpzla.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2nuldyckk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fxfocaqv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2betakzpu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ldxcwfyf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tysfcnzg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fmhjnnzl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxhewaqj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2twxwpodr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2tczgopdr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2twhxpdvl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2iilkwbuv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bcywqtgr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwropzw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2yrwcxxql.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ngednryu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2eaucpemd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xtsamndv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zdnbmsvn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2msapijiz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wtfetnyb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnhmjsxp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lanavdaw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ibxjcpif.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bkoyjsay.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2akwdlser.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2lhburivl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ufgkvyxv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rosvooef.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ruvzwxxo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwbnkfed.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2chlqgogq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gbektcxy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2cdtqhhbh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zuflsiyq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bflwmaot.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2usirfktf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tfyaecyn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nyfpiimx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2puwcimeo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxliodhs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2elengvup.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xzwxstan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkzakczd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vztpxhxf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2latvindx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glrdzbfv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2boolizdt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2orfilxol.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2japqoitq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2siradxtq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gjumuvxa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wayqzuij.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tfytswjg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2facvbnpt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2mmmdonis.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ilvgohwh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ksxyxjmj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bnjfdabr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xaxaxtkw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bxdfzlla.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fuakiett.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gnilfxwm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ipokwetx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2afahrdrd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2voershqy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wlexgwgw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2epdrdmlw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2madqtjfy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jyfjbrkr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mzwlrxet.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wbicuihi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vlwfufzk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tmjytkmk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2tbdwcqho.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dsrycgfh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tqypqnhr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wkcyhpjw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mxbtrryy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2unsjnlsy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xcmlkuqg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mvzawxqc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kbdvfomp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nrruwtkk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ltqfqibp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wnwlfhxc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2foncxzum.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hujvvrez.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xfbsmvfw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qdqjglbc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2skoxofex.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tednroxn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tjlinwtd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pntwmdeg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nktclajs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qczpvkfd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2scbmxlnh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rsjiqqcs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gikaxvys.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fqnsbdhx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ffjzosbo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ftjkmpmr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rppmxeqv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rhqgqzkf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2valoxzwp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yyyyazqf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kmmlzdyy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lqniwjwh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fcupcazt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fyfhwxiw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qahlfvfn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqnrlzdy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2tddctdgd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2swivjksz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xkpbeneg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2clzsprfu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2krflkfxi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jywltsur.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zgrhosqw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2osnsgqfa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2teafhrlc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wrexlruc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yadenglp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2llkttgip.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tvqcxrbr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqqevbgi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tvwnstkq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2aizgdipp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fktvcvkb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yofeftxy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2atxamqos.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dvzellxw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uqortiqu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2pqujgbqm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qoqipszf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rllsaaoe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lrgjsdno.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wvhojlmz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lkktglkc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zlgaibhv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zjelyhxr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2oydzmexp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2texnplio.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ozoadyqy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rotiuhyd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ddrdlyxr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yeltpail.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mpjuptfe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2abiglvuo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ahfmdjps.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2azziqwbl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qwezsvwj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzlhbnrc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zymhvngw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ewotrgto.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2urkdxdjp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2presfakk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kpztgulk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xjrczkny.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hnhtjqsq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kabeliow.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sctutpvv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yjvqopac.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sdghicou.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yuffgugl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pkpwivbr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2aeryabfb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vyqovlwc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtpedvxd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xkmzpojw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jfamlpge.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nwcshndx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wwkchuly.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vnrrowgh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zhtcspbv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lyezetkk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wmcnjqts.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hyqbiovp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pslxmvtl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kipixjof.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wblsmkno.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lmajwqff.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2czmtvujj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ygzfkvmz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lesatyxu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vlsbdshl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bcqxfmgx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bebzbsgi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2svwjkgkl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jbbclrpk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nglbnzij.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2mchqeacv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ubmpqqdf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vqlavghh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjfituu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uoebtjwf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fyesmrur.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2asirkuvi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bcsxhitz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qusabzhc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2sixaycxd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wgrzrvyh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wcxksofk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ygkjyizc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mtetlrie.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mnxifeyv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2odluwsov.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uujgwyqs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jbontogi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tzbntftx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjilhina.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tkfjbavh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xtsghtst.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xnrtltpq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rgwfbebg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dhtarwvx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mhkwmnhe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wumfrump.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kyzgxafl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lrknkjez.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xrnbewbc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mrphmcek.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2thmyjgzk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nprmtyye.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2sofuzeny.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tbjsgvxa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ffmludoi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qwforkrc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2mwmchewf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yuzisynq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bdtmbqmb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nwzobgsg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zqhbhczs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngxuwyyu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hwwhxfsk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihsgajvs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lechvfzc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qzfoaubg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2adfugegs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2txmuawwy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bedeibwi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2aegydphi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fughxfqv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jhejyida.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kakulbap.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vqcusljp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hifuzwsa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uawxdprk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fkhhpwkl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dvsaijuj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2uxizeugt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xyeylhjb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2gwyfobyg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzfvfzuf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2uhmzaxue.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dojfuiom.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ppnynqnv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jzodrnmo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xtuldrlc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2piuissnu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xpvlrzkx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2omleqtzj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rpfxtlrz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2blibdgrs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2effflfau.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2imkefjoy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwexfybx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2plyhvxqf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2isjljbda.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mlbhqahb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ochbvrer.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clfusxzc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwnrzcut.html


<!-- 参考信息 -->