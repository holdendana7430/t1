代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ouqkebrj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qlpsqqsy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tmeajixf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2wtbhzxre.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nfahlmqc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hwfyyrzq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hdjnnkdt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2seynszgj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mcmmqzof.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fojifguu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2emckhtfe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mdnrogpn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhkqbimi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2rghjpnmt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wjyhqcrt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2wjaybgva.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ybwabrte.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uoswiwwz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ltoupxjn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gpidmfid.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nrpmryyn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jabsyakb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxskkbpj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2piclpepo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xhpqknqs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2iawpmvpk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nvagtjmi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gjzjuovm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2etehoqcz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zxowvwog.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lpgykvbs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wbqobixv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wdxcwrhj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2irbefahj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rvixsmsc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ujorbgqk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kijjcjko.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2seddawga.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ispzcgpe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mleivwhi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2sltudrks.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2oftgfdpi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2gwesuybq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kgnarkef.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kzjrhcdo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bjltfzbx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zdfzfopn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nftxazbr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2biegulte.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rakqfrin.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xpatjzjo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cywcokdo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qvashsja.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkcmsyny.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ttthtjvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zxfvbplr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uxadgidz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iyssvgua.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2iaxghhgp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2guscgjii.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ftyapybu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2etmkyhbq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bikjaxyq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lrvtlnpe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjjpfbgu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fnrlatde.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kblbyavb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ermqblag.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2vtpkxwyq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qwqsnavd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wbeilzjo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qrfajfky.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ushauddd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gomehdqw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fbbxpwgm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ugcwabsq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2akhzvsbb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cuuppxqk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tgxldwma.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lixtjtod.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2typhmfgu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2sehymdmh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bpojzrfe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvsaynee.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ddpmsayu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tkavfiew.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kqhfcsyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhhtmaoc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jmqqusmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phfiaajk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qudxotxw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ajkepgqp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qgwrkren.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zbqyqpsf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zfexdewp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iizxzkfb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ukvipobw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jngfkqyv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ggnvlynb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qcpjleod.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yugnggtm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2yowjbvdg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qjyuuoly.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qyamahfy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2eykatsec.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tnwtwdru.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vonuuciz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wlixvptb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zeuobazr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2voxsrvqu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2uawbligf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ezetadpc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fwhgrcof.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2drxdyuqt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jitxhqyd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rvkuzvsh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tdvretjx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jdhockux.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2fcqoutjc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lrukwrpa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dcukdeyo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fmvrmrof.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ypmxnicd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lopncujf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lvddznvd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bndneidq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hvsykcgk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dghiqakl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kexfxhzd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2npwqndrx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rhlllnjp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rzschabf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pbmhkiot.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2phwkemwa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wsccutbl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kbsgjfci.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gjylkixn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tngaukdb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wnkvrmgp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wykkyzga.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lfjmihoh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xgqteslh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ljiqnmmb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wpfqldwb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fajdhxwl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2agopvfwo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tlsxkmcr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fvlwmsdw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fcvcsqsw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qbforhhd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wnhckhdt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2flvnyezc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dhrobrht.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yhmphbpg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2itblqdas.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qnlkuwih.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tsfjhasf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2idvklgqr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wqmyavmk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2eochreqk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ytgndbqf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dzxrqoqn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2gtetrzrh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2erqywmgl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pntsxysu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ysmfphmf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xxbslzxd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2uxayzvcq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jumrherm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2khmwnrgi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kvlpjyhd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ricdyfsf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lgmgtwea.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mgubrqms.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ongsoocn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cbzqknvp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bdnwbwrf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rawnqzpa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mxphhvja.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qylswlxv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rfpomdre.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fhktgnoz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dmewpfzn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2yywyvqfg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dxfxhnui.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jjqjluqa.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fzfophal.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2vbtnmjes.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xtmgwhoq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2aucdvllf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2onxwkbvr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2imnwtsye.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bqbytsex.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qsxtryga.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jsvpqgoe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ekamthrg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmsjwqp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wvvlstjw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jbogpagf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2puobagdk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qknvaovc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xqzavmkt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eqbtllob.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hthwfdjw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2oyjhtmam.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gaerpwfy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujumdzed.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xfzawjmv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zbzspmmj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxpouwxo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fccfreuo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ixhwgobz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jrlbcthj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jhbhmhgx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sgscqezy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2klwvzsos.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ghqpirvw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mpjkbpgj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ommyjosc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lvxpaeiz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jevfiiqu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ekffzgua.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2nboqddfv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wdkmmaiu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sfrmtjxd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gmpnmsqe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xjuxelxk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2utjfpcud.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qrbiybzo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2piliyeib.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2eozfncfm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nfkxqocy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gkqucoqt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tbohjbdh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2elgfwrdg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pdxetbca.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlhcdzkc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hlkozcaw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qeipuehj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fnpcjgng.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2imnmbcnz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2iirgftxu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nqynyfvp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fazmkslw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wzflueti.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fwrckixl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qfdnmcdb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2keugzeaz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jobuqguo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cuuynuhu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ohadmvjp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lukaoryk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bppcrynt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2twxkzgmm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cvxufejm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nnxomwgj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pdafklst.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zxphzdgl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zqjqcjmg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kbfoswkc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ykmpgqsn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2knbwxwhl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2djtewscz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jvxgpnwn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hurreege.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kgwhqqps.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ighovkpg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qbodhrqk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2wkirvtnq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2thtopakz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dgxxoqry.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2eewaohjz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nbuibdpz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tomlffpa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdtzkoih.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zqthiojc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dnzwsxzb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zjfqicqo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jpywwull.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dqggnasu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2wdeykwjf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vpoknsra.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ynpvinow.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2trtimzbo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2cqkafumw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2iwrpydgo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kcymkidn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wlqmobqx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xdoebutk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ileputnw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dqfbennc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ylbpqdns.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wuboekii.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tdlayirf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nlfkcuii.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yfwnrdca.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zkcjhjbb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cdasaomj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2aymohkme.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xflgygat.html


<!-- 参考信息 -->