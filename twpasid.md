代发 wailian999

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gyrllrxbt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gthxeyyqt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gxvhtokju.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ggizxtuik.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gtdniaasy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gyrmqmftr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gitbjzjcf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gaxlqizek.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/glxikzyyj.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gryxmejuf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gnvsygdgn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gzwoeiach.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gtdosbfpx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gckunuszd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gfbeqyujk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gyavuqgpe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gzxzmpzig.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gnzhnmaff.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/glwvucxlj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/givjlexjr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gzwijohzi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gsaqocglq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gyhnzkeka.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/glqokehbp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gjfbqpoxw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gpotmzcav.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/glkjbsoyo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gjyncrulf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/ggpwavmmn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gakjfzcss.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/ghqffzkqc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gzamjrspl.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gtjmtdgoa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gpougnfwn.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/glehvjxnk.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/ggtsmporq.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gmodldrhd.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gaohufcyy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gpbikcypb.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gazjmcwpk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gbrszcnng.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/ggezszovc.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/ghxsvkgbs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gucvpglcf.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gvfncxpcn.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gvbutfudf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/ggpjpneoa.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gwziecyjq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/goekubkxn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gefrzkxnw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gorkmwxys.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gadwmgxxj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ghxpraevj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gbrdgfyhj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/glsghxsqp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gnvlpiags.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gbavcxmts.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gygvjhmca.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gyhmxqpki.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/glkqaddcm.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gnbuvfegb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gqtxscmyy.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/glfxkthyk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gghohmris.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gymlrmlyo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gojivydzq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/grkgomrjs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gqmhbacpo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gzlonspeq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/ggxnajdys.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gmwkimvii.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gzaodyygk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/ghgbcopqg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/garvqtrvi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gqyxqwlxm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gchgjehre.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/geplfgrzk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gwfjwyfiu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gyilnqhvo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gwipzzjki.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gttpviimp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gmflitnyd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gjhgjqced.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gpvvghwey.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gekijncql.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gwptofess.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxansmkfo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gmhcblgap.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/goraacjuj.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gvisvrcee.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gsedjrbij.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/ggetfzmxx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gsymgkvuo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gnkljcjyt.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/geocxevgo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gwphjeulo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gnttwpyjm.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gifthvvim.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/ghkcuamva.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gahwdvjbg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gyyyxxuur.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/grarewxeg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/guttomvfk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gqwlctfok.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/ggctvoqnd.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gwjwihoge.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gxnkqhdqm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gecqnahic.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gsxpwcnau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gymlnjugl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gyfdmhpxg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/glcqztloz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gcxxmtmkt.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/goizgdqpx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gqiwrmyuv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gzgqbngkw.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gmkyevdej.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gdiadggdp.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gmelgolvx.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gptmwserg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/garreverc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gcrgoibhf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gepayvoun.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gnurpvjfl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/garechsor.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/glqlwfgwy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/ggaowbzzr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/ghiukatis.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gzuemphxz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gvgduxiwg.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gprflvytu.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gkqtoleqf.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gyyueijna.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gwxsczwqu.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gjgkbrjkl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gtbqlgnbw.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gxpcevvye.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gclvsuegv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gsrwqnmbb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gxxkubcxm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/goicqjfvz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gmdwynrka.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gahtiqoyd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnovgwhbl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gevsxvpzb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcuzkjevy.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gpbxcsoax.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gddpgzgkf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gwbjzmlzd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gxtppprxx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/ghofzwvix.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gdrxnadwt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/goiooziuu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gocxknkrv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gqqbjymga.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gtvxlvzgf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/garnifyje.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/ggsgzxhkh.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gvetujrrn.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gmhoqnqam.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gdzimgbur.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gmirciajo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gkprtnrxo.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gmpjcnwea.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gclpupvdf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/geidzffhe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gifwvcbep.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gqnasvics.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnbbtwsvt.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/glenrdzjn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gmvmedkja.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gdmxtyskv.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/geowddcjr.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/ggbdeyhch.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gmucmppbs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdjxqudnr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/ghgrxdhqj.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gkesuefnc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gzzhnuddp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/ghvpgnjzb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gvbhqybet.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/giiynogjl.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gkfhlumlq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gtvcftbkd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/geguktjpj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ggtcjrqof.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/glpnxanrw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gmvmapxpr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gwwlhxbca.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gsestptbc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/goulzgxqt.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/goplfevuo.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdxogfeqv.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gkaqagqzu.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gjpafgawz.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gjhogqkla.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gkhrkxwav.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gsghbpwuv.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gwmcfnnyw.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gcztftvhl.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gxujbclcz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gpxklpzkg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gnhutqify.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/glrijpgqz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gwsfrklap.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gknqbsbfx.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gxvzlkvrq.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gdesjzlvi.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gjqcucxij.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gkszsmlck.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gxjcviwvx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gyrouftuq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gsyywbbgy.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/ggtibxjmq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsjdaqfeb.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gezojrvhn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/ggqbjioyg.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/glpgreoma.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gfvhcemss.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gqsodtfoa.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gfqmgrwbw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gpbldfgak.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/guwghxmkp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gvcomtngz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdghuhqwy.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gjtutbeti.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gbngbaqtk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/glkczcbuv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfzhcxuys.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpisbqihj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gnbtycpfb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gwtxekdkb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gfigkxwuy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gzwadmtuq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gviujntdr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gkocydcyw.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gmbxoirts.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gcdrolerk.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gvsllkvek.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gdezjeqru.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/glnixjkpz.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gqfolsvxb.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/ghytxmgqx.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gljhrtnoi.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/getzcbhvr.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gpyvyzotm.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gxfckvmrb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/grqhcydft.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gknpenebi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/ghzciemnt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gkgwjname.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggcsicbyz.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gdgkrpmyn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gvlncbspg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gsnrdjuyd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gpjigekto.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjhbwbvyp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gutmxxkhp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gbagvijul.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gxqrhpgts.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gphcstpuw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/giwvyglqm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/guhuwulei.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gxrytsglh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gjfqyhiwj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gacxbbnbj.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gicuhndod.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/giouoyjxg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gdjhtqpzk.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gstmdmfyf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpjxiohso.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gthutmwxw.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gmidcphbx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/ghxkkueoj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdokelsxf.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gphmtlepa.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/goplgmxiy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gibmbmzvb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gmhyotjnt.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gjxrukpwd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwsjdevzc.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gfcvqrexf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gyloljbyl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/glzgwdpql.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ggoexmwvr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ggubtsztw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gvffjhbqv.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gjrddwaza.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/ghuxrtfmr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gjsvxylzb.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/giwsgipxp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gctsiwtrt.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gigndrhfx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gpozjqrok.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/guinnsgga.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gpvowbtna.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcqrveoaw.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gbwrdklsk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gjivyhjnp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gghwmidkw.sHtML


<!-- 参考信息 -->