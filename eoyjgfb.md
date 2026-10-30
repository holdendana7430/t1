代发 wailian999

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gssfvvkza.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gszqfkaju.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gspykwlle.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gdjapcdiw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfpvboglu.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/ghmcikcye.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzjmqqldm.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/guebudmna.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gjxdljgiy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvpwbmhqe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ghznscfrw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gscxgeiuk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gcydhtuvk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gdlkavpnu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gpifucivi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gqdbhnmfj.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/ghsdotljj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/ggrzuxbmr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gzeirsqtj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gatxlwqal.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjyvcmwaj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/goujtghmp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gukqxabim.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gvhvydwzg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gsehlwtkv.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gyofgrgvw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gmrsagxpv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gsfivedct.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gcapubwfz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/grxpwoaui.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/glbhsbinu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gjevotqom.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/ghcmpdjnu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gsjnqykoe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gsuvyarlz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/glgzolmqi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gagrjqojh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/ggkhykqzt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gjpcqniwf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gxfklxfln.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/grqxpjplc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gzmiohpys.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gvbmkbocn.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/ggtvqvsgd.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gqovlkwth.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/ggzcrcgks.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gipuwlche.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gfrgxapyv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gjkrxdtrp.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/ggrwgdlzo.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gvuzpbgxl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gglcmmoil.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gcrzmdhez.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/grsxiqsog.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/ghghiobtd.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gkfxhnehu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/goynhjjys.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gpozrbvpb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/ggsziwcah.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gtpuvlfow.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/golljwykh.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/ghbilnpzt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/ggzdimhfg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/ghpynffdp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gzlgbqnxe.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gmxkyqtuf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gcmkvibyu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gofmxjzqv.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gpopkqhno.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gumdiltsb.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gkjgawlae.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gsnmetwrg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gdcqxdbds.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/goobilcyv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gdhspkwni.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gmjauwlug.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gabezlflk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gvtnrqxwy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gtwbuziww.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gsjhqqwgz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhauykdn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gdcrxcgou.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gayfjbbdd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gphqtlqkn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/glpcyvdxv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/grimnhmmh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/guudnnbyx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/grmhvouor.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gnbvwrenq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gkwsdeqxy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gsocxrtbq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gxijtugkj.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gkxaqmhxf.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/ghstsbjtw.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gztduyoqr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gqtcfztfy.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gzrrixlua.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/grbyynhfe.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gcbdvhydc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gnmawjwtq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gbgsdzsld.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gmtpxbbcm.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gwxrmtpgs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gnnrmvyof.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/glgacvchw.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gjzaxtiwe.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gbysmjwne.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gqwuesbwm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/glxrtcwev.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gpmrvrlwx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gspxcytti.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/glvdovavy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/glrbgdvxa.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gzxwwscqg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/grjexdxqx.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gqksrrvsj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gucvvjlry.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/glvvylqpq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gayoxreij.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gbxlhhmfh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbmsntcbo.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gfiwhvenv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gyqochygy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gazqkmmha.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/ghyxddgdo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gsvxjdjdq.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gdyfsvjqo.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gnriqxctb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gdtcbjgrh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/glwuvwofy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gkmxhcxzo.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gxallmrjz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gmtgpfvlw.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gathcrarn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gpowxyqfl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gvqhytqlu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gjzoqhiad.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gmskkvyhz.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gqpcuxuzg.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gomakixdt.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/giuxlakpi.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gkkradwcd.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gaofdoldg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gmgcpijey.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gwdftonds.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gmenrarkt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gpgxwosdo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gutndjxxa.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gfankuprc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gtiavvdug.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gsjgqawlc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmixliddf.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gjxuecpbb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyqyujids.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/ghhhzndeb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gsedwbrkp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gzapgabwv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gfsprkren.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gzqddxpbm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/guzwfbdfw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gsllwcxmq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gaejzcvgz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gyzssowwx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gjqacjcoa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gvwikmhjc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gdghcuqui.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gkojmlioi.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gplxobuyn.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gfrnxfyvm.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gnvcnyruk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gxbktuqcf.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gdzsngdaf.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gtuidxktr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnzatqpeq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gmjckwaxw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/glxjdjytn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gdjmknxhf.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gsjwatuqq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/giimxkvig.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gclxwfntj.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gmnyjymxs.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gwstyzaup.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gjhedmswi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gowaagltn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gmdhasvub.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gvwqfwemy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gmaxazvhb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gxyjhwyfm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gzifezdeq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gwunxdjvc.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gotpnjtbn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gywnwoqyf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ggmndpknz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gcmbnyylp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/getblrjvl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gwkrayacu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gnujipthi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ggtkrmepf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gddfpjtzl.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gzvalquom.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/ggjiurpud.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gxricjscx.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gmhhcbxie.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gqmbrthxc.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gmkjsiprv.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gigliyyjy.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/ghlmwdcmf.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gnriloypo.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gsdszemts.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gcltjefcw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gocldajez.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gybunduyl.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/grpsguivu.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gjduusgwy.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gwnuivwjs.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gifjiveox.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gaghwaliv.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gkczgntmi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsowlkpmh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/ggsnqbmbu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gaxqirnuk.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gwqfiwqag.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmvxkfxpg.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gjivegqqg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gwarjutwt.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gdnsqgljo.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/ggtqauzwk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gmicwmnme.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gxtteavzi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/grrpwfcon.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gezrytofv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gzxzsomjs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gjznsimac.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gblohzbwt.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gbdudmfuw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gvxfefrmt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gcwksrqbe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gthynccbq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gbqbrqjap.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gcoymhfrr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gaefwozxl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gllnvevvp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gnclynutk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gvcalbytq.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/ghtmklfau.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gvfcspubi.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gnxmfbrle.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gpekvdayc.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gqthfcdkg.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/geljyjtua.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/grhjbkvwi.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gtsotniix.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/grtxlhkuy.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gxdatqbqw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gppepiakn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gywfatyzp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/ghvvmpwjt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/glfzhukde.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gziljrlww.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gokwczjdt.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gxvwokaso.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gysynqgcq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gqotkcabb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gqapbboqc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gpvivingt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/grbotycfr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/ggqqavjac.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gvzvbxdqy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gtdrzcgzr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gqkbvzeyv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtibksvgu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gkjqghycn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/ggqwmpufu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gmlseyqha.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gtskeysfa.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gwhgejqrm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gcvyfxuzp.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gfyduigsf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gsbgtjluf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gndzqabhj.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gfudubans.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gjuyjnjeq.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqpqbrfhp.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gzariqtsg.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gkslbwqtt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gsjviozyi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gubvkhbzs.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gvacuglbc.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gpzykjldv.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gqcebolhm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gjjqkqywx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gkvvrzwdh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gunmtkvib.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gxidddqhp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/ggugcdssd.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/glpygqumn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gkcjpxndr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gamwgoeqc.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gklmpldkd.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/ghebhclaa.sHtML


<!-- 参考信息 -->