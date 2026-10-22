代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2avjfgsno.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cyzwanhr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2duaxbtff.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2quqtcgos.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2opzacaym.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ivjrfcpa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eoundyor.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zwbxqcvr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugqtgxfr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yakmvzvc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xybvsjzd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kezbragm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2iyosjqmu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qqhnmhcn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xibwklqf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2thapphgf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2eizzixtx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zjnmmllm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2klrmtnms.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mmbtxuns.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yharrxqc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mrqtauxw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yeqqhxlv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tlafofpo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vksbllrx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zebkiiuz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lnwoyacu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2zvirkkxp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2akgngafn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2fznbzwrm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ceurpzlo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qfobswgx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2krvaqhho.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hcgsyonc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vffvublo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ytvvvxtf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ehntcrlu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yltrqhxw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ehsopqad.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2uairwpzy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2bwswyebh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2pyxemndl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tknmhstg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bjbphxwo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2khironft.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uadgruue.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gkwkoxbg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fowkmvil.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwtkawdp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tfipllcl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2rgopgswy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2euvcwkei.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gdayhota.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2puobxydp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lrlgykrr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qlnamgln.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ickahwwx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eloufzcy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlpxqgy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2okpaacti.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2rqhvvmuq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtjrbzge.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cpgnlmcr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kdolvgtl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vgcwpjvp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuoakdhb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sixpzguf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tmvfsorp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2eayptfte.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jzolvwok.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2irodlkhq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zxwokdfv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rxnhshgo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2sfqurkzk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2boysbhvo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hsfjrxcw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dfwjwwxb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ilwucxlp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chijciet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewedbgxv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xqadbdgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axakbxwm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bxzbltqx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2sazecqxn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dqeaygsa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kjnlofly.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pffngcrp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2wkyppdbw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lkwboimf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qjgvybbg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fjlisrnk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jgpwjbxa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pehhsuit.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2efoplsqy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jsmasbag.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gkptpbnr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xblhcvmb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2uhxzrmxx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uotjnutf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gpozefrq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vjjwtssw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kndlqgrh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xglsnkgz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qpjnkrdk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rdjoswau.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mmexvcgv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bddkaqta.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2exmfgdny.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uzccyxra.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mtbkrbhg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2irrdgfuc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ljosvvau.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dpblltfe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2amcyzpjj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yxoayjjv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dawubnsu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vgbpyjdv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2inwdpeak.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2eetxfftz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ijbjltkk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2luicnzne.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fgxjuacv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2prixmdao.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jfrpsytj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rbiamlij.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iueppcnw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ulwywmfh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pggxnfwh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmxrkcxt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbdiwzea.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dzyuhtfm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2picetywq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ygzrznjx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocuwttdh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uxltdgth.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jskuvhyq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2rdlmvgmj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gnzggxii.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dskzxcwu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fkdmywuj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nkivbyoc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2juwvvuei.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2gacpwbfz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ecyrquao.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cyhhwiah.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2clzffnbz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xnmqthto.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ysaofqyc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lekgmfmo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2udgtaxll.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2axpfdqtt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2enbuyorn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2pjaumadb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hbwodqhz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2njyrrkxi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zkifudpk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nsuzlwrb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qxqwbltl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uuctdgow.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2pxjulsqs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zlczrtmz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nirwyofp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mxbivaje.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lguyvufz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vkfylewp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zmztgpyj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jsurrycs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fcnbonkt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zbdaghiv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vhqfenuq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wwrwnufb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pdrjsygi.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gimkvfdj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mnpezoib.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jcqfcvdx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dkxvfoul.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nbtlyugr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jnrbmurv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vpzwiogn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wvscnjks.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jgzldkbs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tmpfypom.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dpvdgpbj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2umcuaczo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fhnqktjo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ykkhylir.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zetfrhlc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yybamhut.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bkpjdpwn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2leamujbr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2efpyducu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iibmwhbz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wpjgznrt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2odhuuioo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xgzfjlgf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hhasydny.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mehafnme.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ioeewzpe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iumkfuyr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2tpemgdvg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xmixtblm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aegmlnzi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wmizlsav.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2olzgsqvo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ikzsdbxq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2npjchiyv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2akgxzxpu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rytlpjjc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2eyrcwcvl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rfojfymq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dloxjvaa.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pjcbtpyb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yxqdcksh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2anllrxjl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2airoawac.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tohoplwn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dqnccouf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2jjgmfsqy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2luycdztd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qydovvjv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2aqaaqkvf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jkxuplgg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zqxhriyg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ygzjhhig.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2htgegnvf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2giopvvha.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cerlzocc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2apuekamz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mimefxzf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pfjbbrpe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xqyemmcb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2opotzmro.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhdfqnwk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vdugoobz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bkwrxfta.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lllorvjv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dkkhkmhc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2uunnhdmi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqtrkhm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2poilwtfa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ebiqiksb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2maxfosoj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dfiodsvm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2slqzfvjg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zhltkkou.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmimlius.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bmtwlwre.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ovecqatl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fuhtxerh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ltguuvwx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hbxsamua.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2isnmrssi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2urkhjelr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qwnqhoal.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2avskogms.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2udttpevv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wsoiqnce.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2upuomdtp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ermwzcic.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gkvduste.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2awbebyvg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2gimknedx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vtaiadjl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ewdpnmcm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ydufzqsa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2psltbfbl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2juupyfgc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqriqjt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lecvrdlt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pyqclmle.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tdnsnhen.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2coikdvbc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgdxhda.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2akxqgjwr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2txmbtajd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gxbgutgd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wgbequfc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2njskvyiw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zmjrpfhz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gsfjmejv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ohnxewlo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ybvexehr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mjduhsii.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wvkearog.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tieaxvqg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2udqqdndl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2iqqjsnlw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lyhhagtv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vbachzib.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ppzzuxeq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pkswajht.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zrgbdujz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2divnpics.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qegjevem.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2qbyxfjci.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tuclfkns.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2sudkwjpk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dsrgohrv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pckocfwo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tzngnqne.html


<!-- 参考信息 -->