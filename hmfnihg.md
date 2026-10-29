代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/ggtcaixwh.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/geiotclwc.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gkaxggjdg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gpvfluhxj.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gjlkmidqm.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gavwcxllb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gszdoyoeh.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gsstnayxz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gipipwrnz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gsazzcdhi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gzimqjwfj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gsrrtvqoi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/ggpwqjuvc.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gcvmstrxf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gogwfkzbx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/ghxzbgtqi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gkdlecprj.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gqcivacfx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsagwobic.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gerxfmaqb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/ghgoehmcp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gwihqtlwe.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gppesrahv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gslbmbxef.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gfdmxafpc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gmzlqlrvn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gzizkmqli.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/glnuiunjg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gdyfqgptf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gdocaptkp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gjremozpj.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gjpwjunih.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gimeikucw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gkfegsdlm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/grjfgvpxm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gjcgvqtgt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gcgnzfcea.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gtsyvliso.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/geampwggy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/ggowkldbw.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gqmxheeqe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gzkyypsmi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gdjtgtiao.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gumrkogcy.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/grgepfdrm.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/grimuudxu.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/garefdnwl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gofmkwmhs.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gvvwjumtp.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gighkshel.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/ggppqomcc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/glownvytr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/geynbkpql.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gqwazmmpe.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/grsoovwnm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gqknlljoy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gzieqqwrj.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gzihwpjyc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gamxqfqwq.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gtpfabhyc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gjueszciy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gozfbdndm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gkvwwalpe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gchdbqksq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gpkzvvuad.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/grrfisjio.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gsspyznjg.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gjkljwtnr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gpjushurx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grokjfnvm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gosinvrwv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvlhwnrln.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gjdsjxyti.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/ggnngzbvo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gvomirejy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gujkjzdyq.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gzefdgjgz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gnerayssv.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gswnmqfvp.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gexbkxdhf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gimdsenen.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gcaagqxhv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/geoemxomb.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gbthluxyc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gbmrfpngb.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/ggxvhrzsg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gwjvzdiuu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gaggkultj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/ganablkbx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gnmurqkdj.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gkjllijyz.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gnwngtjrd.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gvdultxvr.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gpaydvvzk.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gcevdgnaf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gcyeawuxn.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gutwxrlyw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gckoxzsub.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gmjzyakfp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gitsvyhdz.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gqigczjro.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmloaylui.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gzuluerbj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grcbzufbu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gbrchsrxp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grajdwpkh.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzzqjleih.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gxowjquva.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gsshegnni.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gvsfyqidp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gyzpfuvsz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gvgxuozxe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gpizyudbi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gisyqwywc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gguqvneui.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gdjnkkzlp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/glphdhdzz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gbfxjhmds.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gwoidmder.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gmsbnnnju.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gdxiqdldf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gpevpywvn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gfjliiwox.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gekdcpnpp.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gqpdlrnjc.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gnlvndejr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gwcowdtuo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gpblznscm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gygrghzan.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gdkmbxoaq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gnaiksqzu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gttxroyqs.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkfldfjds.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/guznvkybx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gltniqkxx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/glejzieac.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gbgpzmghh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gahuhxrsc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gcmqjbgeg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/ghyhglzri.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/giovtevcf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gadtveoee.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gvegxwvtu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gbktrcndd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gfohcyukm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gjmqmasgw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/goaubwbnm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gvaolxeln.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gcyqtsxqk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gduwvwjyg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/grbszcsvt.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/glwstotym.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gnswwtmrw.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbdlsgykn.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/grsuoefti.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gyergknvx.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gwadxtpzl.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gkbvhvmsr.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gseizlhwv.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gwxdqorlr.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gsuazyknt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gssqgefwe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gbytjdiuy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/grrcptjrw.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gcaggoufs.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gxkazlvtc.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/glstctpgq.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gzwgnrwdg.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gdchuujvi.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gwfxulkoc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxivllhj.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gvpuohinf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gpaeaetnw.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gbyovisxs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/ghhdetlhn.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/ggvoevgme.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbevwxjo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gtogdzfhl.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gaaikoaqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gnqdaoecl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gidivezue.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gbifqvjgs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gueyxiczx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/ghokutsnl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjppuqnpt.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/grgldxife.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gaksucfce.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gbwzumvie.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gvspxkaue.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gygcpwfhr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gbcwwcwxe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ggyrholap.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gaibqzyrr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gadtdayvd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gyllkqkla.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gkuggjnmi.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gkhcobjbu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/glissigtr.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gpahhymqk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/glxopigod.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gsaaamdho.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gzwvbgbji.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfrqjccfi.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gtfdxcoxu.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gxscbhrqr.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gdphfnyak.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gppjdrkwc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuktvdik.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gnwuwvebe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gcveajdmt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gxdzxtuyl.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gimpwbsve.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gzvxopjat.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gzcvbroxe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gwahbqxpe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gqczuvhqf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gkzlfwpfn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gaioxuyyp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gufwcdcdi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/ghzulhivk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gocrqzija.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmevtvuog.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gxzjlqefx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gqylevhdr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gdywbxgoa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsgyrtnmv.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gorzbvcdy.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gncpyfqax.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gwfovtimf.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gnkhmnxdp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gynzlbidj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gclzwkeqb.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gdqctbkjy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/glxneubkc.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/ggdxgabkv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gngxovgak.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gabchklix.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gwwxhufju.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gvugzqlxu.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gyaozhckp.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gafdpldeg.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gzovbexkh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gfybmysij.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gbqnmgemx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/ghbkjyonq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtloydquc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gllhpbwgk.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/ghadmxuqq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gqwtdopuu.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gkwfkbwif.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gnvrbfysy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gopgvvbkz.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gyelflhso.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gvgrklubs.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gwmatknxa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvjahtdyd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gzhktpwwm.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gmvrbjuhj.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gdqopbclk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gfhjzysvu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/ghbcfjdhp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gxzkhvghd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gbqziitzg.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gnhfnkbde.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/ghmmycawt.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gahekzqhs.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gmlrpcmsf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gvinslblz.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gnumdoznc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gupdeitrm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gvvbomwfj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gixlvjshi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gyccshojm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gmpznoxkq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gzmqkaexf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gdglkkfqr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gbyzevpjr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gjoilrtof.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqkmgcxme.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdgneinhi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gpqkdgpcf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gpvgxnxfd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gfvopidzz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gcmwkfyzf.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/grlucsjzi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/ggfjkosty.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/garunfyic.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gfzfbldvw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gvxkjkrrt.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gatfbqplx.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/grrvwrzkl.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gjngurijn.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gqbyoblex.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gtgfhvyei.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/giupmzozk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gnvjmdftk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghyrgiczr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gccrthpma.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gqevggjdw.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/genvtkdhw.sHtML


<!-- 参考信息 -->