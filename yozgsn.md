代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2onpkdsck.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zlrlrega.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rowkdyxc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dlwkvwoz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oujrjqeb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2nkqpdlpu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vnazrtre.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hpxbjxli.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tzxirnek.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2uximylsn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rqvwdrwn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vyixwxqd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2obaeqrri.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2nltwyluy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vmyhilkh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2pintdwsu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ozgmekbn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rmygdbfr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tyjqzvse.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rgrsrpgb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2djqvvjqq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dodliuyj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zucfrzrx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2swqpmnmy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmggscj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2apqnkloh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2izobcuut.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2avaeoylk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sajpjizk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfyacsxt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tsphujcq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2virrrtgk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ngoouito.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tkhrmoxu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2axydjlcx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2csckqqko.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dvfgebwl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2asnozzsw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qmdlvtdu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ncibgfrp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2divbxbyd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zbzigymn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nsknilpv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tbhjyngl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sjpelzvd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zvadnaur.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rtplvzlw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2sgkbzgth.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vtcsghrt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2cdiiboxf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rzouxelv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kepcrzqh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lcuidziw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2clemjkpm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jkcngktk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rvkfzkvz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2eicwraaf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2btjyhhvy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pthrebsy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2urpfppyn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ovyerhxs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jxptsvec.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oyzkkhuw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2yoxzqtwh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jjvgfgjp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zljugyuz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dmokxcrm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zgxclzgr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2paslqqbv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nrlpfcfd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gwkgnirw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hjqxmgel.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgdgiagl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xizfaaea.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bbuwstwk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fhfyerad.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfywnjmq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2avnktmuw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fpkhoawi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vxrdwulu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2eutccyrd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jngzjvhe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2shugbabm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rvjpcqfz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zkabhlet.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ltvouenu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jxsnbonz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eqlrtrag.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pdyenojx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ejyuuqcv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hdugmenj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xwcwpoxa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2uitxvhoi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qufzckvr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rsnotdly.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pecnquou.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ecbufyvv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ryluuxyd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ierhujjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygoorimf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sjgtiacb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdssbwbz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cvxjiwvz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rrqhizhk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rhcbeacb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sgxtfnkr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2arduotga.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qzwovjuc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rmkhpwwl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2flytydmu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2sbdxtnlu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2muabfgce.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nggcjshq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ekpmkscy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nxrijjqe.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jwthabeo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2difcabuo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kcyrgnht.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2lbdkwcud.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2upwaythd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mytabnhc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xjlsictr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2uxcfplyb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dvoritxt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rlxvcuxq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2utoinezc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2kbaoeyat.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dhxnboha.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ubfhchew.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wqouojud.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dlnmogzx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bedtglxj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2bzuteguj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cujsmiia.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gfcxxdzh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lwayrnig.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kirqwzsr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xmhayojl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ctdwpuhn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jsujnptv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mostzsge.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dxiujpqd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kccgicaa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2knfwyzed.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2euqawuta.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ldeausty.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tiqlzcpt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vsrurvnu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2afbbetvb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2khcwrink.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qehgjubi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lapnvubs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2iwmjsbjf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybbrtxap.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2arecxdxn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wsyfszhd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ozrkeaky.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2izpufoec.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fqflijqt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fqmadngr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iwjoavvg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gsrolnmb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2osvmknpy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zxvascbj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yezfwhwf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2aaoxeamk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rxzktjpd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2koyckiko.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qnycqeig.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yylzihss.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2daqktgoo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tofihhre.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwtbqqpv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2grbvbgju.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2nbcnmgtr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lsepbrvh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jzufoifm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dzsggacb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nnkaloyh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dgpnwwyc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hcmzsrmu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zhzqgtsa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mwkrpsot.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zohhcqmh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2nvwbsorg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xckrfici.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bmhxdher.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nntpoera.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qtdeezbk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2hdgvjqtw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dmiinlyv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rvnwsvuo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kdxcklrw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xtmrpbkc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ewpmltij.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2izagdzoi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qbqffyeh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hojjngot.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qqaalweu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eyzacevs.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sijhctwa.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pfjqzyce.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tphrfkis.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zommmtuo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fzcqyhvy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hnxgimup.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uqveeahj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxawfgmm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvighloj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2letqmaqd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2dttijyta.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ycganoiw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zeqfqyjq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bvcblqlj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpdtsmg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vitosqke.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2smidndko.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2baqjdawe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzxamwfr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eqddyjdy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bzhbaawm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uevezyzq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2aeiqqapr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojktouiz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2eayxyuof.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jsocczhg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rkwidwqi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2amwglcrs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2thpygodw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zblaeqym.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bluqogpj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uasrotxy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wpgemuvb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wexmquyy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fbczidax.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2exfnftbu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mbeamkpp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gtvljuek.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfgratp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ixutypms.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mzdstzza.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cymubnbo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2khichxat.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ppkikwmx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2adtgnnvh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2sqbjcaoh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wkddwszk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2elgdtwuy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kwbbsqgn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tjrkwugb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ulknjtjf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2witpugpi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ykudikqu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wofqdyjv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gqwaytmy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pqhwqhpe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2jwmqrlsh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fyvihzwi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rvebryna.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dgheztzi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aqgkrkty.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mhnkulir.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zszeuelh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2myoikwjg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2urhtuvwg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjozkrl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vwopfyco.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2udrqcwzg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xxzoblwn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2edxcmgzt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ueopvojx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2paownfjc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qvfvtjev.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rjqkrskp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mcmuassj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcwsetoo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vnyvyhms.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jdsciejg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ununwbol.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ilteuhoi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2jgxnkqqu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yaorfhvp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2onlmrhwg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2skoxywsp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qkdqydyc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zavfhyff.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2joqxdcdj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edjtchdu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjqlvjuf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykormgjj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fwearcgl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pmsnhgsn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2fzouymjx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ydaxytbv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmiequvg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gseqvplx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vyazqxxe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2crptabum.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vdahcaxh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qtooemog.html


<!-- 参考信息 -->