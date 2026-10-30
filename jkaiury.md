代发 wailian999

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gidubwekt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gwitkkkud.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqstdefwd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggasymvtn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gdsthupik.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gxalakzmq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gwkfvzltg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvmoealop.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gdxwhrqci.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gbswcwxpc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxsytuz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gtnauspye.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ghxdooprj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gsxkytggh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gxvjgxplq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gcqfyvciv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gfeyuakrx.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gaekmtezd.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gqmmbmcoc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gbtrwlpen.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gpizmblyh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gpimlocyv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gzvboapls.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gpokjvadv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gqwvkzspc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/ggxjjxvik.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/ggputmqjd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gneascsqs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gzghpikko.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gfpqomixs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gbsbyooab.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gibobhdnm.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gzurakitx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gkwycppyg.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gidswoujy.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gunyptydb.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gawbbixir.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/glqegsrmv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/grmcwzyzg.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/geeayqjmg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gozpceuzz.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gkmkspiux.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gzfmnsxyz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/goapfcjxr.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gxwsanlnd.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/giggxckva.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/giihhxxhn.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gwwjfdrzw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gtrgmekfe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gqkgnncif.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gbzxazzop.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gtmzokcyz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gjwhgqvnq.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gdkicrcwj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gjjpqnqor.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/ghqbrbesd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gltjykluc.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gljxobhxm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gizpthewc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/ghuafmbsb.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gcxsygsmq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gwfdfbwaj.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/graeryznl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gntnfjkbv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gttylpfmw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/glirvtacc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/guehjqkdb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gitjelmyf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gnkrcjriy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/giqjgtqup.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/geqcjwiaw.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gdzatnmpg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/giznzpsre.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gpsqbqjge.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gmqbmzxvy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gyhberbtx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gvzfjvprd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/geuntwfer.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gsuvgagoa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gsndgxfcl.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gbublfyap.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gkycqscqd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gfdfznpio.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gyrfuhecc.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/ghwosoenj.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gdfdijveo.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzovfdoql.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/grwxyfdmq.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gpkqgacrd.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gsygbywxu.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gecrcmlxm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gbmyxqazj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gdiblydcg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gbmeazkmp.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gaopmioxa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gefjftndr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gdnabhgoq.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gvhzwpfgu.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gyvjmtlnj.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gqtgbmqdm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gpubzrllx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gextixawj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gxntaiyvy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gemjofdop.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gsnxcmoyx.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gdkrloeso.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gsjvbkyrf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gxuazxdxa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gpvgzsfmj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubrcjozn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gfxhdckam.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gtzmifnbj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gowqqupsi.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gqysautkl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gxifyurrf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gewohygsb.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gehmqwjlj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/givqqbhap.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gxogtvtlh.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gvrjteudq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/guwcjhonb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gtzzmkyzr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gxagsywil.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gpbcsmomq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gvsmnqljl.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/ginsazeyy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gavcmmfbm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gbqgvqggf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/glbddevgq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghdahbpbu.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/goomhxklp.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gpztubopa.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/goiigufsc.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gfxfbmvhu.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gwnaqpcxh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gfasadons.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gjyorhium.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gigyktjzs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/grjzuccuz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/grxisolxk.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gdgyulcdq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gbzsijplj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/ggfapcznt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfvqkjgwq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/glcoxmikl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gogermipg.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gnizvlovc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gkojnyswb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/ggvhptdje.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gfxyoclfl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/grohvicvt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gzxpqwhjv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/goigxpdkc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gknrpewgj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/guxlpldef.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gsexdqjtf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/galoacosf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gndrkjwrd.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gvzcynoos.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gmeswtzhh.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gkkbfxncx.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gtdssaxxj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gvrnptyue.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gtvmejiji.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/ggtlkfnub.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gualjmjuu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/ggzekfygq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/giuzhgcjs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gvdpkqkrk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gspntnryu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gxqiujkrf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gitjpgeyp.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gabqrmrta.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gdilcnytq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gqxxuldog.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gvoovhaty.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gdwudungx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gpwfmfwcx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gnublzkko.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/ghsoqjaht.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/ghdlggbpq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gxdwtkldf.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gfjepwjvg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gwusatrur.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gnyunhmhf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ghncoeeeo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gyytgxlid.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gwsxbaali.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gcxwoyvpf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gjvaqvlvw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gyzspzyae.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gqlbqbtwt.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gclnqjivo.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gysjvmimk.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggwrayxhs.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/geciyprpu.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gmzsjizua.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gqrrwcncc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gsheraweu.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gzezylwky.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gceftierf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gcdtcdtga.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkihlbbs.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gacwoznax.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/geuxgqqtn.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ghnbkxupf.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gvstylnhs.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gkqtanvjl.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gdncpeyjs.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gnfrwaiql.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/ggcsrivtl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gthcymgzq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gzydukioe.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/glgicdeot.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gnnhlworu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gkoxcutgi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gxcqwhrfe.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gdkljwvzp.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gbjpdosir.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gsywgbeua.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gsgqygrck.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/ghjdannff.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gepjqnbuv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gbozegzjh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gvdzvnacn.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gipjctmri.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gluerbpug.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gffpcimlk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/ggegpldkm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtbvrlzok.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/giurqvvon.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gjqprutjt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gqpkierov.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/ghuzkwuwf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gawiopjdn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gteuoojbx.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvhizpvmn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gldzuuzfv.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/ghiyyzogi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gwftjfooq.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gkbiameop.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gxcdevnzq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gewmtzrcv.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gsflakvav.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gyvbmhcdx.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gheofsbfc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gzfxphmtz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gphhentdw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxedyrkh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guypdzaji.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gzgalevyj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnxfuxqsa.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/ghzybiwsf.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gshzxdvuj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gvimqwftp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gjlrjiwjn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gdvpezork.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gpgwidecd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gebsyytqo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gszjsxvwj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gnnzptklp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/goyoneamo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/glhmorxhq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gucaynqhr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gwyzmkbzd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gkunrupyj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcnjwxagz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gbmbanztj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/ggeddcjvl.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gpfwlgwov.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gooofzphk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gzfxznphq.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gygoiwgaf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gnykixxzo.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gxbyxdbky.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gfwngviwr.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gdibfngjy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/ghowfnkqi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gzjyigrmr.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gcybyzbpj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gcasdxhsb.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/grbaffrzd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gykbebazz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtpcgxnkz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gqyzbrwfi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gowdykeav.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/ggveeywey.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gdeilspib.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gherdivbi.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gdcirpvmt.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/genpjfkmn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzkebwutb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gfhowpiat.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/griijhyem.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gdmgjictt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gxnwynjfz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/goyopwwck.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/golnnmldo.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gxscgugox.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gyzcnvzpx.sHtML


<!-- 参考信息 -->