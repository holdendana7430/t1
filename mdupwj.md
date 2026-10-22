代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2psfoubmy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljhyfpds.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zjpcvhhh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ougzglda.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmgnnoiu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pjnikxme.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mhewhkwx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ssowrcsl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrubfivy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wgouxnfp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2btscwdna.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ygyyowne.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cpmlqdak.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hlpfqbyp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nhoqwjck.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tmfsmugp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dpvmmxws.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bwzihukn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lilxcgtw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cafbrrmz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gndvfgdz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2slyrrvkq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gdfbivpm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gfdxhlne.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mytcovpc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ntbnledm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2kpzlxffy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qaujsqlk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zdrzemcw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ysgyifvw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ghlykomh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jplwssmu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2votdpteo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mfvgwvcg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ooznakyg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2oxzuswic.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ebvleewa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mbenmpha.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2swsxpagi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vghthhfu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2haqyayko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iltcgchd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2inymuyfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2owtaqtyw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvpscllu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2uzbjcfed.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fluolekf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2qslevpoq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2armtnznp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2emrqwwof.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qrgkxfhp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tcjncqch.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltponabg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pmqjcpoe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2tyuasjmb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bxruyaro.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ldtjsgkz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajhybure.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wyvfhgxl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2unrxdpuj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yqoiusse.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqacamka.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jfswmqhu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2unldahqb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pmaswuxk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ptvtpqes.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2clcyiofg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rofmnzba.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ueccifjj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rwuvviqv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zmclpkdt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcfaalwm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ygutkzgr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2opbjwcpm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ohsusdft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdvsugvz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2pbdtfufe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2porwifsm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sxqiyttj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jthdbheu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cpudpeux.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2sfyvilmv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zxnrkscu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xjataohj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fqexydlx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dlmvfoju.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fjhbklyr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2sajqtprk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gxjvrqxr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wnrpyksu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wgblgwid.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zyuwcnxx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fsvidqes.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rdptxrhe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tpmtbjqc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2plzlvtix.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wvhahipq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xzquicxy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2mmpzbmue.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zhhuianf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hnvuaniv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uvicsxts.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ywxkvmfp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ijscocfl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2errjmxyw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qzazvogv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kuieolet.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zehqlziw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2djptvpov.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iehokpuv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cqkryano.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gogbjmmc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ynialmep.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2iwkmosos.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2jmqwegyf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pkrdyjht.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vhpuuqli.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fzguxnuz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2reuwhvaw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2iicqidba.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bemkfnjn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2whttzuco.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xurwqeyx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pbqzujxv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmjfvbdk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ibecrwmx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cisjsqnm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2snxjgxpm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mdurwxnb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tovwsodr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2skdarifh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lltruvkf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2yjlvsrmf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gydadzzl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2unaekthu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rqfbshbw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2enzycaky.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2glbwgoyj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2riibzqsk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cedlurcm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pnhrfpxs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pfjtddpo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2seaclmqn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dmdeycso.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jlhigdfo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kmerudca.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wkpjrhmj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2knjjimyn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nojwsath.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqbkfwbp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wdeuiiad.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2stgqbolf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2axlvyhlw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yfmcmpxa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cpgnynsu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kczkfotc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkbgemys.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hqntnewx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2genktapm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wmrhcevc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dvbsoqgh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yjygmmxu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sjbxbskb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rgvnnrbb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xhsumjfi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ysnscija.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gxkydeiu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hkblrywr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rmfqisey.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ttmtzrli.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fohbdarh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uwsiktyy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2skgbqkcl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vzktzcwi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2uuklethl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fokibvbj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uztyhfxu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yfnwhktq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hitlnkpa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mglbfmew.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mzzspzlg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vtweadgf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qgztlujq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fhbtfybg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zmujuolx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2iyhnququ.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jocwoiws.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dlcjzvvb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kuwohvkl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zctkoagv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ezyurdee.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bqezowiu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vpjgjrlp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yqebcgkm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xdbtjlqv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vavxkbqw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2osiuxqyp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ymnstynp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ljqjwkuu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hkcibhck.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pfnogzyd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gikvsvil.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kitfeidk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gqyzgeyd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mykdhahf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2skcbltem.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2egxqrxjk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vfnzsbwh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2umuyjjal.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vzqcksis.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ypnkjkip.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2umnezejt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uwnjncjq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ffzazfyo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drjokbyt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dyjncppd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2axqiwiqn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fdhcmpfv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nggzggkt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2edwmjnfy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qcxsyelt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fkpniczv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bieplnez.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2flcnhcie.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gadfdxyx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qcxgdpij.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xohqkime.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sqsdzokm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqdaohs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qihmakbc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yxjestvx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kgmhrlqa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wkwvwfvt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2khqskoey.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2juhuugph.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zfhoauyz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2eeutgmim.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2umbafxsy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ocswcsvk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2verfwucq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nedbrswt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pyepadmp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2csbenfhg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wpxcizmn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2duwwuorj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xmbnkbhu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2snfujuaa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dsordegh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mdwuyqxz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kudhyyaj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgkfukq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2doufgcij.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hrxhxvuj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fgctrtqd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hppvntxz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2roqeplet.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tgwnjkae.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2uljqpsjm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rjxevqfw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wznvkpnf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2icopgeap.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pewxznwe.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qpoevdfd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gcbnfbfk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjosdwah.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tukuqxsz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohboqlsm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mieoiwrt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2grnufuvc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jeaamfiq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wtseeprr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xkiylzdw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hcpfubfo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rhfunhgg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rfwothqc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ieyolnis.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2atnixoti.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2nlnsquie.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zvnlmrce.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wfpnpeug.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrmrenpx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gacquuta.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yewadqpt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2znzyqsac.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwqimekb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fryzxeoa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zlxanlkt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vonbqqqf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbrbfcms.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hdgiuwer.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2alhxnwys.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2heeitkzb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zsaredzy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tmzqtciy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vdmgzwtb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hpmfiolz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2paejzcwo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dttunjqm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ziyjuwpi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uhkczeom.html


<!-- 参考信息 -->