代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gjnbqylmj.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/giwkssxde.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqwvzlpr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gimdhebdk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gmixrdgyo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/goqqfsxyf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gonxttsyz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gqsqrvwqc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gawexcfct.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/geyuundaa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gtujctkcb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gnjcffisw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gatdvopnu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gwgsbozui.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/guktwxuvg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/guqhakfpt.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gjrdbmlmc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gizdgbpsf.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gzdhljvwv.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gcdztqzze.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/ghpyeyrni.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gszqxjzay.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gprgepthy.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gmmilqnsc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gygnqlrfo.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gkunutgbv.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gzdchudvo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gktllvtxo.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gtqkcmqfl.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gkplmeefg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gbdgidahs.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/grmcruaid.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gjpebhvey.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gfbawftpe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/ghwjrgyir.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gguqtynbo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gnbybjnqs.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/ghxqluyyn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gopaixzug.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/ghrjpwspy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gyyqerbzj.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gclaekofh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/ghoupxskm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gwtvuhiyu.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gerddhaje.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gkjgjdyhg.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gmzsciipl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gbqpjdstm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gzapjekxp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gjkrvknbf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gepxazeav.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gwdiczlio.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gkiklbfop.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gipovipcl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gqnpmdjuh.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gofaaewos.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gmntkqdof.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gjuaqkzxs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gkuxlxtpf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gayhvgdow.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/ghxjnojob.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gpagnsuqb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gkxccmcbl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gwtqduzqq.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gjicavejy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gsikununv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gkkaqgaxq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gxmetivkv.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gchlyuslj.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gykjrabps.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gejixochv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gaiysvcjx.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gwoqeeadu.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gdrsqdxff.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gepnkduag.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gklahexyq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gionxawym.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gimkthggm.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/ggixmgabd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gthoxrjgk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gfkfbifvc.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gcznuhdrw.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gjuexbhya.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gfqfjwxhb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gniyopqcy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gxdryxszg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gmaqvjslo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/griphtipx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gnbudxmuk.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gxkgtfjub.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gkgkwflyd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gsrytszxn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gcygyusds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gkabfocmw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gubhiozub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gyrzrloib.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gbhkqaeee.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gnncuehkj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gdrrkqcwe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gzkacjhea.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gteifbmza.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gynuvwzua.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/guzkncagy.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gtxysqcmu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gvcasojqz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/glnbvzuty.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gkoeahrsu.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gcmchbkxe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gymdsfbhf.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gysaaowuy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gjzhfyoeb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gxqyeuzwa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/guzpkoqnk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gejzxzbav.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gjxtvhjce.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gizicqxqw.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gygsxumrn.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/ggytemavz.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gjxedywai.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/ghqywmunv.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gwurlmntk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gimvlnmbm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/ghovynsnj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/goqubmcli.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gtjawfzca.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gjmvxqfkg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gqbbmvxyn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfvfjlnri.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gdrfpenzj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggzjovadj.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gqqspayzl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gxyjrmtgu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gcjgimxeu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gmaqggymh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gflamcaei.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gnvueyoza.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/glxwznbam.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gsyycxsgi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gbclqejbk.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gdcnvvgfq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gycyfiwsz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gnwhmthpp.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gmoisbzfp.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/goxwxpzrg.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gufcoxkpd.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gyxhqdysx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/ggtvouqdz.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gexwfxuni.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gfyxtvkiz.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gblgmvscw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gxcczaxhn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gyxojubur.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gcgjjdrcn.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gglddjypg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gpsfaxwiv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gybdtdhhi.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gkxmwyhyn.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gkpyoxkkb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gxpeeyabp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghhdqounc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gsocuxyqf.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/ghakothmj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbjcdonp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfuymmr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gdgsljbmo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gegtoxoyo.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gfxwgvbqq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gmcecwgbv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gxwfnrjal.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gemqamlcc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gmdsswkhe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/guwjhxips.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gjdlvfbuh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gcjvdqjqz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/glmewxlan.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/guofdkmsd.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/geamzxuqw.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gbgodsums.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/grvotxims.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gveeajdtn.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gmmfuvpey.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gldhsccdc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gsjncpwqv.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/ghswkmnjq.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gayzzimsp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/grqebwoim.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gglolrdac.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gqbtzurkb.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/ggiraowmb.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gskbdvxrj.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/grynifwin.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gqazrirbw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ghvisbebb.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gwxeedacg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gnecvzrju.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/guzvsgdnx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gtxcaqqqs.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gwktdhvac.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gkczriqrc.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gkfzweaic.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/giliglloq.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gnouwggsp.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gncecibzm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/grxvzzvps.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjpfikfcw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gglpmekvx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gnpjfrupg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gsnrchzjb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtxzsmdpj.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/grwohflac.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gzvcddolr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gtavozsfe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gfkjtfter.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gbyfvdvpt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gnmkaozvt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gbdaxhdtr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gmlhewzaz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/grrqfndtq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gytzlbrye.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gabolnnbl.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gohcggrlw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/guoksakrr.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gemsancgl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gycjdutty.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gwdfqytci.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gjksiotpd.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gtbnkqncc.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gldydevni.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gptwhluod.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gjwgnywwa.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gsbqtvbey.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gubmgszfa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/ggqgzzdps.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gbbnccguv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gddmlxgiv.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcpteeqiw.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/greizihqf.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gmqnahfhl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gekmxxdrw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/garzihrbm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/glezrdovn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gerxkriwo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/grunxwsge.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gfplinyle.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gsjntcwjs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gymyegxqm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gygkyeebp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/ghrbpuqic.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/glxygnitq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/glhlbcknn.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gmcgiopxn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjwockug.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gerdikbfc.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gteeukwdh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gafhomlpj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gdkyokcgu.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gsxoruekq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gqqjoxiem.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/giuqfayus.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gxglgkwwn.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtidavhrq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gmkcvwzoy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gjgdaveay.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gcyaomfjg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnutcroum.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gmvvkzdwq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/guqbtbwhv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gwdkxvnls.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gmlnzwsyy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gjrrakjmu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gkwxdaaod.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/glesquzoa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/ghwfvhulk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gqetqkves.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gcawasang.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gymsqmxpf.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gsggiwcdb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gaubbwjuk.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gjnitodqx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gdgzyjzqc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gviwssfpy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gveprgxmw.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gayptlkts.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gazaqvicg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gqmwqejea.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gqmydhlxc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gukqfofxd.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gcmfturxt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/grkfpltcc.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gjppmignw.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gpcryxcwb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gxdqhloky.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/ggusqymnu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gdnjuovxw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/giamfsxxs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gtuivqsdl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gyufavzrs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gwloiovkd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gragroczi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/ggsfqfstc.sHtML


<!-- 参考信息 -->