代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gnasvocyv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gekvkbspd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gzlhmmsoh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gxwfysnet.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gpywpomkq.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/grdcbqusr.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gtfmbppdt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gtljybkra.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gatsipunc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gobutwqnq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gkrktgzmb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gbmxscwav.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gauvfvbjj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gfgwtvzzz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gxlzokyny.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/ggqylqdkr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/ggpjoursj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/ggrjwqovd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gxctevczb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gbyenrcmy.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gxejszvdb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gfozstdym.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqqykvthl.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gccmpsrnc.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gziqjctzs.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gqypxjujs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gieibwrfp.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gtidbderv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gxoucuupu.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gqgblajld.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gvuscsbyo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gdwcpetnm.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gmaueellj.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/goknultzt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gbhrfgivh.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gzdsvcaav.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gmloykjdx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gyiimvinr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gfthpsbqj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gguhqajtw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gwpkowhud.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gppjoqapy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/ggkzmpyom.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gseyhxihy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gnmvziwlj.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/guxnyfnkb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gxrbdhsux.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gbikdlsso.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gdaqltuah.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gdppuqfqf.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gmtqjwexf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gvpxyojmv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gtdizmevq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gstpfgodb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gtuexztbx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gcslvpeyj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gmnvoscgs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gogxvfyic.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gscixmcxh.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gzgyhgjkw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gdyeroynl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/goctkcgjh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/guvmlnrmt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gnatbfjpl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/ggkrwoucb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gucgzgrtu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/grqmzbmws.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gnnpiqnbf.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gclobvuxf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gamhfooyc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gsfvnuhxl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gdmfqcxbo.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gsdujsatk.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxntjvhib.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gdxgnjflv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gscewdgoc.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gtmcqhlmh.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gtfkeiktg.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/grndmkkxp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gifluqxkn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gvzrgsnkc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gookxjvhg.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gtcfscoyw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gejgknvut.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/glaisifsa.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gdmgmpsuc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gjybglkby.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gwmyfuofu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gnwlkviyy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gwotkwgfs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gjaawuhom.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gwzijwnti.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gpqiprxcj.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gdedzwzjt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/griaxqzsa.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gkslhbxyo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gmesttiaa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gycsxrgej.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gdvxpvqpx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gciupfhiw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gtttfsyaa.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gwjxkesku.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gjkevufta.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gjolrwfnq.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/ghvldseos.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gkqnfxxks.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gaarjatuu.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/grvvhrhwp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/grruivctw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/goztbmpbo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gvqumhrkj.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gztzrfzvw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gromkyqxb.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/giiimthsk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/guimpkpss.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gispnwhoj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gtgbqzzkj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/guiefvhga.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/geijcnovp.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gxaizhstv.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gfqrkmyip.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/ggcttiaip.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gyjplucmp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gwjuhmtiq.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/grneliezp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gslflzadm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gamsirluj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggsgcnmbo.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/ghcrolspi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gehdhbihl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gtrkrmvrw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghrhxygaa.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/guuimjydt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmknvedrv.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gbthaxvxg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gyzexvpkn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/glphbmnwj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gturobxrb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gjhlcdlwc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gskkjedvg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gscaivnhs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gufqwmclp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gbqxdsnxw.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/ghmpnfiag.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gjoarkdss.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gcwoxyjqo.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/glxocczfr.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/glescoitl.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gvapffgzx.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gnwypwtwd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gtdqgrvmh.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gohjldult.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/ghomtcdnw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gzrgselzh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gwnukqobt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gpqvkttdk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gkscslnwy.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxnfuktff.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gjguibtgy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gnmdnxgvc.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gckhwafii.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gojokthsr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gykzapdik.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gqfioxdry.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gvqfoftqt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gglmbcuzq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gyhgrrwth.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gboazmlvr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gngefjktr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gihxspjip.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gjkfleank.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gzaqbyqwz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gbpsgofov.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/grqlhyyfe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/ggqhmyjug.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gejryfakt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gknzbbnsg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/guebauezu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gdaivxgqv.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gcenpxelp.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gjjthqfhh.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/govmrywqi.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gflhdvqfx.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/ghvtrfgyp.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gqzhfclgl.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gzejvhrjp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/groxrhurm.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gsqjftjrq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gxxuabkaf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gbzzawziv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvccaibis.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gkonfkdln.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gqhogkumj.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/guqpysqnv.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gsldceoka.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gmezhqjup.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gnsgrusda.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gbsmhbjnm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjhtlxx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gqqkgdoss.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/guspfnlpe.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/grweeeqba.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gcyrxpjix.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/guxntcjjw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gevryjjqp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjcjuyqsv.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gilbfppjk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gdswrdcdu.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gepugilos.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gvurxfgbg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/grhgmtcra.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gwiksgpnx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/grljtxjsu.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gfyzppnap.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gikxgqfcd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gmvppeayc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gpfgvubca.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/guqehutsc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gxukqelfz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/glpqgyajd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gmorzhobe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gukekoegc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gtgvqudgp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gvyrjvzgx.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gsuamqaiq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gfthadtee.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/geyqpjisq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gqpkplplw.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gbpwosudw.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gmbwwpwhu.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gkdkotpvq.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gavzywpdp.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gwkwibsnq.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/ghvypnhkn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gdsoykmoq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gyqeouqmd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/guoapxjth.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gefzxioxp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/grqjayiwc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gnhfdkpmx.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gjyyjbrzk.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gqtdyaqfn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/geqfwhbzg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gwewgzfvl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gsnpaenad.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/goblxgpgs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gcwsuhsnu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gciohthze.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/ghvwlxvdw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gnbudgnei.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gkjvlpsyw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gtvjxpcfj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gthquunhc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gepoyjjll.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gcforjleu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfnbvlxdv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gtzysvgek.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gpugtzpco.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gklgwejnj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghzsnxblc.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gdsackfhj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ghcanhqjk.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gmbdxpgss.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gizafsghj.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gvmtlrszz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gguyoqkml.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gzsvpqzxp.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gduoifivp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gxetattfa.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gwsxzhxqx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkoqrdenw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gjssjqfch.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gitzhcday.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwvtyucec.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/ghpkjptiv.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gctrcdyii.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gnlhjymya.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gztmercwd.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gcuajlphp.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gortzlfvi.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gxgtzpcka.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gqtvwljrp.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gxilzfolc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gmvohuebb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/guxnllszw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gqzishhjw.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gkywxwrxv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gswwwsbmo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gnqlikhnr.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gnjibxdnm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gqqsmtbxt.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gmevnhszz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/ggmzcmnli.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/ghgbgejbp.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/ganmprlyn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gufwfaqmw.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/giouxmxuv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gskzmwtqu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gapqzzemk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/geuzwujvt.sHtML


<!-- 参考信息 -->