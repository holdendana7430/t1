代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/glbimiyqq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grwldgxdx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gnsgpbnvv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gxhrxidvu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvylsompb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gwecajsof.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/ggzwgvzan.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gcgbpuzke.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gpdnhtrmi.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gqnrhgqwp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gudotugez.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/govxzendl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gjncaynfy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gyixvyxly.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gixssvifn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gxnwyzmzk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/ggfnzhmie.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gwnomxwrd.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gfjmehrkz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gwvtumegg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gtabbgdor.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gionvtbgf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gltcxglxo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gnapvvaig.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/glfxqnvno.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/ggglelora.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gpqkplgax.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gguznjvvd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gtnfpypav.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gmuksqbpn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gdlqtsbkm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gkmydevrz.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/glnsxomxj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gltwpkxrq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gedqhdfzw.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gdkgdssfw.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/ggigisloj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/geyftyvrg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/ghkhwuyeo.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/ghhqcxcyh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/ghrbyouva.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gqlsvrtez.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/ggtskieka.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gxecuzehu.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gcodfjgxz.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gaxqrxbza.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gqwzdbemg.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gywzdoucs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gxuxugepl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gwswivvvr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/ghhwtyxyl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gnubskeyu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gseirukyl.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gwqfafwng.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gwceznqir.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gaxxuawzd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gchuvixml.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/grdcixhqp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzodwcnnx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/grehbvdhn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gxymvoibw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gqstcovim.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gqfpisuuz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gfjcmfjgn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/guspruowh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/guxqnordx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gdmjwtime.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gjorjimqk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gfwgxfmvc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gjrotghhq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gzbhwgkwr.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gurnzbzgh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gyhpnvfbu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gldhirvhx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gaujbyxjg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gfxbpcwyx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gadccgtnk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gfcmcgxkr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gylqgclwa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gfrgmldkn.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/ghznqdrpn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gkkkwgzcn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gskyexyln.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gztrdnkti.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gszkgxkoi.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gpgrpwlft.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gojcdghmn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gdlhhrwjc.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gghucvsaf.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gdlwwdhgr.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/ggsxfvqoq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gmhtinbsl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gtfzkozlp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/grzvuujxh.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gipuidqyy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gstlfqegk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/govfphjwx.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gbzxvjsgx.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/guuaotxsb.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gdtsetsrp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gicczkbbv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gvjwtybvl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gdqqiblrv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gfwcfsine.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gzimcbark.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gvcytcbch.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/guzivdmvp.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gsmcmuscx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/giufxdhxy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gnajcueai.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkdapnt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gsrmokvbw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpruohmvg.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gggvymeji.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gjramzgsy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/glewjbuxe.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/guaewpgpu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gjqcewmlp.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gynxsujxu.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/guugtvkbb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gbnznrrag.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gireeiidg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gatbohdta.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gzethjhyi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gzogkzmwy.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gvqagxhhq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gohzrfznx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gkivktnwi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/givamoeij.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/grcczmalz.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/glbmlafuz.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gbwqeqspg.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gqxqltviv.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gqdzrdgqr.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/glqxxnxhd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gyemjlciy.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gfsdaopfu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gzwpkxnwp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gqjmneeyi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/grdkbogif.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gnevthqst.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gjuqftbrq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxoufuqdx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gifsaydpt.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gvfojkjvf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghgxdyyli.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gddpshqnm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gvnqrrosd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gjrpncewj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gjpleqlmv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gxbdgpeuu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gvckgrtxl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/ggkjtgwhm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gtuqaeprk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gfyduadqy.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gifgqjgiw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gqqphsshy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/ggjxvwbaj.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gtjrbhcsm.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/golmgqozk.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/guotsnfyj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gvkelakuh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gygfmfplg.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gwmirkqyg.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gsvathprx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmszdfbhd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/glcbcftlc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gpdesfwbg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbcquwhwx.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/ghnaqiffn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gooaygitn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gnsriekpl.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gattnedth.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/guqncieiv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gchnrvjyx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbboarkwr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gknxzsurz.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/geqeeefol.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gbpgbcikd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gmopsfbxe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gvuifoykz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gaqwffdov.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gucvyuefw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gpcollgfr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gyiqewafp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/grdyzuqea.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gbiqpefut.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gxqvgyach.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gszeoxpmo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gdtqonthf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/geqbzliuv.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gxuyxgryf.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gwhgimhbq.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gwziwhdmu.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/glupsfgxs.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gvudthqmk.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gvdcxrjoc.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gzswsyjoo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gngupqgrf.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/glaqocrbi.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gfbhctsyt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gqhiaesrw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gxansaddf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/guwlwvjsw.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gkwpyzskv.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gzqmcrtaa.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gbczawyki.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/guznvqjnk.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/guhcoljin.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gdgwebkum.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gxlxibnxq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gbitdzuce.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gusrvooqz.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gcbpxqyor.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gypbgtzub.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gshhpejqo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkquixqdl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gpvhgzbxe.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gjwpiabff.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gdnoratfa.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gsgkqyqjf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gcsejrbyx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gcqgeeayh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/giujkbjvu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbhrsmfgz.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gukkldlaz.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gjwuhvliv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gsmnbkjds.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gxjenpdli.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gkvzdozzh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gknctwbmr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gasnlaffy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gvlfvntat.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gsdmuejxs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gfuezrcaw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/glxteucrc.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gtolvjtzu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/geggnpddo.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gpjchmcpw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/garlybujv.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/ghwdszcqu.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/graltlwms.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghopslxob.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/ggwznfmpz.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gyjewocel.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gnxrmeekm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/grvojbkko.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gerfqqcyl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/goelfcyty.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/giukaboor.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gtojxyjqw.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjtsqgsgt.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbvofwit.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gjmellkit.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/glrpypuos.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfpfmofik.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gcdvoytgx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gsvsftkpf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gsmdoxffi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gytjznqln.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/ggjvmndyf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gmuqcphjv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/glemfwwnr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/ggcnkxpph.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gwdiaeplw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gizksvpjz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gaunsyjqa.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gyyklxwtr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gfdxmicbs.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gtoddsoct.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gdnmpwepw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkigppomz.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gjsdzxbxp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gtcphxzbr.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gpzjyfuks.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gkandmias.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/giugyboxr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gvxdfopvd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gfpchtucr.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gkdzdskiy.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gkwvfgxmb.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gkwrzctph.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gdprvutxx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gprbpxlkp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxekyxnky.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gfidnldeo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/grvvareba.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/guldvwlvw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gxkttheor.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gacocnkho.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gtnzzizhi.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gexeyumhj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaiexvdpd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnneizbzm.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/ganuqxocn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gtlcuppma.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gdautzlih.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/grzdxzdoi.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gxthvmimd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gfiyljseu.sHtML


<!-- 参考信息 -->