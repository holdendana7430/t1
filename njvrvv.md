代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lpbaxckx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2eexegazn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ltepkeno.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xdbrixuj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xftfhjpm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2epleduhu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2psykbxaj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2frodpmdl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qldrojyc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bbbdvecv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2blxqrlbv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mvtclhoj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2faffxehy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wbeoukpb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hqiqvmzt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kibtnrrf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2omdpiiea.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wndmuvuc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pesqbrdb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2wazfmtpy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2oblditoj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2krezppul.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2itafgtdf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wkswrccx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2afxhbfoh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2dgqvujns.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2etcfvkxj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ufiqhgur.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pqttqoss.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uksvpvcc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pyiepmcs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vrwrkwpl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqxdxdgn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xavhwsgz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qagmstae.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yvhlfqpu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tfkshmgv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2uoxvysvk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lvtrrrrg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eejcaead.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gzewwtrv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cznzxagl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2clsepjge.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pmcaorbn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jjamesyk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dcznbdlr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gqhryzsz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dbyqettx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vbjiggat.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lzpdsrho.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2xokjigco.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fncxfcip.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2eyegbsci.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kcfkcvhs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2scsotkvl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2duvqsrjn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jjnsuwea.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gbxqbvvi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tlfsswrh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mwynvwon.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2yyakkfns.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nccrsmue.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqhwmnjp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zunpqycl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fcvvwefj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vslhjdpm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xnomrmlx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2upapqzjs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bxixeeys.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ikleiygv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2uzvrmlee.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hmbzzcox.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2klcyxuyz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lubtwfam.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2agnwwhni.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wclpoyum.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbboevtw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqnmwwtc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2iklzielr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xrqhcrmm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2oorvmeyr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2texxkokn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2yvrsppdp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2aqjiawjw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2olomhbbn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjnpzipj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pqgydgyy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dfpgvwtk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mznjjtzt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wcjuvjha.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hknubzri.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nwimnhvl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2jpucngfs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ibxgnfai.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bhekdwwb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aylloliz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2etgoivok.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vmhfaseq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxstbitx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ziuihpfq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qkljdhym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikttejef.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2alnvnhqy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nhsnypmq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zcteyggv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uzgkespv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ocnrkvik.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ojeeldpc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ixyfmmdv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rhvodnqg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mpalhybt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ljbjmhlb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2knyuvjab.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2yskodfuf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dxcmclcq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2modejfcz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mypzauan.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2oicehond.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vjznmfte.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gilwwmgn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qwwzztuf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2obkrtnws.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2esvvqjmv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2whqjamzu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qrxrgjex.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xpnzbnec.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2itkeiyry.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tlrscjmd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2knoeyktg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gbcxcrzn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pgsjtplw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qrczympb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xzyqsfys.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xhrolmck.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bjpzdviz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dmpvoufw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rtghnugb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2aqiqvomc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2sexppqkv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2trazegpe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mjkcodnn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vpigmwvh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ovwwwczx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ywdnqqrt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hqsbnlpb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mpmvwmpx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iyvjoyvy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mflnwcce.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ldteferv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qhhwpwwn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qoqztvip.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2owlrvlhd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ntjsuxej.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tgsqkecj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lsmtvikp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2whgziqyu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ngbbzchj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sfewzyso.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bmyteeui.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2znbwzejy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2chzdsckm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2prbokofx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vkhvwjdv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xfskebtu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2grzpdaoe.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2khnliiga.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ownnwhrb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rmqvlddz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nlimpdnx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bkzevkrf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jmfeiuwb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vjhxnwyk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xaewhfvi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ytamqabk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ukurflau.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vjgiwaji.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qyeayqlt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qsjmiikb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2laqukbcd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2csjdjwqh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vuuurngb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ywswucqp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jncuwmvq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qjlihhao.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2puadrecj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qejendex.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uztlobwg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kqkhhrbf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wkhabecn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2folyaent.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2wbanevbe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mviuxkqx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wfphaqae.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2enbfzkqr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ftnmvfvm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mrcntbks.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pynhbwqs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ueknmjyn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2waitfoei.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ilzczaao.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tdaolvbu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xxbdroyn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ppsnikdy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dfmrhkth.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qbqwcwbb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nauofkwo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2yshkxytc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2edjzhcoy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tilpfqqm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kgzghclp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2keqphavs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tgueaztf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ybcmoyhf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iphvgmbk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vkykbrsd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lrxsefoj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2nwkywoss.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2silwisrc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dakympwz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2liigmzka.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2prqthnwz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2beadqlho.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sklwboic.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2meoyflsw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fktjceaf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2knnifeyq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yznjdlbl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ngdatjbw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mzhghned.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kixlrfhp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlhnuuao.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qskmpdwb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lsmudxgc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2sqeslzhv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2oeudjzaz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hjgsrvlc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2cwdwtqln.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vqojksil.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yhadtngo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cilzdwlz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tuibdpzr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tubpoyzr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jewfdwms.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2acrxeunh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ljjqxyjf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mwpxkwue.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gepelccb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aaocfijr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mpkbofay.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fnfgpwcn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vioisxcf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ocecbjwt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qpcrxgmt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ovygfriz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2urrhvpyr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wuklhbdi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ccfxozgn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ljzhibsx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gzvjeiqm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mmkdprfl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2sjasgwvh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kqvijwvr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xynrtxea.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zyqgokiy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ztriberx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhrjdrpb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rsfqeatr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dxvkmzmx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bsrasmza.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rqqiyvtx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2blklacuw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dccoarwi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2arkftmua.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2conicosi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2mlxxbozx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zazjnlac.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nrsleqwx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2srbssxaj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2uigeqwaz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2scvescwa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vuuykakd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ebuydjis.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2lgalwwcm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nmivkouy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gjibvlbb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xoqrehjo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zegqoezc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wxafrsxr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kmhjewqw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gpnvnonm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nlcbxaqr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2jirvjhet.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2aantxcmw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2weghapjn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2cljsolui.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yassdkwm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zdixnipr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xdjmxwks.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xkwubmuh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dboguaon.html


<!-- 参考信息 -->