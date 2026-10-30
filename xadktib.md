代发 wailian999

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsfysalbd.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/goihnoqbo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gikeprtsj.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gxbvtdpqt.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/glzkzyuxz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gpfeqfrck.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gtmnlnuhz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/grkvakumr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gqunnuehu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gdtcdsvve.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gtllktmru.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gilvuavsa.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gnxuqeial.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gjbrcvcgu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/goeuknucy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gppsqalqg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gmwjvhtey.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gecaghqwx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gxfmxchql.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gytargbxp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gnqyygebo.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gsihmphvq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gdebhfhff.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gvbefkxic.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gcluvpgrh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gvlehyodt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gymujjbjt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gcmuyfnpy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/ggnmdbibb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gcrnegnfv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gysklydwy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gzqefwnaa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gcxmpiebc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gggnnsefp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gnrhlyhju.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gfutqhmtr.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghyecfvto.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gbrpcpxnm.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ggwdeshmp.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gvqhranja.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gwbqanqvt.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/goccwaked.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gbkprxtfv.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gzitnhiib.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gekeiedho.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gmsapfrku.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/ggjbtqkca.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/glzedhkrf.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gsskrbrsn.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/grihqefdn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gwjwnyhda.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/glayvsxln.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gdypvvxdf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gellmifef.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gzsfaexkz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gjpuhzhna.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/ggjysfisv.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gzqhlbvkq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gbjxhqvoo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gxlkhchgt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gaumufika.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gtidtyodk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gguwatomh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gaiefymqk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gbtyxlbzw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gnpdjmzxj.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gbpxahbcj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/ggtachpyl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gzjimxylb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gumilfnma.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gkhkttevs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gucbnhzon.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gcasmuvoe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gyaxnyuqg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gzddwwfkj.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gxmmohsda.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gkfbdvljn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gjhqkfgpi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gjansnrmg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gsuimrgls.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/giphltslu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gudffaype.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/grqivdpdb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxxmutsgs.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gvcalsehe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gahaizouf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gccvyeliw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/grsrcddai.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gjfmhwzyl.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gyzwzvreg.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gtakqrqho.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gmdzbgrxi.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gtrbukyai.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gkucukriv.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gejepkkau.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gmekkazzm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gdzlkjeou.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gtwibazvv.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gwvrifqqj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gddrifygx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gykhchzef.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gupkeulwl.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gtsawkcog.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gsbmvwxrg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gpcfibsfo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gkzudnhrf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gjvyiviws.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gkvpwwkfq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/grpvikgon.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gbyuztduo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gzmtyvzlp.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gohfpuroy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gmvtoctas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtwohycni.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gktrvibgu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzmcrhmtt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwucjzioh.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gxkkkoiiw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gzogsacon.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gnwdlyutk.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gjnbfqfhk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/guvwcjsnd.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gxqbnccyu.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gaoijtdjp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/glthpypwe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gkdzuhdjc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gxjiyhtrx.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gfjhweimp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gpcnasgzo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gfaxknxwf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gxpsnjnft.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gtdgidwzk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gafejfjfk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/giehnuipz.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gbctsvkcx.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gtufucfxw.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gezmcqzoh.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/giopyrysv.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gbrdjhmon.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gprumoous.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gkryfmlkt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gdzrhtdfp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gabnpctod.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gvyprlbym.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gkubsogcr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gukukcykw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghwwxugpv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggmgfmhff.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gsztumkzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gniijogiq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gbevjmdnq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gpolhqkre.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gmhrafhky.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/ggudegnos.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gasoimqdr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gmzlkhnam.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/glodnuhxa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gfnfxgsja.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gyfogpwst.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gfgniiuzd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/ghfrncjcp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/ggkbdetdx.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gqziqruwa.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gbwbqhzmx.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gsjkdmoim.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/glxirlimt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gaikuddsz.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gqqqudktf.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/ginnovwqu.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/garnpdhyr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gpugsexjt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/goolhzrpv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gauyzbcal.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gyucuhyve.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gqkkwfvjq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/ghsfnshkw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gzgaiywsk.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gpxgywlja.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gajpgvcje.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gahvtldsa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gxayijlaw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gvhoynarg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/geegeqyda.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gjynftlvb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gbymlolyn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gwplymfvw.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gtseetmzy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gxojnnozx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gcarrjatx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gqkdpfrny.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gzkcmzgxf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gtpgdxesl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gsdiwelff.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gvxjtphdt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/guxeagvsx.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gsqhqwkbc.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/geegcquda.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gtspczxvo.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gqmbcvllu.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gjiriutvd.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gixxzzkrp.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gzlsnmdhz.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gklfzdrst.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gzwilxpng.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gqadgaddi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gjpnragah.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gdyrclwox.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gsgrixxqb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gsolgwsvs.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/glvxnztrk.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gbkfyzxeh.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gtqmewavb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gqkncxgxq.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gutsykrak.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gckeoduer.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gpwlzezuj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gqwqbfwsq.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gjxmcjfms.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gkkfazrml.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gbxqqxtzr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gxbxitnnz.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gpxhsxmhv.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gkkxdjdxt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gcfdxxzuy.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqwppltts.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gwiryvlcn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gbvzzlioq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/geiscoamm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gcklibaxs.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gyyjskqgb.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/giveqqgss.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/goigzxhjv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gigpcwbbr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/ggenavkla.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gknvubeyr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gwzqxfnxb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gowdzxwnl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/ghnnplmnh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/ggeaoyvwm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gewebyalu.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/grkvjpnwc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gycokridk.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghtjtskna.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/glgtcpcow.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gcprnzedg.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwadkonnm.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gxjhfimqw.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gkvwzbhmm.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gldcqyasy.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gshascvyu.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/ggiyvzaqm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gimhjsuoc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gewlqymxc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gxrfgkpnx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gxzcfxooa.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggqzsiccd.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gxiwambcg.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gmokkunbf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gqffwvhfa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gmkstckci.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gkufonekx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/govamanfz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtbfhqccx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gjbzronwl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gvtmmxciv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gyexazbew.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gdgdvslkn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gaxznbkaf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gtscksphk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gxqduiykp.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gtcpmsgdq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/ggmgirnrf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/guolehrvm.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/giquqcklx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gvyesdnev.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gyueehmpt.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gbywbnegn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gayykpxji.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnqfzpeop.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gqnuxnsiv.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/glvzaweyc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gshnhkktj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gxujzjrkc.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/ghkexrhcq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmqydvjxb.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/girtsnjqf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gowbfbjdb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gijvnlxuv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggrsmzxtd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gdzkbujms.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gnwlxhshe.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gqwwmoiov.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/goxqouxdh.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gzxzlzdcm.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gltmdrmgj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gckyqdtze.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsincuwwr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/giogaeqgi.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/goghbnvua.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/ggmjxrxce.sHtML


<!-- 参考信息 -->