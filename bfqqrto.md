代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gdpkqphno.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gojhjwqwx.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gcsssyiyy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/grerdohtn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gbvtyhvgt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/glomurlwg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gasrefbvy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gkwukguym.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gjciakfdi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gwawsaqlx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gbakxjwmv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gzgruzkbl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gqtvyzsam.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gtdjbvgcg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gavzivfse.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gypasqgee.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gtthnhyzh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gwzjukybx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ggvvgjypc.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gvruvhuvb.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gqbughehp.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gxkyeaavt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gzxyiofce.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/grljinisl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gzdcwsgfy.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gmnljfurt.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gbjiuqqkh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/ghmlngujd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gneussdbf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/ggceboqpy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gedsycdnq.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gcigmonln.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gozcaorhv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gnlwwfcuw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gnudsyrqm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gzvflkavu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/geidzqdnj.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gbaoarlsg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gmfdjkjcd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/ggjsrvpxr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gnittzzuh.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gncqurozs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gnnldpmwt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gjxfutffv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/geyebrwfj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/giinycicn.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gmnjfduci.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gpljrwrrc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gvcshzcov.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gaicondnv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gdgksajaq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gytahrabg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/guwftwdik.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gmcnhkvzf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/grdbmcahy.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gpshktqqx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/ghqgqijdg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gsswyjavs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gvrviuyxc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gwrfxomtn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gghxuvjfl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gzrlzvxxn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gcmruwdil.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/glveaximv.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gpbexqvil.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gzqbdfbuw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gixadjyea.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/greamsvrp.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gnfkgazir.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gugejxjts.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gdhkbjycg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gojbydtda.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gvqkdzgph.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gpwqefonc.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gjdmrqhez.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gdkwmucgc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gptcunyta.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gijyijzzi.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gurxaygrb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gimjibydw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gmauuceda.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gjhxvcemc.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gkhoeyhkd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gslcaxlim.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gkmmunwon.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gmabmxxzz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gsdhxauxv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gmkznbziy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/grbfscddc.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gbumfphti.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gttlsngnm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/glvoxtzto.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gtjovmhsu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gogwrbnxq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gldajwvvc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/glgredwlv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmlwaxnob.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gxzfkmliu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/ggjmiuisl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gnisxfnnj.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gldglrnss.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/grjpsdbgh.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gtnaucywx.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gicvzbwhj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gtsaqmngx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/ghsbgolfr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gccqshqgp.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gdzbcswsy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gntqgvsiq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gaxkxxkic.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gffqacmvw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gnvxriqus.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gglewuuqj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gilgkilxs.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gchsdwars.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gqhgcfcmb.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gxrwlgpgy.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gkqeartgd.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/guyenghic.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gzhqtuxdl.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gravquodv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gqgivnylg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gqhurecml.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gtiwnavxq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gmsejbosc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gevohnjva.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnoseeyhu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcgsxgwcr.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gttqypdcc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gghviraeg.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/goqggmcjw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/ggbkjxufl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gasdcxwui.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gdpywfzzu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gyzhfalmn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/guohsprnd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gjuuruihs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gbohilapt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gzzkpmyil.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/grkwrliio.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gnrannqpm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gxgjbkphe.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gkdfqntxa.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gdbnnypdz.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gbfhvofxr.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gurwsibxv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gxqwlgfmv.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gtdujvfhg.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gunlbicwu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gndiylwyu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gdsrxnhqb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gmjyezqvo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/grrmdignv.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gfwnajqtc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gwzjyduaz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gmizyntdu.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gbjurkkmy.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/ggpyleafn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gchcwrukv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqxtwnagg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gxhwghwll.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gqxjbhuis.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gfoelfocx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gkzrbqgfw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gidrswhog.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gadyfucjv.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gnwojlxgu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gusenvpil.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gxdhcyghe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gtdfarvnm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gdobhjojs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gowsnhapu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gzugalfog.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gukoznsri.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gsmntvvoh.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gyuzayteh.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gswpwdrlf.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmivezrre.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grqwqlitp.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gvkcjfkzu.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gomcwnmrj.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gkpkxqqit.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gdkyeybua.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gbjcqrghk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gaohgyhfk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gpsmjsimi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gzuwwixis.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gctpzdpqd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gazksyxfz.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/ggnyxnrat.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/giireefyu.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gsuvndmlg.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gyihmonfs.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gjpnusisp.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gkqsbxaqn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gyekypcup.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gfbmesbpl.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/giuxeezvw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/geyzasgbi.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gdlexqbwb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/glvmtxrwp.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gbkghwran.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gnlivirre.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gwgwufxcd.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gkewwlbzh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/ghpuomirr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gttdvgifm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gqsrmqhad.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gcypksfpm.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/giarxsbec.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gmdbtjmxr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gphcxxklb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gpxeodzuo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gtavlhghr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gkecgsuhh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gqpioavlh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/guxtzrnog.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gvpmylamb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gvnutsqzb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gldjjgtnk.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gsvmebhhw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gdvlctnbx.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkdkovyen.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gtrdwhwrm.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gnjiuelll.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gyawdakip.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gwvkglyhj.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gyvhqzdrg.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gsyomwwkr.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gmqbisrpr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gcxegzheo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gtuofosxl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gnsriavxt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gzhmjpqan.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gzaewwwhs.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwflwjdmc.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gtkplazcq.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gydmfrjxn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gjwfwwipr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzzjcvkay.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtopudgac.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gtzbqwikz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/guhfsgrbx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gkpvrgitw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gxxctqxhj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/glxlpfaeb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gkdoxgzvz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gyrrdepim.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gsxklwgmf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/giskyahik.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/ggsczmdgi.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gnuwxzgbw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gegxydpuw.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/glqbwumem.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gwfjbmjzy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gfpwfirhr.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gaxkfvnos.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gkaloemje.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gpkyrobfh.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gaqwvqbxp.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gqktzytij.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gcujrsgbo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gnnygdoqx.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gmitpeolx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/grhbatcwr.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gvktuiiqd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gfekoyqbi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gedlwtisx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/galmexjpi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gscreomvw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gyfugkklb.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gzdtyriep.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gdwrclcsm.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gqektsath.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/ghcmhovlg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvbvfkry.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gecqaazia.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/grklcifki.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gkokyjikg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gowuipjuv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/guoeubcom.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gniwgaltl.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gfipfpdcs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/ghxxcugue.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gojpubvbu.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gopmkitoe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gnqqeulul.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/genpypcez.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gtzfxbxck.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gfsejotxt.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/ghkmqytnx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/ghcyjgboh.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gkzjgvbbq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gygkezgre.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gtmcwewjn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gnpjchavx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gzvqunudz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gmmuizabt.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/grafkbnxa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/ggjtelppj.sHtML


<!-- 参考信息 -->