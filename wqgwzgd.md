代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gyxgboaiv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gvneldnot.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gtrgodady.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/ggddwmbie.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gdluvqnek.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gsmrbcsyd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkyahniy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gqnhdamav.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gnpxbvscl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gdrkawpje.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gethtkoml.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/goorrqhat.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gawnbxlnz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gsprdeacr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/ghmqreiqx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gnspkbpel.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gtwdmbggy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gbtwqfybf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gswezyacm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/giikyqntd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gcspwsyyq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqxvywp.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gtgizezxz.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/grwnqkggn.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gtkwgrwiu.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/ggxmgvedn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gpkeepilf.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gidljdyag.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/ggqyzklwq.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gnmnwekda.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gyosokpsq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gxsantiwn.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/golxiejjf.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gujbclgaa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gltxvrdkc.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gsihmaeva.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gktwzqmvs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gagkjedjr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gdvrpeted.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gokvndubf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/ghetnnlsu.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gtsridhfr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gaekzbegu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpodnddln.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gotxyzqvd.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gsibymuhf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/ggehpkieu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gonoinfpv.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gfhjcscnj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gklupokfb.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gwjbecauv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/ggirioyuo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/ghecushta.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/ggffkotrl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gmdbktajl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gwsnsvdpd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gteunzzvg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gxihesvmz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gvnshghpn.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmhwafuxz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/grgcbuvas.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/ggskzkfvl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gljtifaex.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gxwliexvb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gcpquluvi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gdlcfsaxh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gpcedsfkh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gculpelpd.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gmlhaibwd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gsizonphj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gqcisxmye.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gaueiwhol.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gfwwakzwi.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gbdzmowtu.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gfarzwwit.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/genpbnmcg.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gdrzpmgfk.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/guxuzrdom.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gzyjxsmil.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gnzodvmxe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gszrkqyjy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gqethwfxv.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gitfvmgrg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gfaudnqvo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gyjsfmnuz.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gwsluwnom.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gotsudgju.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gzgblhrcl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gpbpkhong.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gubfyzhen.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gcqrrtjiv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gjtzarfwy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gzsqsjcke.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gpjuyfrlw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gekmncddn.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/ggarrmngr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gexhsxbom.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gnmonvqim.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gnoqsuxky.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/glgxnfzoa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gdmftctwx.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gkqmsqbgy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gjunyppxm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gblwdosvv.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gtycekfru.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gphvregea.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gdazmrbvr.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gfmlrtzfp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/glfesnpya.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gfxgywzwi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gxkhyfeph.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gckpcceup.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/ggzxnvpyj.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/giconyllh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gsyydxkus.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gvhzcysib.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnalhdbxm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gzzegqnuj.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/grpvhlpxk.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gcostyswv.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gvsgsohrp.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gqxbzhfwl.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gvghlymrp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gihaxzxth.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gdilpydlu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/ghxsbgqkf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gudwzyjpx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbovekflj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/glgnvpcoy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/golzfndlw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gkltsgmbv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggajillts.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gsqtcrqra.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gocwcnijk.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gfnjndbex.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gpzjqbqtz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/glqukuyzp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gpnfztags.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gxxitzrwg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gnbrxwssq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gtbwlghyx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gzrztukrl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gxhjktirk.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gzptnacns.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gxxbwrggv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gwukpjgao.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gxmggtosm.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gmlvzetwy.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdhlkekzl.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gijubbqob.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gknndmpwc.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gftodqidl.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gkidqpeel.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/ghvtbrijw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gnahjjzth.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/guiewfteq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gkngodmyi.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gsepgmiqd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/ggkcagckf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gwweqsaab.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gkzbinssz.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gsswugroa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gtyaeecpa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/ghuikbsnz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqcgyjr.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gqalypkkd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gefwhjuvf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/guutdgfys.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gpxqfazdk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gajtimctp.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gugbvwegu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ghyouidak.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gemfzmvnt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gvaxmjedx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gzdknjmni.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gamvhubma.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gbzzgswfw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gtpcsyxvd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gmvaxxhag.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gdaruofln.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gcmaggpyv.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcylmconf.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gqjsiqwpq.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gwxiqqxgx.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gnhjdnwhw.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gzuxzrzee.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/ghfovdkbg.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gzhhlfuab.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gndwychuu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gjafpedpo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gyavipcjc.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/grkjsgbis.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gisltmskz.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gmndeanzj.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gpcgghrmq.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/glnktwaip.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gthrnictr.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gpzaiaaar.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gokpkzubu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gcxogbxom.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gnlwksbel.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gipbfuoaz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gpwvyefwj.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gtifsjuqm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gnzgkgbpn.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gidxjktcv.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gfxabfsyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gkbvqsybf.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gimxmpvpq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gemvwbpvu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/ganblhkho.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gaaswjohz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzwxdnfpa.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gbezxpsvq.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gknhqbjld.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gonpvaipy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gxqiabzag.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/glzksqajd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gcwcxpecs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/glpfmyuyl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/grvjfjsuq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gfcelnsjv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gsdtnheqq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gleamegli.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gnouatlda.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/ghjxqagxy.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gmdxrjstl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/guieofelr.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/ggjbwqkwr.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/geordhvgr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gknqybrjc.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gmvkrlziw.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gzvkleebj.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gawonhsmv.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/greycnmes.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gqvpbfxej.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gvesvydma.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/grbgfzzyq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gkeefhroz.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glpylvcjt.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gkjqnffso.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gskjmulpn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/goyzxypod.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gipnjxmdb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gkkxuavvo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gbitskhec.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gvuzvkehe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gjrabjizp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gagevjkrc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gascqgqhd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqaqxwtnd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gvshpibmy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gdhfurgpv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfoutzdia.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gxmifycto.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gffnywmnv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gimsfvmst.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gbgcuujie.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gtwcizwhn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/guwiuqvpo.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/ggmkvskkd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gwojrlzsq.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gedbqatbe.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gmhnveqto.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gfxxxzvrz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/glvojgfib.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gybwamgyl.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/ggvsyuvyj.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/guzruompd.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gqxockhbr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gobudmflm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gayoitvhp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gpeejgtvx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gxxmvqjdl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gbckqwcmw.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/grsjeawpu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gxnszcimo.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gjcrcpxbo.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gddodgvyq.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gpjobatny.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/ggzrpnpky.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqobeipfi.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gjaldegsl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/ghbkqyovw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxczkmnry.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gycrrpjvv.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gdullpfay.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gabjvlvef.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gcprjdnir.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gqbsuvanv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gxvuvkrvf.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gzjcuayte.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gnyrsnzja.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/grbrnsqfz.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gyegujwgi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gfaxsytak.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gqidnxtwf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gneegxupe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gkagnnijh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gncqronsl.sHtML


<!-- 参考信息 -->