代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ezzmdmdj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hcgafbhe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hfeyqhgy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2odlcyuae.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gcpdsgcw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2syppacov.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2jqbpyffk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xqvagate.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2pdbahpbn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2giykxuis.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqvhikc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jujuyfyr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2smzwcpaw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ldzqkdma.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zvzjqzlv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qmaeruay.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gafwdkpb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhlrohcq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bhlpdfoz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2etnzwwuc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uflgxfhd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2iqvfmfjh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvozpjrz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yghjyhcp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lieozlox.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2asrmjesx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2yzojmnik.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mvdbkmup.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2viuaxwdf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ugnmqkrn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2afgrbbhp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2lggorlpk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2plhzgxcr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2tsvojhpk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gyjiupmw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2iicjouog.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rtadedjv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2wybscbsp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wylmwspw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nrvlessy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2cchpupay.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dabwhwpy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ixtnfahu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vvtkbqgm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2oaprydxf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ctzbskmp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zmusgact.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2pdcyfgli.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2razjrmtb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2iawjjrnw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tysxztwl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2baaomrlf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2swrhyutx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uggsdoon.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xgzteubg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifxkuzbt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cqdukuvu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2asqtjjyx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2aomcqswm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2aubvavom.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2brfkodkv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2yfwfhavb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aknawqfy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nlfcynty.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcegdmci.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2njmmcqmf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2agfzxszy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2plheqlcg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2czcnikcl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2draijuqq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gxyhbrma.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2luuzaqwk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjyozuoc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsxkjojl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2giwqleqg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lhiunjyu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jyxpopln.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ujyrdaft.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2eykgkdvx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lsxhptab.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2eiuihjjs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2oclnvxny.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jakczehy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqobsxvi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ylcpderg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bfdbipeg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itljxhgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijokkqjh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2sqoxweuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdwqmizk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gtgjmqxy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2kzfjoyze.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mcpoynvz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bxyitndi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wzbsfifg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nfjujpvo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dqneuxmu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ejsdmvhu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2vgwmejto.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dpaupdqp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hhavziqu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wgraknqv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wphatsnf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wovcwtsq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xmedzaxa.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mewgnfvq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ahddksfs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xxjdfuec.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rnvwycwq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gevovamg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ihwenvhn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rvjgtaci.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2plhyqfol.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2izxfdlcy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtgbjht.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbffqhn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gjimkaof.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wyuxvroc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qnxoesqt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lehzuhjx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uxmuqyax.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2smxldghi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kbtaxhho.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uiotbmds.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lwauevuo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2yvwxabzw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2tboqkbho.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vtxwhykv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fsbvwadc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cftowosi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ewtqkcvv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vzidfdam.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zfiivmym.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pcebvcdm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lqpnisci.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jmihveuk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dvnuoprl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xjldugov.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fnqntqju.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rcbymupd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2kzdfvklb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rdfbdxxp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wxrhskvh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2twawfwkq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ssvdimih.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sphnxizm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lqeykygf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pugxbnma.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qhocsjre.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qgjmizji.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ddcwtnus.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qipdbjlw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2thispizj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ertbmgwz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vegkpjgt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bdgzeave.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2prmvjlmr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nzwknopa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rlxfvvcv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kebcsuyc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2byjqsjrj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yuwebxhy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mbhjzcqc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kwbdnrjc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ufpkupas.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kqlinfgm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ifgakvgm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hlgbggtt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2woojlrqu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gycxumaq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ahtnrqjp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ogegzwge.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2usdoqnhl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ksbapmpy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qtjtbmja.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ltltzswp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2coavnznp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kfilyums.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ymoupmbj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zzzzfugc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wftppxtp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nucqhxxe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yorjetoa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fgkdrhnj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rfaybdcs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cgbrldsu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xfdjxlrh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ilzomkbw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hayjccal.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2iqeevveq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xmupxzqa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tzakurvr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ipszkfmf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yjfgenfn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2awxuhavm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wyykuela.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xepkdddg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kjuczduj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jbibblrb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2umigflmx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2asbnvdzq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2modhmgew.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zsgmugxd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rhjdlirm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pgrgdajr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ntffcyeg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zpmneovo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2uzmxynpa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zorqymjj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fwjhvzqc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2prpyunzr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnyyyaj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzotusig.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ksxrpekl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ozbybpwf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2snkjogtz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yrrmpreg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jpyevqpz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2cmviwzlg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cgewzxtz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nhrbznnu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2sojejmfe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2btvnsclg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2txigmeja.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lrfuctbi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2maduaoga.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tomstmgb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2awitqnyj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mmylstjh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ntgzosml.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jviqjagw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yccwtuyo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2aymsldbx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xbigwhsd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mcrnipgr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjchjrh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vxcilsii.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wjnjjxuc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ujtaknwp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2gsabgumm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqvqdpjn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gxoeeoaq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2broklere.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2wekomcjm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vwbitxnb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wdmnyzpe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2eqrjygai.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uzwbzqzk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2irgcqwjn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2szacnykx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rsjkxfon.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hkddapvi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2aahgodjd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsamubae.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cgqcguiz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ptpxxfmg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zwphadtr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2adpgbmrk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ghjzmfcf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gtgwijwx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2yogdkaiz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vcxtvseh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vgbvccbr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wurzfkju.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jsnvmuhu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rezcnelt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yvomkleg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dfssidwf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ignzqzaw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zlflewaf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yoqdokqt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2duzhgsvq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cutpkvqj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ckntonrw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aykhmtpw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wthdxzky.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycswuese.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xinbkndm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvcbbvpi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2sxiwyuyp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ebdtujfd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qlhguisv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2otqmxycg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yvatjxhk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ufqihnqr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vfzrnral.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2huvoqgee.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wvqrahtj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ljnlfziu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qjllibqc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qzqkajrl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rxrbripq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2utfuavxg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mkvoboin.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cfwdbopk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2iitodfmk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qziaudim.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2neyjnjqw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zzhecnkw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2naexaloj.html


<!-- 参考信息 -->