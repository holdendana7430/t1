代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gmwjcbrjy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/grkbgbpxs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/ggzamshlp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gxiwucsxm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gjrpwymew.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gqzmzrvag.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/grwxlwsuu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/ggxnritqu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/glqylxlnp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/ggswruvxc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gziupqvyh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gncybiqbz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gbsconuig.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gjnvtrhho.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gzbycmbmr.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gfeesihpv.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/grfocexoh.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gtsbnszhe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gjwxnadhw.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gawycsewc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gzprxwvmv.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gsirdoasf.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gseatoeoh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gypugfwan.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gdomczzhp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/goagkdili.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gegigsehe.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gepvmgata.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gliibtygd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gvdymzrvd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gtczejanf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gscfbubim.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gdznneqpt.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gywsjpixb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gspdbvzex.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/givycwngl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gzqvqorft.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gcggeephg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gitahlftz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gfhlkcztk.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gwmgivdxj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gismaaxqp.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gvjlbcplt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gtijsjlbl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/geywpxaqp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gxbdtyddu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gttxycvrb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gsgjfmomb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gjtfikwda.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/glgznhiyk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/geurvowrp.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gtgtltgzh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcruprfww.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gdjxzlywh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gkhygouiu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/ghumasapt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/ggwqhzvbt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gwengppdt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gxoaassci.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gthiilesk.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gyjnssvpv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gqbmhqclj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gxeafuimq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/giadtsyvr.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/grcrbfxnf.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gmyonzwom.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gramzkhbd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gqbmdlohl.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gxgxptamp.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gaxuiidja.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gryvclljs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gvmmuoble.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gdrqqfquo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gsetgtews.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/grfovtyri.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/ghjgtkpaq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gtctmfqcm.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gqehiolas.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gtichhqsg.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/ghvqhvymu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gfepxbffy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gfrcqyesp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gfrmttuvi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gwwyeymoy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gbyveotzd.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gxjeqzryk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gajthhbhn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgaztpw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gttfbbtmz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gaacnkrhe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gqolhjntf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqqcovagg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwwtvcwdx.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gxfmkmsxy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/grxcqihed.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gxhllilvb.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gdbbphasj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gvurzzggw.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gteemmkqx.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gmktcjjsi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gccntcspt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gpboumcga.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gtxvrfgxi.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gtxtezjta.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/geinxvvnf.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gydwnoyty.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gqmgczyat.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gmkdisait.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvmhoolti.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/grfkcysfe.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gntsluova.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/guifdxmxx.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gwvnvlizz.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gnpxfahhi.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gfixaprwj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gigykyqkh.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gpwbmalhx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gllgqnzgu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gioseqyqv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggeiqsorg.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gofmaqvtj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gmwlztnjy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gaqantsfa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfddstdhk.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gtgwvmqol.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvqilljar.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gzsgqfnai.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gbnkgdkim.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gegxhpocf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gfjfideqz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gdiyxufoi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gorxtyesx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/goxklukzx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/ggcsoivix.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gilbimqae.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/ghqodtucw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/glktrenkd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gnckwdjvu.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/grdtolhlr.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gguqzsnxg.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gkpjfxmsf.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gfjfuouwm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gzrejpofq.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gmljlerjx.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gvpzofepm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gnhzxhofm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gbbceusgt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gmkdahlcj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/guozsxfxm.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gblamcxxs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gvkofrzjv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gzeqneykf.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gokpmijqj.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gcbnduxsi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/grhkraxcy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/guhhogdmw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gssqylzqm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gecrvkphs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gsntywlet.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/ghmyryujm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gdarzcrdl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gbyhfxetl.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/ggyifpozp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gvnwsgaqc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gopyrpwej.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gbiwyzqdj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gzcdzfmpf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gibokslgu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gxzbcqjiu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gylklhoda.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gcfimxpdr.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzblgmkni.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gytfreiee.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnzzxorrz.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gfdqbqslm.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gkzkafovq.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gvpqdiuna.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbnhhvvwm.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gplvnuqza.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gyeiqpqvz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gzvpafqpf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gxzgldihx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/grbnytmnu.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/ghdnmfqkx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gptlknpoq.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gozhndbqq.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gcwzmngxc.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gdquaaxld.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gexouwqjr.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxxhjegrd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gjyqakwmi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gynaokatn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gyjgipojn.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gnhcnhnti.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gqcaafxep.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gougmoffb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/glpvobiai.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gfwhqdlio.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/ggfmruezn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gqarbtjds.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gnvqtjiys.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/grzcprwvz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gwrimxqsa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gbjzxgrke.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gyngpkedc.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/ghltolqtr.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gtchnhjke.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gyrdbodjy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/ghdnyyndq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/grhvlxorj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/ggqeboijy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/ggzvdfvie.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gggbxfnah.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gqorysdbz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gbqdawups.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gqscjytsa.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gdsoppznv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gbrrbwmla.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmlvcjjuv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gyafuzujw.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/grmvrapqw.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gvhzmlqff.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gtbgtizsp.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gbyqzacqw.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/ggsxpfkzn.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gzjodlicu.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gjdjeyycj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/guunfymkn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gpqwnxqxj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/grudqukej.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gtvlmmpgf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gkegobzfe.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gidjbnpjc.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/glhhxbqcp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gdsvstbiy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gmsvkhjrx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzmuagbkz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gddhgtzot.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gyysazxsj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gfbimcxny.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gkyypavuq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gchogotmu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gmrpmxvdl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gkwwerhvq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gjgzcekil.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gawpxjigh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/grugnpgdd.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gzpoucnge.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gbseexfpn.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gjgrwkqyr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gcgyiamnm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gtixqyrgf.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/ggxhxcbvz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gbrclcygt.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjncalwms.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/goszozokz.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gpvwvdmud.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gdmanxzqa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gnqkbdebp.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gxpcoasyp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwwobmkhd.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gnpccvysi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtrxrnpbm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/giiahzxuu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gyxkxkuvw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gibwypmif.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/grejgyfum.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gkzhaeody.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gdjircbfh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gqzjhtsky.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gtmmtjjhw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gkevbwkty.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gkcwopnto.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gnmcftmue.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/grhstwfwu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gglypzjsn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gucymlnjo.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gladvavyl.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gegeazoek.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gazhhtcfc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gvkxlnuzm.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gmsgxrfmm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gpqmkgunh.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/glaeapsvo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/grrcjcmov.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gwaonhxdx.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gxwbhqzym.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gchswrhwa.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gdggwkmod.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/ghjglfxed.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gtxscarts.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gxwzcdcfu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gypqcjcdn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gdwmluulp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gvpkeftdn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gkkhanymf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gicvznsug.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/guiexsovu.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gnusmwges.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gtpqvwdif.sHtML


<!-- 参考信息 -->