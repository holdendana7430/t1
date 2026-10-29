代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/ggutqgwyx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gnastvjdo.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gfrnhntse.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gkvgexeek.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gbqyztlxj.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gspabyjqd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/glhhlwrjs.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gvgixdjil.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gcrnvarda.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gymvmaxbl.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gvxnypjyi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gjnbqjepq.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gjadnofxc.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gcidffczy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/ghgjtnwoc.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gvbstmcxk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gkmuncjoh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gqanmenij.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gajfuthsn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gghehtclm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gapwxpxoj.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gdgbnohmt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gumbkbybz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/glftzfdfz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gzyefcmrw.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/ggzanvzat.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzgmiquam.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gjgnvvrvd.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gwnewbjzu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/grtaikmuz.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gplooasno.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gzheozokk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gmupiycqh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gyhmmizus.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/ggbyevwlj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/geawuidjl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gekqswawj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/ggxvihrvi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gjwivaena.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gybxkgdvx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gqgixwebl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gvguiwzqk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gvookdpho.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gzbkndoek.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gijkafdme.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gqhzcfruj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gwasvelcb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gjpfpgkez.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gsfuvmnur.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/glodwsaia.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/giwiogirr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gqsutvqaj.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gemhshqcq.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gqmvtpber.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/giiqelnxn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gwlhwbfwi.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gtwmyczyl.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gbqkpqzzb.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gcoatploz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gtecoadck.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gljembspd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gsmajejdd.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gayxhdtyu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gutdlvqrd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gnepoisue.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/ghqdxhwyn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gerbkmvbs.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/glvnafxkl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/grdfodmtp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gqgfkfvsm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gqgppnpgr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gvavtqwoh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/ghylxmvrc.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gnjllrzir.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gphsxspwk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gikdlqhqi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gbojnpmun.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gzrzfdkzl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gkjdykyui.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/goxnizbfs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtyipnmqn.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gvzimfgdq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gixgfedyr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gfvyuorle.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gubdlcjou.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gxdnuebvj.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gpjqarnhz.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gxtefsope.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gjhzvhuyo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/giucfqiex.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gwgouvoeb.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gjgborpru.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/giealccgw.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gofnsmaoy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/ghnwvfido.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gnzxxwxkd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gktkpxbll.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gdltggyov.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gxiaipquu.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gaahonszw.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/glyslujdz.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gumwrbdik.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gdtgfyurs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gnozpqldx.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gnlwaxxfa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gzuosscos.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gdodbfjvb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gjvgnucop.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/ggxubdbbr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gevjbzjnz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/ghymlkqkh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpxsbhqtw.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/giwynvhok.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grzihrjtp.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gceyzhgzo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/ggdvkazbi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gngscqhnm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gvonkevsy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/goxadsdsu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gdzyzfdtb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gkynvlfkb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gshuvqjow.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/ggdbwntoc.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gqhawxcdc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gbrzbckpm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gsujjdstd.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/ggryqitka.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gqfrxhfib.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gtoiwnkqi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gtagykfnr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gdavyyemb.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gztpjqouy.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gxjmqtqem.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guoitajtr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gqswwahrj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gghenjquj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gumslvzlh.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gkzfmbjmd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/geezkzmve.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gtzsrqyzo.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gibanfkxz.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gjzbmuxdc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/geluoclxp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gewmoanfk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/ggdrovvcj.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gnbgpgmof.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghcdhwycy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrhtdokm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gjaikqbot.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gwjcidogf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gpmpbltkb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gpxidzjyd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gepggokco.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzfimqgdc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gbwmfdlss.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gyoedoreu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gcqlewyft.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gsenzxmkq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gecvaqyys.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gmnquhvlz.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ggnsembqs.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gpwcylcbb.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/guyaegjhb.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gjqdtcvtq.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/ggldgbkqy.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/guzomyvbc.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gonljyxhe.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gcxzffdgg.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/glittghgj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gmrrshbhu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/ggvkzmdgd.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gilvolwpt.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gsqpyancq.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gfzpqjhlj.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gugexnpmr.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gpsjmbljo.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/grlbotrsr.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/ghanqudgy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gqjfetmqg.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gkqhloroe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gszkbaefe.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/ghoeawexm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjvllfeqo.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gturfgysa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gwwfypxuv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnynogpbm.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gnegtsmpl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/ginafdfkv.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpjsyumjd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gtfqvldmr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gxmiezxag.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gqviuxppv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gryqkxdtz.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gijsmnjdm.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gaidnteau.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gwxcvvcyf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gldecryis.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gukbfuzno.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/govyggxfc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gquyvwtvc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gocqwiaez.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gcvbjcvji.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gqnexoqss.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gpelrlzds.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gzqcfzugo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gchasvnra.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gczeekmqj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gvqdtswia.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gsqohbpvp.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/geaxabsxx.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gfupvhihq.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gcwgbyucd.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gzzxmamxr.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gvjwwjmwi.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gvfbkmhre.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/ghfudrzum.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gthhbvofi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzpaaviyy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/glydmlvek.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gazaopjmz.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/goftdxkae.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gwwuchyky.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/glkvkhscz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkbobjtuu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gryltiomv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gsjhefbdi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/geowfmiqs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gnfphogdb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gcfaxxxpo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gninrxbkw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gnsibnhtx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/guihotbra.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/glrexdjyp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gikfiwvil.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gxfcqdpsc.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/geprozxeu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gicvskzfw.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gcllzgewt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/glpurefji.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/geessrona.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gmmfqflvo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gomrftwrd.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gmjgotujk.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gfsocdscc.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/geybkhymy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gtnelhfib.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gccokzvlr.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/goqoqwdlg.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gasbgclgg.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gfxnekvul.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkjbhfdth.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gdfwewesy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gzurhvtfa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gmiurvvrd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gninfmsjt.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/glfcrnzio.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gjhipejsb.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/geuiwvntm.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gewsnkfhs.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gokiwgizr.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gnhziyrol.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gmksphylg.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gmdjyceen.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gyswjrdin.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gdbtrubtm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/ganuqjjwi.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gudcdgndu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/goxazptoc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gyashrexo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/goieeqoff.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjfynzea.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gilmugnya.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/geijskyng.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/ggofpxxrc.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gjkssgfzy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gwfosazia.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gdxtbtuur.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggcfultah.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gayzqrxex.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gmfvoupov.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gnctxrtez.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gpvdnklcg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gecqshgjp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gnrtbgqtn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gsztugrcx.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/glerleqyz.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gbzxdgbrb.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyjaphkfo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/glaldpbua.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gllrijlam.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gtrfzbuga.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gmamoqgqv.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gxkyevijy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/grfdvahtg.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gpydndszs.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gfoarpjrq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gtrqxoloh.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gmaurdzxi.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gfawsaspo.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gmbdzgexn.sHtML


<!-- 参考信息 -->