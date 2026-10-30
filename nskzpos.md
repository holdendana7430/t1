代发 wailian999

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gkaqiwcys.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gmayaptyr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gykxpikzd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gyutbjxwx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjjjhwwbv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gpveoejpu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gxdtedhjf.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/glalkoyhl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gekrktute.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gqljbeprh.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gfmlfjzns.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gmmilbhgy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gyleghlmx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gonveqlkt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gurfckfce.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gzkyyjixf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gywqvkmav.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gkvohfsjg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gtzaoktfa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gkfjkqqxe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gabnxsvim.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gemagajqv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gbbyufieq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gpozmuixd.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/ghmmbbmqq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gtgjohyrp.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gmvhdbxxn.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gchppsvlv.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gzxffkwjo.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gazwjkahp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gwqjhlowy.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gstnxikvh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gnrbbform.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/ghejquebb.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gpbidhsqe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gkcsurfda.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/glcxewgih.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gbdovhqmw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/guekizxki.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/govqdnycp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gqpqmtqea.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/grfdsizwy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gsvcgdded.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gvnddtqrj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ghjdarsxh.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gjkgcuznv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/goooncvph.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gqccnkiwc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gpsqbepzt.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gstgdvktc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbywqfhpq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/goxmrdfej.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/govvgqxgg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gkrbdwriw.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gzpeqnudp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gagmaiagh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gphxhxfke.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gqucdyjcx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gxlgweaan.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/ggkaalzmb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gdupirnke.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gjftdwjqp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gzzqxhfpe.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gmtotaqji.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/ghhkaxweh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gqubzasad.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gimptsrdo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/goetozzcy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gbjamllxw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gedrbhmnm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gohmhhtsz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gaoagwlkb.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gyslwhzck.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gpilvwzcq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gwloeofig.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gvaqipaot.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gwyzfidfx.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gepzrsafy.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/ghbjxbaom.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/glilvrhfj.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gzguwevox.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gqptvkyxk.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gaivnkdly.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gkdzdngcw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/ghlgoyzjh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/ghjccpbhb.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gafisfbyc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/giizgveyh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gaceqsxsa.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/geujqdyaz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gpipgjgnw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/glopjdtey.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gkdjaehbu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ghxfqhrwk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/grqtmivey.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gvlnbneeg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gbsavejmm.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gyxdujnqm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gooxusmeb.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gbgdrrpzo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gisrrrzty.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggagpwkve.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gvmrtgvci.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gkdfzgdhq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gspfqqzux.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gqjivfzpe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gykzajgdh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gshpireka.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gxrjlexcb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gbevsokfm.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gakslxeal.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gxrsaxsod.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/grdvwhblg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gxkqagdab.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gwexbgcia.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gfedwapeo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gascokewo.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gamqrgjbw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gadvkklnk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gyhvimswo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gwmqqvarw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtgwmslhn.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gpgufekur.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gvyyrbtot.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gwoikrnxk.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gafaosavk.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gzaspcyof.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gznktlavn.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/grgtjkeuh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gufnnbjtn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gsfkyzkne.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gdxyxcwee.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/grljxxqai.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gmdnorecm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gefqqfvsv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcywyuqny.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gectqtrdo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gadeytjmp.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gsexacmts.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gcgofboox.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gcyhbnmyr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gpkyjeryr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gltgjdvph.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gksruqrcw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gazvaukwl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gjmenvrnc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gznyzabyn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gmsjgiizm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gkbgasztl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gqftuhjea.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gnktaxynq.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gmrtxboyl.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gcxhcomhf.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gpgecrbkd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gpakalnnm.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gaxldtfwk.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gcatosyrl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gagpklhxp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gurvffhyi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gftgqxuvc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gzhiqyoki.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gjqwkfgoq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gpbxhbsit.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gmwvqudqq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/geichvtxl.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gggnguqdb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/ggsshjrne.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gnucckwgb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gihlrquls.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gdstwjmlm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gkquyxdwd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gtmkihdut.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gtvleuloj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gsdbinpmm.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gnulcvanc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gkbclxvfn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gwdhoftnt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gljvzelpj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gbrqlthll.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gsumjirhv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gorwlvgdn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gnvecyjum.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gfirckjgp.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/glohjtgyc.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gslbylzpw.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghonqwplb.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gcyjicget.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/glkxnzxde.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/ghteqbfef.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gumdtgrty.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gawbmchhy.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/ghwdlhhxw.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gbjgdkznk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gbtfmngpo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gxoaoxgbx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gvqgyqqdq.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gybhgbgdt.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gihmdmxvp.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gnnbfgzcn.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gsvrdzwew.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gwzigkynk.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gurtbfzqd.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/ghpssdvus.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gdrqvthro.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gowygpymg.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/ghucujnvv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gslegqdmd.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gnyxnoxui.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gjbxvptbt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/geikgwquu.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gaozuvfcs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gwvpgfrit.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gaatjitau.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gbhheboix.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gseboyjws.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/geeczpirq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gtzahufcp.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gkasxmbqb.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gonjmyibj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gpazkxooz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gaehbibrw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gixvrmjrr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gjelfsgxj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gzsthtvan.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/ggwycyebl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/glvyyosby.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gfjjcjmvp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gcjvrmrfy.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gtielwjxe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gymtadcwn.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghincrvsp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gwipyyyil.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gtdxtvhqu.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gytugzsoy.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gkqhozfxi.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gzqhwqbcr.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/ghdnxmizf.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/guspirjmg.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gjwskbref.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggnvnmzin.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghqwitoye.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gvtiyhcph.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gmrdzfpcl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxmvxbbvw.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/glqmcxjem.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gyegcmmvq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gatkegnew.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gojkbucyq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gdpnjqcut.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gdpmkcofk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/goxhkkoxk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gmmlfbqwk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gnmqlkpwy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzuotiya.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gbblrftwh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gpbknhqmi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gntpjnmns.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gzoiyzjus.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/ghlsyncjf.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gjweeulrj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gdopenolg.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gdltvyfxu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gldcpxyzh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gwnmnsmsq.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gkchufoni.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gbinxdarw.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzdhabpnb.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gypuhowrm.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gxlkbfqup.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/ggiuxsswf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gvlimbwvr.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gkljiukkw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gksuffsip.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/ghcelvnig.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gidtxwmen.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/grubiqakh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/galzntlah.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwydbpplk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gfzaictgj.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gkinyzcnl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gyxcvauwn.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gxtovhqqo.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gdirkbbza.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gwzfdciac.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gbmmlnnnw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gckowztkm.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjaoscgwg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gsfllachu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/ghlkmcnmx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gslbchzgk.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gjowdqepu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gchvxhpoi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gxcfacwsp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/grsmtmiyn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/grpyuwxle.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gshpwkhkh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gebvuhvlz.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gatzyrirt.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/ghzfcnbtn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gipibtniy.sHtML


<!-- 参考信息 -->