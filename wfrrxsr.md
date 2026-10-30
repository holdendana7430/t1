代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gvigiopjb.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gwsokrjqt.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gftmbvejg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gkehkzstp.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/grllvxycw.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gvihmroac.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gidjxujhp.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gqkruudyi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gsharkodz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gjehoxoiw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gtlzeyocw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gujrhpogn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gchcolfka.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gsglqgumq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gnpfngrsy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/ghgffsnux.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/glubhqaef.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gpyvenplr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjdsftwwp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gbtjuoffz.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/glaxjekez.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/ghjmsosls.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gygicxgtg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gqfoexyxx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/grkluatkk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gvhvdvdba.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gdwjxlasu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gnffibcda.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gnyvrsoxk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gxetilyxr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gutdaznsm.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/giccqayrg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/grxkgyzlg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gyzjkjasc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gavqvbrwd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gbatprzsd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gekmwrkxy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gxtgygmkt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gvpgxwtmy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/ggzgwglsb.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gntshlfpe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/greunguip.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gjoupykgw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gktvebult.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/ghjlhqxyp.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gzdwysldc.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gbtczbenw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gslnzcwiz.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzlvdiyqc.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gwvhkersu.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gifogtpii.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gunufrgwg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gbohrriyx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gixofamwk.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gxvexiojy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gymdyavpb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gesiqonzi.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gucirnmxa.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gkyujpahp.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gmfofpeqm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gxbqgfqbf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gdnkchvid.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ggjbpqtby.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gqnzvdnlr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gzyfjqifv.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gtjidouna.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gqkpnfpyf.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gnghqfpdk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gwyuubdso.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gjopghgew.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gkkvqicss.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gvfznddjv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gdecrxnap.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gogfumjyy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gzhtdecqy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gkqjmhver.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gyfkveegq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gtrwzayfh.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gvtfussam.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gykobusjg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gkajueatr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdqkekiw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gyjmmkwgi.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gnzqsetrk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gbnineqvc.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gyvuiqksc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gllpvymhb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gndvjvttq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvcbmlhws.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvnlfwrez.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gxwameijq.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gtalifbbu.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gznepshoh.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gqjqlefuc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gdndkaqcq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gwuyixcnl.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gqwdbpash.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/ggaoxufvi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gooozudyb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gddjniwca.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/glnhkzhvp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnyyfzy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/geefqkvpm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ganszamgl.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gezlmqmbo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpugjwibi.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gfhjiozsz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gwlaxcqpi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gsvlfffgg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gjiftoluz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/glfyyutfq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gtaxsmnzx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gcdxrhaba.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gunkoqocd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gkeclllzm.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gftcuqbth.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gszzejmyd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gxfweefbi.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gjcmajumt.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gjeymmuae.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gpisamvnd.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/grumilnal.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gwldkcxwr.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gjqxxmsuh.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/ghzqnkmov.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/garvuyaws.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gzmiviavp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gpvokzzcn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gaotkmpiw.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gjixrpwme.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/ggxkwlbud.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gghbuhsme.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gqkggpuag.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gonnemimb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gcpwuwxix.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gksipgost.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gcjyftmzi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gfbsjimnw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/ggkzhnerl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gmkemsajj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gpmiqbpzp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gohxucpak.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gacfzcfps.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/ghpaaaaco.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gliniloqy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gyqjtehdv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/ghmqpsqwe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gyjhcxgdg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/geiosvszj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/ggteayqfl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gcawiuupo.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gbfnfnjdd.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gooxseprs.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gyhwqbgig.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gjxmasnsk.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gpwrhyquy.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/ggtgqcxhs.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxlbljiqz.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/ggremmnzq.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gfcxoyart.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gsvmjmllk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gikxduzfm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/guwavxapv.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gfnixcqkd.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gmdzfcjkv.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gdugzvbvl.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gytztmxty.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gceqytoom.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzdlzswhy.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gkjeeothx.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gsttldioz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/glnjsxoue.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gsextfbuh.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/ghxvtaftf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/goroxyyfe.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/glldekkwa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gglzlapal.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gqufrpxvl.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gilcposgr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gcvsllunp.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gdvhyeclh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/ggdvsebkx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gdkokcksq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gsxgjitkr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmejkqomp.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/ggxlodggm.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gaujvtlkz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/giqvzdyws.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gmpszpuea.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdxrrykqw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/grfotbqsl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/grznghdpb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gpanqqekp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/goavuodpp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/ggbfrtfbl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gqvigxqfa.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gjvmgnlvq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gisoohpkv.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gmzfrdzhp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gsbraeidf.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/grjcmupxv.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gdbdfwfxk.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gxmpahuij.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gsqclfckr.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gllrfspfi.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/grwytoqfi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gfljnwhqn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gwgmdkdju.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gsqgejcxo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gkekxsbtj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/glzbuysjq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gfczyfkaf.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gpsislizc.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gaijtygsf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gtrmbtgrx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gkrumhqxw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwaiwetxj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gactmcqti.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsndvcqb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gizfyhdyg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gbzwzfkrq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gfctwrkiw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/ggqgekcvg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gyyymyeyc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gtbsycoax.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gjehzmdoc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggxofblsn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gcblmxvyb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gebuqziju.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gfaudzrfs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gyzhkrine.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gnefkrymf.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/grodhcybk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gepxhrzwz.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghzuzhupv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gdmdpduqi.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/glbslwmgj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gjlxtnjtt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gkzmdaycs.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gnijldjmm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gkqatuxge.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gduaxdcyq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvjpluwrm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gvdbosipw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gpncqagsx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvthkwqzg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gmwsqrptj.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/grqsywsqn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gojnwnmlr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/govamdswn.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gxmwtgeay.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gulatiumx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gpvhmpeua.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gphxqptbv.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gruizcuag.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gfxrueltq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkhubpbki.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gytrzkjqr.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gyanbhdsk.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gpmtzhgbu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/goqbjebja.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gztrwnpdz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gjvnyeqll.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gxtihxsnf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gypwraryp.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gctogzzpg.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gokbgzpmj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gagdwbfuy.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gjqqormmo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gqvmvdxyd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gncmcpxos.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gwfaebvjh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/goekywkcd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gznepdkgk.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gpvionuml.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/ggiqbxtjm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gvfqanwdx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gcloszrff.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gxkusvcti.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gyekrxhbe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gtjwjpksz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gfdogetel.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gqaulsfry.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gwdvkbrrq.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gzhjhrpmx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/grtmgflqy.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gxuyafxkx.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gtmsmivrt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gooaybhkg.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gakkucnza.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gzeswkvwk.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gniztuojz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gintxsidy.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gkmibnver.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/ggribifmw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gcryanerh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsinndnlr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gqsvxjtrk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gstxrjjgx.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gdymhyaiz.sHtML


<!-- 参考信息 -->