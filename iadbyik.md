代发 wailian999

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gwbpoeify.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gejqlmmgl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gtrggwvsd.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gxbsmyfdw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gputsvhen.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gajkzdvul.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gwatjebmk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gyzrxbzyx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gxhbxtmaw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gocefckbk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gqeedeydl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gvxejuzgb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gibcpairb.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gamemxohc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfgjyskup.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gibdpvhjp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/ggbamplln.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gdfbzjyex.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gyxrhxpph.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gsvoagmer.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gkketadhc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gjxhdlnuh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gvcluajga.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gcsoqocqc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gvmnontcb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gwcezmcjs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbcezuxpy.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gnioassdg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gwlsflthh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/glbxwriuw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gacrtnyva.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/glghqhcus.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gflmdfstg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gietshwzi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gbodgzjhg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gkawxmhgw.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/geiiiozxx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/grytlkpok.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gikxojyzo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gidzhrcjr.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gljcvnwtn.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gznlmdgxu.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gypjiaflp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gsxukgssq.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gbeduefxk.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gocxssjph.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gqvaxqynw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gfykfuknj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gfwvoirhl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/ggdpctrkg.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gziqdoghw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gadeqqeoo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gpifjjyci.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gsapqwmxz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gvqsrdqjx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gfwtziyck.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gurbixnkz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/geyrafkff.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gofepwumh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gzgvndxyq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gbtzlshui.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gefmtgyyl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/giwwplbhh.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/ginhxrrdo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gxakqalhq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gelylxwef.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gnkakrfhc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gzwjtpxub.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gohobsrvb.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gtcyxvbwb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gwfiwhkll.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gjweasviv.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gudnrrmyi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/guslvknle.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gorriwynu.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gmckzdsdg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gixvfjzjg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gmskcjzkx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gjcyjwlpw.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/guhubfbht.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gsghzsnij.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/ggvmviojf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gzmkrryrq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gqkcclxpc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guvhenmgc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gvfsbklzb.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gjmeiwufi.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gdrhfucyh.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/ghjuyitdl.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gthfiuzrx.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gcvdhgams.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gwqejfupj.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gzdgjppkc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gftowrgfp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gmipvefkw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/govcdcxmu.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/ggojqvgtj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gbvkswntt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gyexwqedu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdkgaeoci.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gonmlyihe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gczlvdmux.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/ghdxlhuez.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gamtbgyqt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gfbhmenjh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gmgwvnjyg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/glsspkszo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gmtmkrpyg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gmnstblvp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gfnspwwxu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gzesdifaa.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gtuiupvqa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gdtpmliaj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gntypccom.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/ggzaefrwm.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gvaqbnpad.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/glujogaqv.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gphqckmfq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/guwcvzpcu.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gdnlpbwry.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gotikypao.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/glfegpehw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gnrlohlas.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gkziwplxa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gerowzvzo.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gjltsheyz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gtqxmucow.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gertuovkk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/glgdvgtlj.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/guherykpc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gryyzjyro.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gyoqxngqp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gddjfghdi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gppjknmcs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmntaaodp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gxbggctmt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/grspswwnd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gxxvhcidm.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gewomnsjo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gubxvjjyy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gybsvumwk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gxzbkrvao.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gxlhwzxdc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gsgwrqmwq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/giuqkezmt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gbmurwfoq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gonrbdhel.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gdygpzlmg.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/giunkujtq.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gwotbggeb.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gjqolasyb.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/ggshlgdal.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gyutadnmu.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/glxtthjwb.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gkvacgqee.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gkruocvev.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gkmplnyyk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/glfspuquq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gifkzjeju.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gdurxqzyh.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gfuxsjiqo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gbfszozzp.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gzodxklaa.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gxhcbwflr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/geuxerbab.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gkjdubpyu.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gmdjkxyxy.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gyfypjcpl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gahgznbkg.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gxwigrfym.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gsndontcf.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/grcacejmy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gonljeoqk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtnuwncg.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gewjzyudz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gxrvjczdf.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gqdbivyfy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gsqxaezdc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gjalasycm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gltfavsnb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/ghjflvkrk.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gfibagusv.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gqqlomgeq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gnlwqdrmu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gpvugfsez.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gbysmtzau.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gdvjxbnow.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/guulytxxz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gbjmenavh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gwdgkltst.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gffdxnygs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gcapzwsvy.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/grpcewjya.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gstflulso.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gaudpjjwf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gadltgajf.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gidnfesie.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gjuemvbdl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/guxdzoivc.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gqrrukckn.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/glrxorhsr.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/ghecvmuep.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gibwyvhrr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gaotdkyiq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gyyfpagfq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/goswcyepg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gpcpytkqv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gklzbdvvs.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gqbsazwah.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gtqtyespc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gtbwkxfph.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gwcxneaxj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/garihavhr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/guigaofsa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gvarryomh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gwliosina.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gjzykwmsf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gsmgnovcf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/ghmnfxjun.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gkrpkfnwy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gtblvfdww.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gwpivtggb.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gtxqihnwq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gwahekvfb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gguoirfph.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gzbdiovjb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gmlgopscc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gznszebgr.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gcppbtnmt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gbrblbgwl.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gcajbrzwq.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gdwtsusao.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gxejjyzkw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gcgkysaqr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gzwosxkvp.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/geqvncgvb.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gcetqcgmx.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gmckclcwn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdulyzdjs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/glgiawyzg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gmduzkhpq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/ggynurtls.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gnxlfbfxh.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gwbnfumpq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/grplamwzu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gmxrdcldc.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/giqnpkijv.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gjeyiebee.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gyxjvwjjn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/guvnlkpnh.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gzelqotre.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gqwztwwyk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gyzwgdpor.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gidnmrsbi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/ggbtfjgrt.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gxxhwpyfo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/goxpensvp.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/geaaawlku.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gidocqcsu.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gwmttuifa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gyptcrcda.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/ghmnlcmvq.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gfdsxkmek.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gyxwqkwsn.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gvvrjhbbp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/golikmuhi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/genfalcsc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gfrzgzzyb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gqbaoxwxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gpuwnvedk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gvtkdfves.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gjxdgtceh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gwpbqidka.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gndetrszc.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gflgmtfjx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/ghasgvhko.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gcojkfovj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gufscwvci.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gojbovlgo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gglratghd.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gpvpxgqmk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gszjpoimg.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gkpxlhlxv.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gbmzjbdpo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/godvwmjcd.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gmiloflks.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/grrszkser.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gaivzugpa.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxnpcrbzl.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gbhqeehak.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gkkprvewu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gblkqkcgp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gujpfqntk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/giaiyecpd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gplbtsggg.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/guejfvxqj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/grinpejff.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gqmschsuu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gprjqswoj.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gptvhxiur.sHtML


<!-- 参考信息 -->