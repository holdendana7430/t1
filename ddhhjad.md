代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gzywexqkv.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gcxdniyxs.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gkzdbsfma.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gtwducxcu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gdfijlbhw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gorrchzxt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gupuacqyb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gbhcvlyrm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/grttwgoym.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gludenxxr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gnuldjlta.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gdcxqwacj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/ghlnqfwdo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzquyokxg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gqadawtul.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/ghlicaoss.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gseefvcma.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gclsyoonf.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gldonfqog.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gbuajlxkf.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gxizawepa.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gmljmawfu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gsufjrabq.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gozgfppyf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/godglacgs.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gxkblemwv.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gtsluiwcg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gjssbjezj.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gtqngerve.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gzyoilmtg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/ghvbjeyag.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gkydyyddr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gotwcklkt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gnimybqpw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/guibdxysp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/ggicsykpa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gasuednop.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gnzqqipjp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gzbtmlvrx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gbdfaogdj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gslmgrfmn.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gnytcbmhb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gjroxyuxb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gzzxwsqly.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gdbuqvjns.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gwqnlxcdf.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/ghrzququu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gzknsdwec.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gdueoxjiy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gdqesnmok.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzilmnmm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/glrcazkpq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gkdabrlqd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gzxhisxye.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gtbdhgomz.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gzbegvhyq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/glphxsrgu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gdeulljqh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/glvrdnuvi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/ghbdcdstl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gkfegyvfh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gynauhbmt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/getctmcht.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gyqdwosut.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/golpofbcn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gcxhlnhbq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/glcnznomi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqjsuigdk.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gubwgcapy.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/guyrgbohk.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/glzlugoos.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/ggvehctqe.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gjrcwpvkb.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gzmqsqkpt.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gpaggsvjv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/ghskcunci.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gisurpqsm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gyelmymnx.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/grdpctelc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/ggivxwfdq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gfiqexncn.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gilgjwoqy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gvtbbotzq.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/galnyhcnj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gvzeheshg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/ghobvqfqe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/glghjtlwh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/geqyqwbbf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/glfsxlpqq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gvvzcaasp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjjptvrya.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/ghkzcivmq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gjbnbtzsp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gcbupvqka.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/guaweorjw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gpajupcgv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gjgrwhtpx.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gmdqxfqbi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gmzobklch.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gsimfpxre.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gmqhkboyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/grptlslwp.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/ghrchppav.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gkfttxpku.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gwnnmykxq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gniuejfhr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/giqpylceg.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gdbdsbjjx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gzyrdonxa.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/ghfgorqlz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gpmsqllpv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gttmzvfqy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gpvdnrzsh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gbrjkhotj.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gwnnxuvog.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gugjsfnaw.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/ggedpplof.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gxxaegbjc.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/giglwsayj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gvmnmkpip.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gcktrsnid.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gcedlccjf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gcqwuwzdx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gbkodhbso.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/guagbfjgd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gbhipkmjh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gztkxgyij.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grmxidzsv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gkiadiyyx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gamtmehmz.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/grlhdbsuh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gucszvobn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gjuyryfan.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gghedwmmc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gtwzvdbom.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/guihpyaap.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/guqasipap.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gwrvlbnno.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gtmqimhgs.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gmcrofglj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gpjjfmzoy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gpntlsvby.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gobfuruzo.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/giyhdacfp.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gkuawlflz.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gkhgachud.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gqpwvjkue.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gkhbgzift.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gafjputyb.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/grofyyesp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gvimuxicf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gemvvznzx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/godicjdsj.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gphmuugho.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gewlfyxor.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjggbziok.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gkpclsnes.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gripsemle.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gfhzuebuc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gbffssqwe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gyvnnddkp.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/garolukdn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gdbozinib.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxesgkey.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gbcidzeqf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gffivvqwv.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gyzwulumc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gvlpjhzsn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gxmwgfhhf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gwhtiysia.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gvidasuin.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gyatcmaar.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gwpncepgg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ghjqerrum.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gehjvyfgh.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gkkcpwaap.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ghpswekcv.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gabkggqow.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gddzlhtye.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gkyjdijtm.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gqywzrmcb.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gmpheugjq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/ghkfcitby.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gsvadesou.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gdakzoopp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gkklijbmm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gzrbtihnw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gcgxsnksr.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gtomtmrnv.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gpqvfztkh.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gsijbqpku.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gqefrjtcn.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gqqoqurbo.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gsxyrztmj.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gdjkxerle.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gxoginhkc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gtqvdigyn.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gsxzcjolm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvawaubis.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gmusqxspu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/glelovboh.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gwkxrrwpz.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gnfdxcwmo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gpbuhgozz.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gfflawwjc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/glcdqqnsv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gujcjtwdg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gzmcxlglh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gjwipuqyf.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ghbyigjwh.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gyxapmwzt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gsmqrxiyv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gdzkbnnuu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gvxejippw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gnnemwhkl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gugnekvph.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gqlhnnaut.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gqncedrso.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gvpkqtpyo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gjovuammz.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvmcncsfe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gvrqtdnhm.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gffrtmsfg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gbjmwtfmq.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gsidcqjio.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gvfmyelib.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gzqnwzndl.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gjaodokbf.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gsrhfcabf.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/grpuqxmau.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gtgylnsxi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gyxljdwzl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gdvhxxdjn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/glpwzuwzy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gnpiuwoxi.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbkogisqo.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gsbrvmszj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gkxrdgalm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gwmzlwuha.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/ghqsqxmio.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/ggztyfzpy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gleclorpo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/goqyjyqoa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmaaedcle.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gobervcbr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gsmazryau.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gajcimkam.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gvnvgyzxi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gvwgpfidq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gktqeplxq.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gordbiogg.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gaxwtuwie.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/galeblrcc.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gmxadugjj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/glftesmqc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gvzcypkyw.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gmhpkojfd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gehgjkumn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghlhkjyhh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/grlmomtam.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gscsazggn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gqtkqkouw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gepqlwzhr.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gtxnccktd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gghwuomsq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/geidrjnaw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gjfskmduw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqxfgwdos.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/ggqlcrwjl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/geuncmgql.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gtyhlfpxf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gdcibxkwr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/getbhkrjx.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gycebsihe.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gysefypvo.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gcnrmvyjz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpatwamob.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/ghdpgmpzz.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gzuhctgpr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gcdurxowx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gqtlujgvp.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gjvpdbvhh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gmxcuafgd.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gcuqxfozb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gfblsvgjm.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gknfleolo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gjuouovsr.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gxtlmgsqn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gdfoqvpzz.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gtwoznszp.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/grcvexzif.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/garbjfxsv.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gjmxzfvuy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gevyssfcr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gohiqztdu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/ggvzoflig.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gadjqxjce.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/ghhjncxqu.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gjuckgljz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gkayrzwfx.sHtML


<!-- 参考信息 -->