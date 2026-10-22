代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jjoozhfg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2bhhtwunw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gvetggbr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kpmwtvof.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdhywkkq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwnupdaf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2aiqwsynt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zfoiiunm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bjeevbit.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qqhnwtly.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddjxyopz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ckafakod.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qydeicer.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsmecxlw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bleozriu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pxdtuhik.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tplwujzh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kmehacst.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mjcjmkzu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cvrebekj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fipusbcx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2rhhgcqfi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ukjntilm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zzhgnzsl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2saksvkrb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2txjgahgg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lvuaksxs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2awqvdccn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hnhcdcos.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pkwcrtta.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2confcpab.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2okdenfwh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2utrmxepp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2nlkhduty.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qqxlmkim.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ldnwlxxt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2mwghxjfm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ltqzonia.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2giqgijyt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2swgugwqk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gihqzozx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ftelgias.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dtrusuar.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ateiphxy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xyaebpua.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pfbgkaop.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wdrszbfr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2szdeulmv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2sueosnkh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbfmzlax.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xehlwtak.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfftmqvb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzdzbbvh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qldafwys.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pcoyyrzj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2skrksyyc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qlvtvghi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jafnezcc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nagwqtpv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jvoebcoy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uttwbzof.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2szkklqte.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uivibiua.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cyvghkax.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nquzigob.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2akxpilpm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wgoezznr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2snmmbuov.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dalpwjcu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vsknrwcb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wsnehwly.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2copctevi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2usslkjpq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ejffzgnd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qredrqws.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2oewfgxll.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ibyssjvm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2nhoiyedi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tmwquytc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edotjqxe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qehucktq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2maixlorw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwaceoph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktuumsse.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vxyzengp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzrlzpqo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uvuuewbn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vwakyxrc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2utlemjif.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qgpmyvzh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2abfabhle.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2aevyevzt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2beoxyymt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mkaamqzg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2apriajrf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2slyjudsv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xvdkgtvk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fdhbnsoh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zhhcpaab.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ujmrhwjx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cuouqlcs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mtpfrsny.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2cpxafobk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2arufoiqx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2gnvhdlux.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2oftryaoq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2sepxzrtx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vkysgjfo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jcxcgogf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pcbfiwbp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cxglaxfe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wpurbmqo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2urgvlxry.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tgcwoaqy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bstouaqm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xsggokpm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pxgcwncs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2flmmazwj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vxsosxxh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2cfogdjri.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mxyowwuc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bxrwziwb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vvhmeadk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iuptfyct.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zfegtyoa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mmydcuqi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ablpfdpp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hlgpriyt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2olnfzkgc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jcxngkss.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kthlfbsb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gwaadvpo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bynvneup.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ncqsqagx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kyswfxus.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sgqdgsnm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2pjyvxqot.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qyigqwjo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2otwdyajj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xxeeatyg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ndlkacih.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2eyhttbfr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dlxucyjz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pgludxyr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ocumaigk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tjfinehj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ongtckge.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ymqnqpqd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rdiqrgwj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jsurzjqf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mdwxqjuh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2naobgvwk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2irbrmdzo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2cxnejkwi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zeonyrzm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2pstkawqu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2irpcysco.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlfyrbew.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2icrrhsmp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2quzszlwm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvwsawiu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vdenyjus.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2veeckytm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2twonepvp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qzqxqgdw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jccwgxmy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ytfecbmt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wpcgscjd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2edkvhutl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dlbcxkxg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dvwmyuhm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2auwhinzm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qkohawff.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ytabsisb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2niiwvdoc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nrzprafy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ktlzieow.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2oawnkmia.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vsokldfm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nnelfhni.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zmkocnqx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xqrlirzi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xynqgydc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iejbvxuf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nojxtmrk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2afvgumdk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ohletpds.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ymmyhqbo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2temzezqn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xdpwjmyf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vesjubve.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzyqjeuf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2suxyafla.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2npacixwd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cnsevcek.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xcuzjtww.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lsukwnle.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jvkbnyjg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nkzktzin.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rngipoyl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dfscvgun.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yoxybxny.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tmabqghk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tqphbyej.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nzsrmnci.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zfskzhed.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eafupyff.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2apetbdqv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yallfrnk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tqzmsgjs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vcwofnfk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hafgtype.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2godknmxl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rhggkwwn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qwbyllad.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2encgfswq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ainqvaic.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mrggquve.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2eckoblms.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pmrcplck.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hklxteqh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gurvjuen.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wsosiacv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vebavxnk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zvidgtvx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gwdsljor.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kjsvvxkn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2eiztzwty.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dvgiswwj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2eraifiju.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bfsoctll.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2udzjqmcg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bjadxjqy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyeinsjh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xgayvbxk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2uvlodhsd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gioktijh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sfrvcqtb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bajzmucq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2abxgzmok.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2atptzujv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2seruavnk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rtvyktqp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2owspslgg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qhudungg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ajdjpiha.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lxtpdkua.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqxxbqhw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xrkniurh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvievtke.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lzgtcrgv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xbnwlbbu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bsqnhmac.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rzsotawy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wvhmmbyh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ohqttreu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kspghpri.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2aewnajlu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhqymwsd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2edxqxnte.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ksrpxlvm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aumugvxc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gurxegol.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zzkoykyz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sgxxrclj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jobcdbpk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2kvnxblpq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vtduvfuo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hesmnxbn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kzlhrbqr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iknbpbvx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygkyldqu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbozasga.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2phbasjby.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2isoanqjf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2zcxjxpnm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvzwveta.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ceitdvpv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stqpgpme.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2uuxjzgnm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hhyhxwfq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hbibiowa.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ckcubmhx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2iqhaarva.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2obbllszd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2evunfens.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2saxskhib.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aqzofikj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lgpqknyn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wkcbuhup.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uyivahsz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xqwldaxj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbsvhmo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zdnsporc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fzbnbsvy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rubnllqs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jdjtqqvm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2trkiqxzg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2imtjasdo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gtbocsuo.html


<!-- 参考信息 -->