代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zzecyakf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ahkzhgaa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ptsowqgw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yplhtleu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qrqeqaid.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ctzlddew.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3addfsrhi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3twszabom.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3oaycbnwq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gznhzfyr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kunqeyvr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3osnbvzyc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3doqkczsw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3badtwoyd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3onazbimi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rmlucluz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3nkgisqmh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcdsdwtm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aafzmbod.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3yyexvlfs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3pdvmfpzv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3btiuttny.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oyqecydn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ifwhnrlu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3giortvdo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vuxyqhhl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hisopesx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qgcbeeut.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3asrvfbid.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3agtjtvwe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uswjhbxg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3juzwsyfe.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dkooirnn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fjmxywtm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ulgiazwg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tfaybgkc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fppsbvyj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gfsrqoaa.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pxkmumxc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3akvurpgp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zfanonyz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mkldcxus.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3yglqlehr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3srcxzxmk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3grcawjhe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vtqkpean.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xxuzngxc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3zivuncbt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3udxzfenk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fyeahsci.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3imvgyckx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wgpglres.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mqsuwplm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tlfvxsnd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hgkgsbmr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tudmlslr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3lixcrici.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rkabpfjl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bmqsubba.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3alviotdm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jghtepiq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqasjzdn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wzuogdih.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytkoklez.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hefjdmup.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wxvkdxgc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3khqdsftw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ipynhghj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ehimszcx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nwhugpio.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pywaocpd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ymqhivjn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgbbbbiw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gropnlex.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rigjnarm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tbtlfiop.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fxpxxdxp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3aieebkth.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qptsdzne.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3dejpugnu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvpuonac.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lsipruut.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kphivsqa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rfonjtuu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3gwjjrahd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qyeoztdc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3iujaznqh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cvdpbkug.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3gttdrvmi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3uxtwqjao.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cwacjbwt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pevvlcsl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ugkpohob.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3khnarbum.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lrhjwxhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogayytzu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zqbwlejg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvbxgqbx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3okeiljkb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tvdujabr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dtmyovvo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qijsdgpo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3joxquers.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3iieuswht.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ffxblqtl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mnmecgfa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jkkjucyr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wylcuatj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qnqqzqhb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ivrgznox.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qtoniaep.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rbmexvov.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3urycdxfn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lzeciqry.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ynwjtfqn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ftihanar.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yzttjbhs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3utchzvjh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ozhqtmml.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zaoahevd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eixyxjqc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cnvavkwk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mjmdtvip.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3auqbyygb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kuhdleek.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kzcsciwx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3exboeyhn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jumaassn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tipnkjoy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fyrcicci.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xrapihlq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lsfnpmsf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3iwrtnzce.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qcwsqkxl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3nkubfpuz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sihumtsh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yfzpcjcp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lryjtkxv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3paaijoft.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3micprybm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wmncxdef.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3frseuzzf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3onrdsyaz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fgbdxsaz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vsoimcnd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gdbwvaez.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wbkgtskz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vzhqfyio.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3njdomqxj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ttefcyzy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3iwwunxbq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3uhwezmnx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jzwfpttf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jfwlfmia.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aikjlguk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ythwlanr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jrostzdu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nstkwnqt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3jvnptwwz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gstxgxde.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3omfpatti.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3exhlrcbj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3apgkwhvt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bubkbmft.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3hevkladb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3zcnnigbp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3oedsseug.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fiadhtfk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jkfwihvr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hudqpzoc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ybdrilzc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3psxpzqoj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3eqqucseg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jurpumve.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jblvorls.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mywbnlix.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xiqyxrcs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gyifwlac.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3oykbcssm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dmdophng.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fifjnmui.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lgjozzfc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kvqphnnd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jmziaokn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3mgvqsosf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gqysdfxk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3hrbouwbu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fwnvistw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pmpyadtj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3uuuwvxux.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gtznqlfk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ckloyogt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ofdxdgdz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nmgzjxyj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dcakreaj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ytmqxkyp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ueajpetg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bwmmfzsu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lrulljdk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lfillkpr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mbiwphnk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzhtpibk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3umywegvv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnysclvr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jggtnuxx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wqzdvoin.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pxgtiicx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rftovoyn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xyvnlkqi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fdovvzgg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rynyottq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3giewbfjd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jsnirres.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hjuxmzvf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3veswmjmk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fvbhdulc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tkcyeair.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssehhznq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwxqchy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvmfagww.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cojdnwmu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vhqwxnvx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3plsobrsq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gmdwumfp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3iaduyjgv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3prqemlcj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3agderfxp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rypfcijz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ngsoxqdh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3juqtdsos.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bfoegmqo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ateicjak.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kvxicgwx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nipjpfsf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whtjmugv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3adgxeogz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tmboximj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uhhkmreb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qzlleyjb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xmhcdsyr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xmylrziv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vfgarnwx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wvwqmzwy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pefglpqw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mjkdiqdl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pvdzxizk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hiqnvwcs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jkpjnwnm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bovjyvjq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jsiupgeb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3tcusxrpr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3tysgcgab.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3oopfrtbi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pjnuhssv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qnkeyaya.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3letfthhk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3cxbtgxwg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yxdbbkag.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ftcukisk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3piuavytc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3owzqhxuk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3osblrjmm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3soomhhoe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3tsioqucy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3syszypse.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fgwmumvz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yxgmoyov.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zhwwdnne.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3agyuovri.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ofobecvb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vffalpkt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rhmcxrpy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ekkztasm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wzjtfude.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3itopicnp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3kbsdezpm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ummgswys.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hsuxktll.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nhtrnhpb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cacfjfgi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ambtbmim.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cucoyekd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcoxipld.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfoznrt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3idwihlpb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qgcbcqer.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uufjvzmn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gppngkua.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3cfjpztkm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3niyjtsus.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3itgrzkbu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3djclniah.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tgshwvnt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nqsbyten.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mgmthnyt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fhgkshfz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3sgpdwxyj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3onfwaheb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvqkkznx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3btxnaqsf.html


<!-- 参考信息 -->