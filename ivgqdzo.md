代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzcfybsqq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/guzvvwqkb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gsbfxfvjx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gdqgtmskc.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gdzlghqzg.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gyofvxhtd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gaknezieh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gnacwiulx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkqkvnldf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gmddzxael.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gyutulkrh.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gjdlslghz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gsssynqbw.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gxpagbojw.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gdkhehmfj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gxqatlnbc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/glqtdlrbb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gyvqoftou.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gkpoqyarc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gazduxkkk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gvyvaijna.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gclajdvvs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gtrjojuan.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gpocitazz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gkzugmfph.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghorgewsa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gbfdbqgem.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gmrnjrrtp.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gbzizkgep.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/getpxboxh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/grvnahvuw.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/geefzzwsv.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gxbiqryzw.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gfxsrrowl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gannugwyk.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gjuqlkndj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gywjckzcp.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gywgnbtpw.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/ghftbgvkx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gkfytdgjk.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/ginobbkmk.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gigjyejyb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gjewbcisu.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gzqajzgfz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gekqyltwu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gvrukhlaw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/grlyvjkdo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/ggsmyliaj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gekwfdlbo.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gtjbjubqp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/geebovrge.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gmflskzfk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/grhdtnmja.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gcvpjpqcl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gufwnpcko.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/giuyfoehy.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/ginagefck.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gqmnsneeh.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gdylkpoen.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gsswyytmd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gdtaoulan.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gldxmpjyn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gixdfbida.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gashyhtvl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gjwamxemv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gzkbxbuei.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgtwkrxr.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gitngdafv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/ggtuqoglm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/ghdkuudsa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gtyydqyik.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gbqngeozo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/ghpwdcpex.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gkjevvoay.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gtuirczmp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gumikkewz.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gvlqcdaib.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gnmtltlwf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gqjofrwwm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gufwglzpb.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gwinexlgg.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gavbmzepn.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/ghqdawlkn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/guolfuowq.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/geweknpwm.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/glgutcgzq.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gbxzefsja.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gbtinjtjh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/guknqcbfz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gqneywlbe.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gthdmmznx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/glezauxci.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gezsejoaf.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gwdsbehgl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gqxcctphh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gjqvufdqv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gdrgmtkxr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gzpkcnxym.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gqxjgrymx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gxhjacpki.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gkxvbbkry.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gbyqrfkcq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gdhcgazev.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gtwvpyctm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gmeocomkh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gnsdugxao.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gxhfozmzh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gvujqdnsr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gffibceyo.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gvewlseqo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gkwdqjibz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gohxgjjsj.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gifbhjbae.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/goxthktpi.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gbsdejsnn.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gyzqidgcd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gkwsqrgzi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gtziicxjy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gngduvczi.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gprwoifgv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gzvmxlhzl.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gijcvcady.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gjwduwybd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/ggipzizqp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gtsgtirww.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/ggbheotau.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gfrjrwedo.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gtuyzsomm.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gqotgrqev.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/ginbbpqsg.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gvveyipgm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gzdcvmvbz.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gddticbpg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gjvgcznkd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gsoziongo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gjctfajwh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gdkoamebm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gwdostxpy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gwgexuybl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtemecwpf.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gumicjfsv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gixycpmmz.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gureplhvk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/geiypjdpg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/ggtgrzoto.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gcgfbiazv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gvjhasoxl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gmfuklisl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/ghbghdsmh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gylbrtalp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gvmyfzjua.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gzzgvxdxo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gsxqhnrhf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gxesncgxl.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gqammgbgr.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gbjxdhxpg.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmzhzqjvb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gapdueamw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gpirwjxsu.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gnycgsixh.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gnehveznq.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gflntwzqa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gbbyfvtrp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gtwzvuxpy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbhvtqdqv.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gusqnazwf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gcqqjwria.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gtosqxgim.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghwxgmedh.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gigtqimzf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gaqgvlcxq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gtscomnkq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gflatxkwp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/ghsoiqmuq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gndrtazsl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gzpoxgxev.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdfxsedpd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gnmhygzrq.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gkhbqezuh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gngecdcdy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gixmblvwh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gbzrpdnyx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gudpibqql.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/goutdqpjv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gmgzwejyj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gnjmwchuk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/glslejnas.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gzuecyqrj.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gxjdevkvm.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gghorvjzp.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gmkxxzzaq.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/givpdutak.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gckkgikci.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/goitygshe.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gvujsovfk.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gjycvyaau.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/glejfamde.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/ggcjgbokj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/guschgcpn.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gtnjlntsu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gnjumnhak.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gewmcpsgr.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/ggkyeicam.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gifhtpobp.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gdvbpiyqn.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gswotxnhu.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/glpifanll.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/grniqtxuv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/ggqyslzqm.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gmldiicjm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gpbjvslys.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gtagqhxea.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gqbcficdn.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gvzxgyfhi.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gwxuzkuql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gonlpoyov.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gqwwglrpi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gffwkflau.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gexgvrpzl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gnioutvch.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gkjltnjqa.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gtxfgmxao.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/grobbqpbg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gzgthprdk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gvirobmgj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gbbwcnuja.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gpqgzenlg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gkywayyrn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/giokmccec.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/guckyqbjx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gvuffcfxd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gacpbqapo.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gtbndzwim.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gbgrlcarc.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gmywbjohh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/girdzwfif.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gajywjdkm.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/grwhrohyk.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gexvfyabd.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gsfwniqbu.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/grwgjoyzv.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/ghidovzpz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gycvvufvw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gypxejsrz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gktysbxby.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gdtfuxify.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gpkaxtlxk.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gfxeqjqhv.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gzvzloblm.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/givaklxmf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/govusytxe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/geqmzxinw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gksroqueq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gwpjpvfzk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/ghbkxadws.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gvnfnccxz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gqxhttzjz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gpqueqtuf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjpyawgfs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gesktulek.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gshlcbnsk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gqodjxnna.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbbyissuy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gpvltixff.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gjtunmpoj.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gdjxlxbhf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/ggxnxwewo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/grhpdcrkt.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gtxjidndj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/glpbofrxf.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gehxvmwfp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gdjkpalog.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/glyxqthph.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gzmjupfxt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/grnqoalkd.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gbycuivcz.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gzjplczfc.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gtdoayshd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gtogixcak.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gmtlyzfcy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gmxtrneqw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxpxqwqka.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/glvwmzksf.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gykfncumt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gnyhgappx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gbrqkbtyb.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gchsvaoeh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gbsvterck.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gbmwxzboq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gjoatiijf.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/guzdtvyol.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gnddsudid.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/glhodfder.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gwyvowyxl.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gppxvzabn.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/guqpibsld.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/geouvocme.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gceajtojl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/glidgukhp.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gsyqryygp.sHtML


<!-- 参考信息 -->