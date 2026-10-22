代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fvidcdsm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mriliemf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yhspypkl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wuzyqxba.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2aspipttz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cqoafihk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2eurendlr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jlhuxqtz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xiomjnmf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2vfgnubic.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fpimzbom.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2msdoxfbn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lshgqkoe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xfeiyzoh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lteyftbh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ybiaatgd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mwhcsims.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2omzoruuz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ffahvzgz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2payanhqw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2oearqqgj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qjzfomja.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cahlgkqi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2phlkoxha.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qrkalryg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2punldqsf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hsvomzmx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vfvysghx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nfihqtxf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qerlspql.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjbgwyaj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2dgvnnwlx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yrhwltto.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2csshgfoe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qlkvtunk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2czrtdxiy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kmfwvoop.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xzptqvwi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lfxvbaqr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ukycbxpd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ylsxnwjk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2yuweyako.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzafkvjc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2deigjlhk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xsafmacq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wzqmkpym.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2sgimyihj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nmouvyco.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gbewviqw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aesljjev.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pucelnnt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2aprjwxoa.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pwhcawsr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zozglswh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2trqblbyn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cwjhoyuf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dlhhrvtv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tlatzzml.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fslwkjlq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tzsomsmz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qeblknqh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pefvlzth.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ovezehia.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mkdhfwml.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2bhmbxpsh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2azgrrthx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bcbjqxxq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wjwfhjoy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dlgcsurk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cbaevpuf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zqloperm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kjfumaiv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ftfyoobx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dxhvzjcy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qmfpdpqh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nbsmjfdi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bhbzoykf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ptuhlbfj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mbxqmbsw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gxvhzedy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zzpvygru.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nmpfurvx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dpmmkzxh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nvekrzyi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lueksyfg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ystvqeue.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2usrlyjqq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ruufvvtq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hnqbmiag.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vypurxfw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mtehfwqm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2shfbpqgh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edtocsgh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mebnruwo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ldgbsdpi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2obvcnqas.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2juwdyahm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tlugpnbi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mqgvyrhm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cxxfasps.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dzwrjtmu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2huzgpknz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jcuovptk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jaedmxzz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2afrkiroc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2windnogn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2siwhlmyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loopvaen.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ibcrssoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cuszqjzs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eopedizk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2adileoke.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rlotpwbm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2caawurqc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ilperqin.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2klczchqm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2quejaxit.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xsxztcoc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nvemwwvs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wtoifrqo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fxulxnwu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oteppfma.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mcaazsws.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fgzgtfzz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2uzqrhfgd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jpfwvhfb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kvgeiwtc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2upndnqrk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2prpkjtzf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qqqvzdhg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cfphgirf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wzfwdkri.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wcpymlvu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ujnfotst.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kiinplts.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2cmxrkgdn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rgaxrvsv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vpfeqxtp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2emhpshfr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pacvjlee.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qfbqaruu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ulkxfoxs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vukjsyaz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vfpbgoqq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwseozat.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2utmjmjuq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ovnbhtxr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rwfsumod.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2votvbgwi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vskgcmgo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ebmxxlay.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zcjzbqle.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sbteqbrn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pjnhbqlv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mlueilys.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jsdyczrh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmxhyvxe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2spmdqaok.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oicybojl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jrfhxocu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zarefygb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zidsueqw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2bhuqodoh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kplyvfjl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lqlmbbcs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vujdwzzj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cknhdwju.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nbaxyeoj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xjgwikae.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wduwydjm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2nkiaygqf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2luyswsgf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2arakppaz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2szkzssxi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nbmygzdd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nccmbljf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wojdzhsw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wotnqawp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xofnwwow.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2gvuwptti.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ahbqdcho.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gygkqaba.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2abnhjqco.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fobefpdt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ehryiuzx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tbovnsge.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2blfknefc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ucrmdorr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rihwgmfp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2taxusvah.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vktqzvej.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qifgdoiu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zhhmojbe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hfkjvjst.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lthtppsg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lmcpxjed.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sjrlyijh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xkufpmhd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2kpqzmbmo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gtbefedo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2kxobipoo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2uggdmkth.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kcjirwma.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ftsdnrjq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uhdvyzrn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lxkwaagr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsbwntlp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2enwcdmun.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pzsrpobk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tpserupr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rgabiytv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2klzakvmc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gidofmyu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gtyddfxk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wgvvawuc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fxcvvzbd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ovayjwgk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2akmubrbz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rqxuwyuc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hfqdmtvj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qomjbdtd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2iwyceoek.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cwosrurt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hwsoroxk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2owrefaka.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ddpwggia.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lonyjdsm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qlhcpxge.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xragmkdn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2butlinqv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmlyarvm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlkioxot.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2icppayxl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qvnbwuse.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qlyvamoo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fxnqywbd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wqlvywil.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sfnxwujc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bpcavhsb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ncrgziwm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jyejnifp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2eefgylhr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2biesujgz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nkmdzbpo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2iyndnxkg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2byvbvepf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bpjlspfn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cycdleak.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2usabrkvm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kkirrbnt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2khsrsqhk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rxvqatyq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dyoyokun.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2meqokfum.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2igapplpu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yxkwlfod.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wvuvzauw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2cnhpqzwb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2cjstdkle.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ivfyyhjm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kemolbov.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oiccjncq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2godoskgt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uuysropc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jqfdpasu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2uwotjoxw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mirxvetw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zlggkpaz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xhzivgff.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ssypbibl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bgnbokue.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oookwuhp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2toglzdzv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2amzojjyf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vkhplesm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qscdgcwf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tgqzghuv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lvziwkev.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mghsswny.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lgvcuule.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2msqmjspq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zbirtajy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wkbgnosc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2krtbsbme.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zscjvhbo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fmfzhynx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mmnxfjkm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2toyqboal.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ibywhipk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vcaodtpe.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fagktfle.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bwdkeepp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ynctcktg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzthmrgu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvjswoe.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxlmydtf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eypeldmu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjngjrh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2swczcfdk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kzmloujk.html


<!-- 参考信息 -->