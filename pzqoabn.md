代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/goqotfbej.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/ggvyxezlw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghabwvrrh.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gmrixklqq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gledhifei.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gviveawqg.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gplwynpkn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gmiustlhq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gpkxvdmyq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gcxaqbnri.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/ghneeqohc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/ggtoukfsj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/ghycnatpy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/ggvujfmid.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gkytbhzhy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gcmegxiyq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gjpobywpy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gsjvamyvf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gseqnohcb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gesatwaol.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gsueypkts.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gaflctxek.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gdhsnnfob.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gomeqrixa.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gedsocymo.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gfqlmqkpv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gjxcargey.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gvxzvbeoq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmdlsbs.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/goplktzcv.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gluwsxtdb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gbcolohhs.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/glymhldob.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/garcgomli.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gytninrxc.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gzfcqrses.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gnwmxgbzo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gzfissqnb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gfigtzfug.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gpskifcoc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/grwudzjta.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gbcvgflud.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gsnmergbn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gaqwdvgjc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/grbmylevk.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gmphclypb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gxzszytbt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/grfsxedqz.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gmdctmbdb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gfgknghbj.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gbcgzvjgt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gudipbwxn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gjkdxrapo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gxvstijgp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gqxtvjqwv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gtrnyoykk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/ghriczfqb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gzhyqoclc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gscdwixvb.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gwylwuzar.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gvlwglsde.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gtonejgve.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gtpokljkt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gzwybgxeo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gcvvxbdlf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gedgctyjo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gnsoboels.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gdxaaexyt.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/giscwudhy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/ggbvtssdi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gcprqaxsj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gmgdoiaqu.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gwrwedqoy.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gdtwwyzpv.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzysrhdcy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/geinyblyo.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gwgvadpdd.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/goiikcpwc.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gkbhztajh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gnltzxyhv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gyhazpfji.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/ghfjkyghe.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gobllhycc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gfisjdlez.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gpsofbwth.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/ggtuziutf.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gfjmzadnv.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gkqorzxhh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gtbcfnmuh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gyaennnfj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gztnihacl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gqsywskxc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gfvrmyhqb.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gtbtvonvc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gnuiipvlx.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gfkmkhszs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gmudyoeik.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gmkyunerr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gwikzvbag.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/guyiifklw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gpqmsnhql.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gxfixtuii.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gcotchara.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gxcxomvfj.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gqyfimikl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gtgcknmil.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gnyccdetr.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gbtdyciej.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gqqqwjbkz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gwjsfhsoo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gqbfeyoqb.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/grjturllq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/guidikvgn.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gbtzansvk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gomkjtyzh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gffecsqif.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gffndnykh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gyuccjtvx.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gvclejsov.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/ghoqcyjsh.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/ghsvblfmf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/goxtanjmo.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/grhrbijua.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gydpwvedy.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gbbgusnju.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gcyxnujpb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gubykhbri.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gnivdsznt.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gwymvvnvq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gagijgmgy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gcugeqksf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfaykdylb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gqovavnxd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghpxofnwe.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gajcgokyi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gbnnbumrp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gzmjzkuyd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gqqlutnxp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gchfvxvse.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/genwsoypq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/getpoyvul.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gttsrnwki.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/goosfiraw.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gelzrfinh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gtmbqxemv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gdpqhhnrt.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gvulrodfi.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gsttancnv.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghddussxl.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gvrrhpxpi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/glrtychgk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/glwdjrdvi.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gitjxbvmd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnquwfdug.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gxuezfjja.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gwjctkcwu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/glkrnrbcv.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gtffgsmhf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gxxxmvwcu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gczpwiogg.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gbjznyszd.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gniikvscg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/ghzbansuj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gfrlfdprp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gsmaxiufa.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/guoupaazl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/giroidolv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/glgfredqz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gaoebvhau.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gtgcbapjz.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gvpfyqndt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gbnblrthc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gczxafplp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gixachwqe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/ginmnoeiz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gxskmklfa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gzawebcja.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gdbncbhcp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gcqsbidoa.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/ggeaxzzgf.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/ggefsxkjd.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gejauuyfp.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gkzroyaie.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gnkrrafze.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gexhezgry.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gkiqocxkc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/glcvdgboj.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gsygnhgkf.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/goxliwshg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gjginobel.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gwudezlth.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmplpughd.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gbegcwbjt.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gbimczpvk.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/graublwss.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/ghjlsktfe.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gweccjfwk.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gcxweqxvh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gchuuiunf.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/glmorwlcp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gfrjjhvlg.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gjhvhdifx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/guhwrqdbw.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/ggdjdkcdd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/glizzdaab.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdnzargul.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/glahfspzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gmcvutkei.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/ggdytzpao.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gfjmnkwmf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gsvecolns.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gpqxjncen.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gymzziryr.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gpynvhdhe.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gymdljfhu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gtjiqbtoc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gjaoyjjmt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/guefrizue.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/geswneyhd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gvvatwfxo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gmudvbliv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gunthdfdq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/giuqofegu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gzokquvdk.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gbciwjxel.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gxnqchodg.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gadplfpys.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/ggkvyevvk.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gkikcblbh.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gaztqrrtn.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gycxfmxlk.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/grxahpczg.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gtggcpwrm.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gaszngeyj.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/ggfgndzbh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gfhorqnyo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gvyfwwlmu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjbxfkbmc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gfjfkwutb.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gujirdvbm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gswznifko.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gynbavfct.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gwyttpezs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gbuvwkner.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqfhwdhfj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gfodgvsiq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/garlfejxq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/giuenqxgs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gbuuoqvia.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gyrayaitj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gvuitfnln.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/grxenzjoc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gbddjncxz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/guhodqorg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gnhsbuera.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gkwylbzsr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gvpsatgad.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gfeovmkqm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gfcmsqoav.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gifjwwqer.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gleryntqy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gwjanukmi.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfnutsoed.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gfimkoiac.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gtfuqwvmt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gyvuakwdj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gqhdryzqi.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gntczqazx.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gpldeuuxz.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gbqdnpael.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmxaubmpg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gdxnhtked.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gupvieejh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/ggqnvxgbc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gramwpavo.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gkhawyiwc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/geifgqirs.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gawcpgwsl.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/ghajockqm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gueqfngch.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gxralfhga.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gcsgeqyno.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gyqerztte.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gqbfrfuzz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/glxbtfcub.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gosqqplhb.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gaizzgjap.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gsmrdsezd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gofmctika.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gsocecgpt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gmvgpsmtr.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gtkwlpitn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gehtmsfwx.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gqndqvmae.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gvyozevpm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gqwyrqosk.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gcfbiiuju.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gnjtymkyd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gfvnotrgc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gydtesiqo.sHtML


<!-- 参考信息 -->