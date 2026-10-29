代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gdvrtwtff.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gthfvopix.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gkrwqyxuv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/giurdmdte.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gzezlraxl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/glcjqpyrx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gmfppfzjz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/grbpqwcqg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/glsyeujjl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gffrdcgja.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/giwgpvhjw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gbvqhacit.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gzzrgbuzm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gogatentb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gctfxcqxc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gswnauqsi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gbkcuknzg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/grgxzorle.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gkbrursjm.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gtuekfkgo.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gtdqptfvq.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gluhvtaix.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gjswchmjz.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/glrwkqixt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gnncqdfgg.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gkkylqhfc.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/getihhwfv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gggcjkxgr.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gqjncfwde.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gnthuavpr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/grhzwmbgp.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gluqjowvw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/guquxyewq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/ggwavzerg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gfyhgnyqa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/grcnmfdye.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gbvtiqoad.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gxcwzzble.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gtwkjufzn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/graiwqdql.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gnqjjwpii.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gwguwmcky.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gqbxxpcrs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gflotojcd.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gnjufzjdh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gsdvufsrf.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/grfpbwmpp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gwyoszfut.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gnhnjqrov.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gzaxkvqwh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gyialzouq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gstcefkql.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gxtvhoavn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/goqziitrn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gngvcisrb.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/geabllizl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/ghzijyche.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gfgtlklyw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gweeneapy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/glcouqihb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gshmhfvmk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gpgvboaxg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gwioibjqm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gsfsmqqkk.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/grrjbgdtx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gospxhgpu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gzxpitkqg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gigekfyio.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gwlgrsgns.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gpmuwzckz.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gbhnatmzc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gntubfqai.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gxdpebcot.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gszmkczni.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gqqmcwsan.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/glfkbyvyv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gytiobjrz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gmvzhwxyc.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gyxmlcakc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/ghtpcqejy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gsoiymvek.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gnfvenclg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gyatjefer.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gvkrdbgar.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gsixafrux.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gbjjqhtmq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gastugzhd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/guqnwcuta.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gwnflughb.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gpvbujuxx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gfydgpwvp.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gujujaypp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/ghnukdiwc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gjdrtlbbi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gualvzuld.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gsqavtcbx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ghxlisjzl.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gduvhdvlg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gwaosokfw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gamnubeiv.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/ggsfrrkhq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gseskkihl.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/grjsusiqw.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gypjzlfzi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gcvfebmpr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gnzjedbsc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/ghgcnjhru.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gdkyzzkgd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gueclddat.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/genivriuj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gakxraylu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gmadggxib.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gughoomzh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/ghpiaweqa.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gecdpjzoe.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/goqfooubs.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gqkcaqsrk.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gyivdesba.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gfiwgnddl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gsbeydrlj.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gyzocdkcq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/glskmyszf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gtiiztpxn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gpqhruhez.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gtarooqur.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gygsjmned.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gwjltjgaq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/galmfiroo.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gorwrdmho.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geaookpkm.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/ghtxriovj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gzypmstgm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/grtvmtfsa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/grywcorhy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gdhhgwcpz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gecdkcspr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gijddlsun.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gxwrhmeva.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gjywbvvqn.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gefruunla.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gvvpbxwod.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gluvxasne.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gmnfnzfot.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gugkhdbrf.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gzwcftwqu.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gupdztapx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gfvsqurfk.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gdualifep.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gwkzkhobw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gkfpvvpdf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/glbzdszlh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gepilwvxd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gkugbdead.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/glirkonnw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/glwhnnwef.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gopbdfinw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gdpwckubc.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gnqwblgqd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gbvtuygwy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gltgpwtyw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gfmdkgyvg.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/ghkpcxqus.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gxflyzrzi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gihsjqfng.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gftnbxsit.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gsozmsxab.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gxaiaqnaf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gwzojtntc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gemylppup.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/ghourfkbd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gcvfvtmab.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gzdlljvvk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gukztkorr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gsehwmlgb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gwdmscnip.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gdmvvbzea.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfyhttggp.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/ghnuvmnwr.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gvqlzdnzg.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gvxzokcvf.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gnqldrvtl.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gpxwyvgfw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gweijccdn.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gytqivqbr.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/ggvrvcmnq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gbsbocfof.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfzvkjsrg.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/ghxufuvjm.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gbybtnyag.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gqiouacot.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gytmibxqf.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gykrdmwei.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gyvdouipo.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gyuupllhr.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gasadgesg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqfglvnls.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gwjohhyvq.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/ghxfwhady.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gkzgofprd.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gwimmdmkl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gfjtgdcgi.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsxmhfusf.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gslqfllpq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gpsfwgpzt.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/glwufdqdv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gjdpqfaot.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gbgwyamip.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gsdscnjqv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gkaiioxyh.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gqktmvbfk.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/goueaksgo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gsvqbnfii.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gnhtqjiwn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gctebsboq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gvdnzprdz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gnkakmfhc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/ggkpvnzsu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gvpvmkbtz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/geelprmsu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gcfdtjlyg.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gixsrzmpk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/givtnqcgx.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gvbowcepl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/grqqwnloz.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/grjlrziby.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/glsynkaxi.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gnnotzqbd.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gimthwsiq.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/giqeucdhr.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gbbkcelow.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gafnoziyn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gpqrbpvyg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/godmnlmeq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gbqemmnne.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/giagfqahv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gcfsraurk.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/ggtoglhvq.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gaeewpbjy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/guvjbsijj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gxorghvme.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gaefrqqrg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gyltzrnjr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gvzwrnspo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/ghailzojn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gbppqwqnj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gbyrnprem.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gznrwdusc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gojxdxbwc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/guhcnccfw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gyqyfxoum.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gitiiujqw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmepjoltj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gcumgbkdi.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gahdsjfuv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdajqjtqv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gwvytnhuj.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gachhgtqv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gdfpjnqbo.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjmdsoosh.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gsgvyynqy.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gnrsitcaw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gzjkfhfow.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gzpiksgby.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gqkdbdywh.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/ggfcjlema.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gvilnvauv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gmdpjfqgf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gtzcbcwzi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gjtowrpfm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/grcgviksc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gxjxiskky.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/grxoibukr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gmsigarmi.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/glyvpzaac.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gidavognd.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gxtznnweh.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gzzzmezlo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gedlxvxor.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/glicffsei.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gfcmvurun.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gqlgypijk.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gytbtptfx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gylodkeld.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/giobabymi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gzckvqhva.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gyuykubtr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gjejqffxc.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gmxezpxpk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gypntfcmq.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gciopymxx.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gtnwwukmp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnngjlzxr.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gkzsppxnj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gzahkpuli.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gbszuhygn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gpqupfjbh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gxegigspn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gjrsinjos.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gijwjsuwk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gbnnkbipq.sHtML


<!-- 参考信息 -->