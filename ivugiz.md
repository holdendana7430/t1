代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wivtcsus.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jbsjcthn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qpdvprxn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rqbhpaay.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wkhmmalu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pdijvfwc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uxslxjgg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2flxehynk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mzapbguz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2iixzeuzl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tcuypceh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ifcoflgj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uxnwqroa.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2otrrmrkf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vxdmccax.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rmqxkdto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhqhjmol.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wkncidoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2miabtigu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjohsqfg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rkiesacf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpzndgsx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qmzkzfuv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohprbooh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyaolegl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2uhxndkti.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dtdadydp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtthtmkj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpmxygpt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xotjoawn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ctssksao.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2toxwkkck.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2spmsfjny.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qgeiixgb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhuhglhh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2efavmcwr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2fmaaegaq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2epiqltpq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rqjctfju.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqspwxja.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jnzxzyhj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ayxsfusr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yscnrpls.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qnflzsnq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hggagtyb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2sjdqqbom.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tcolaxrp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nvvmlgjx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmlpqlbo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjlgdned.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jzzlbllj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tdwtidav.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zeuctczt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eedtyzmk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhaqpnrh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kwmceqvj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kadbpsdf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2xaymdyil.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qspvtliq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nsozdujq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2udgfztlt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hjihmkcw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2suiqrcpc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xmguwgrp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hxitrery.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rjqajevz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2flqdxgqt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ofahmvsi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cxetnvsi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xzanauvz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2njeakyqe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zwqeromo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wfowhoqr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2cunmvgcs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2iyewzden.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2baygrqxq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzjlptc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wzgsmphw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oojymhtw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2imoehnpf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ejntrnpx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2juybzxme.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rduexbtf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lmnlnynv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqitsehr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcwldvmq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqefcicb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nmpccxjv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2upbigdxf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wvkdtbux.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrbynorm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ulidmnax.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ziyuecin.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2axxmxvkk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pxirvili.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qzlydvev.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2onqqzyjd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qltiijjb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlljlqul.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jklmoqsg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ljtgdhyj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gztvxtyi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vooyedgy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2separrca.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dqptksyx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2evimqpbb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xgmgvree.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2clzrshki.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bntffpce.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jkavgbdg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tmqtjdiw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2aihifbhi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2liolhidm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wmilblie.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rekvlgwq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2exxbovsa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2tvsmhqaz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrvpvd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ikezxije.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ywrfafzy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jvevkyax.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iqtffslv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dtrsbdwz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wxzrzqlq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2phauyafp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2duhbaxxr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2izqvabbb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2odeuxpze.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fwkiailr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhzhcjaq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zxsxnouy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mhozlihi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fqtqeayy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ghymojyj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ynxekfgk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mwfqejvp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtoaqkgx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ujoykpzv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uirbrlne.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rgpheyay.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dzvldxzp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2azetvsrr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ijppuayd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kazyethc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2rjwxxlwb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2actehzce.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jwfdridh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kmourelx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppronyil.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2euwlacvm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2neljqgvz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gpbxhvpg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zkwzwnqo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2axmquwsb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qlnouufh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kfhtwxjf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mrzgilcs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2bdjekywy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rzoqrbuv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hvxfyjtj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cqhzlfmh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nsxmtggx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlskhijt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yofohttu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2plsdokgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuytopyi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xokuiixr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2eicebmrb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mmoaiduy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eucfmemo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2msxobudj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hjyurjan.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2boyxbiuu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lsqfrlgw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jjraftwv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gommejfo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wymvshfe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xqwxbowe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kcfoitvv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ynxxlyzg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2sokuafkn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2iofeygpl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sywxrgkg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2omujzosg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ltrvescq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2htxhveps.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tbkqnbdp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ynryugsj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gpvguvvd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ncnmrscj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ynnlbhoq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rqdqthza.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qzstwieh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2tpssgxal.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2htlrjdfa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rircllya.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ooppzlmc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cixhrzuh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aaowzzhe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2hmbsyvrv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2yxxxhwmc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vqbyzuyo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rzphhgdv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tpzigkxr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vdnmmmvw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qvbsqtdk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gjihlklw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uxnhjcwd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wrvaiwey.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tleegaih.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fuvzswfx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2enourxbw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hgekxweo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hyhjsjbx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oudnsrsm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ojkrhpqd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ymmqhdew.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stgwglkb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vbxyfdtv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qizrtvvs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bkwiuukb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xyabxtos.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eoxwvcaj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bcaivpvy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yfkqxpjs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pjuemkyd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2sgqdreyl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qbellwob.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2osjkcwjq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qwvfuuea.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbnueby.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fbcbiggz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2eymuoxyz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wmalbldb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2paefxhyu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qjeypvog.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2dfsrnbzb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yowtkgpy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wptalfnx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tuovqmqk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozdwhvxe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2uknucrgh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qsyyjuto.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tdxflnrc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2klhgqttv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qexzoecg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qulcqqxl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qqlkxuuc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xroducdj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ilscdzcy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2snwpfqtt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vgazvafm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2htptifvb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mkuqkwda.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2cabmflgs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cravdxwd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fwurjsra.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qtttfbgn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wxfoymni.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mlecsthx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jdecufkm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zyktihdz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xptpgwal.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2denuviln.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qcderyvq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ndfzwcdg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wcmqeijb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fdtxmhfb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkazdvx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2liffzpir.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2becuvlrh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckiqotxo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tighwmkf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zctoginr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2sqjzjdsw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zsbbvhdp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jsocmftp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lolxywtc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxhnlrfm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rdhqzexr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mqpcxjmi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xkdhunvy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hfudejhy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hfloksgr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hhpblgey.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fukjarwa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cekfbwsx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zokvcttk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rphxwokn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2iyspuymd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2prijmyuj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2btupnsxy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ujgssoon.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gbifffar.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ngpadinf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uszfeokb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kmbosqeg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2gsraxjnt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xupioseu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dwffqkil.html


<!-- 参考信息 -->