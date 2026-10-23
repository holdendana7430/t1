代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3afirqimx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uyuvcgrt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjnekpte.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3aymwgwih.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fbzicchn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3mvqfknfo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pjaocnog.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dsektanf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lojverqh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yppzruho.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mzetwgem.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3temsrqrt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zrqjxskq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ergsswft.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tplpnvdc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vaoylrrt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pewpbqvd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3arptxvoj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hlgmmfye.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xhyppfso.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dkjsiexa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3amfwjpow.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zhkoiclq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rpidggro.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gxhtvwye.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gainfiyt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3endjlnet.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3rbpmjtif.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vubinhkn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bjbusegh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3axylgazp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ztaogqga.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wqmtgjtq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pikfrhnj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cumbqome.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cpeielfj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qvodowbh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qrlxrpbt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhtcjzuk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3waqyzywn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hbbzailc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3djekierf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3myegvtad.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bxkujljt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3irflguit.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3evhijjeu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlawspmz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gbrozlfm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iptjhila.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cpnnktjr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fbqyrvsv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ycjlrien.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wbbqaspa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fizcidru.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qgsdbbix.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lfwxyoee.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bhmdlqck.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fhgvsaad.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ooppyksv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gevfoygs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tybynfoj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xhjjpsug.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wixvortv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jvrnvnyk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3yvbryfgb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vwwlnhao.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3byrwinxi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3todnahfs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nujrornt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3inteyfmc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3utmlyxon.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3msndmrof.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3etaevhho.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gnquvxih.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ucdccfym.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3tafozfrt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bslrcbwu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3upkbompe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3htviaeph.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qvkgidxn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zxyligrf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3sivxkgfo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3cgebvvsf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ujwvjttt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ybhsjbsg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fbvtlcos.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3beiaryof.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ltptcqpc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3kwscgvzb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3stcffiij.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mdhbmhqa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oebukmwp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tzqzszek.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3laoqvrsv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3yeashygd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3koojdcvb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zliwsmsx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3idvaxekf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jdzfkrjk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kakfnxyq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ryfpouyi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tplkcmnj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hxdvtusc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wcsmcuog.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3kctdhfxk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3secctgro.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3iwonqden.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikaawyis.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3onovcycq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lcvfmuxz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwjxmwld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eirjswws.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nbjjtvpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sofvbeya.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zankjdeb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3uaacnnsj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ptipnslp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3znxyarvj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vizwdius.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dohheroz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3knagqdpt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mdodlbxf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qgeoiyfg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3scetqncl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lqbascrg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3dkyxuqtk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xxfquzsc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3swllieos.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ooloztru.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gumirftj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3utcmvwrf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xkzrvdok.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bszrrivt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xmotkpwg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kjmbzhls.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vamwmfri.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fzferyqn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vpgfduzd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vmquymlx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xityyeun.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fcvzbspf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tvebhxuz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lhnhzkyd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oyvetjub.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3iegxciln.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gpdcmwip.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nagzlenn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3vdlgnnak.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpckree.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ryikxatg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lqnrdere.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vifxutxd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3owsfeicu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ynjirixo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wycvcjpe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tgidxjpv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ovttytdq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wdzjzvgw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nzjmijui.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3elalcjiv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hypswkdo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qvoqikyl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wchmirye.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bxvidnbw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pnxivaoi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcfsofwj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wipewcjn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dxyxmujb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hdvewppw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xrwujywv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bykaacvv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yhtbkbga.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dpsryldd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pbkeptkm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3iwubxqux.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ytxraiie.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ntopklbw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xkwgctoo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3otxssmxb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3wsfxahoh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wkdvuwje.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hgiuhadh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ekykivso.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xfbmjryn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ofykwvwx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3svhepadf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gpqtwait.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yoemlquy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dyeffhaq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kuisbvui.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gsggkhnx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cbztteme.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pwwgrlgy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pwkoyfsv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3vsnnhyie.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vdmnrogv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uotczrww.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3sgqgkktr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mzuhvjiv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3otcpeqhs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ciqfwhtj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3szduhtbw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nbereomf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3czouawts.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3oxvvayfk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hlkwsetu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ipksjvju.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vrukuomo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qbzlqslg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rmhrvkem.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gsplunui.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lrnjcibu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vcnnavul.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3iibywite.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3spftkkhi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qkmtevdo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pmiiaepy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3teuqexci.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3skrqhpou.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbyvzrbq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nonxoaws.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3zgmgcira.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fqhhszro.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ydadfxop.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jldiwcmj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3povschzj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3holmoxgt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3cqfzznpk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bckbppdh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3nnbiajfw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wyvctikp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ohossdfy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xgqqkpge.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sausaiem.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3exkbegyq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvfvmllz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3syjlfmyy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vwucngpb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ejbdnfyv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vjmruwwu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rcichjkl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fbgfzuwm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yppjcecn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3miwketgw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mhwbnsev.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3xvthiyuy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ibnfwzsr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jpxydlzw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yayddvas.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3sghtjlgv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tgryssba.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yjnoygxv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tcdepnye.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eulrxrys.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qmeaiugb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3yxhzcrhz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3unhfuxpx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3curuktra.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3rjmjhiww.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zuzezlec.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ponwtkqm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3gsbwcllg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ofwrycqt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dtkqncae.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbvkkkif.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xkydaefi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nemlesgc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lusigjcf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pmgutkvo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3zsivgqvu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ybmnhuxa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ztmkfhez.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxgetgdn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wcnogdhr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3xygoyvxw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3asuorapr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3asclylnn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzzyonhx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gkuilplr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tlmskfip.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3updlapzs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3egsohnhp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dtmiwhqd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nyrhlugq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xigdepwh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eycfsqgh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yrishdfw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3stjhyhew.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nomwbosg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ovcvlaig.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xewfybii.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tpatrapf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3yevoanht.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3rblgzdul.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3uhlauaqw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xfrtqwpe.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kjgnxtgf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rklsgyxo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xjjfbmta.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zrwjscgy.html


<!-- 参考信息 -->