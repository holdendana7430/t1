代发 wailian999

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/grnsjfyfn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gidpndlui.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/giqbxnawl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gfufoyltv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gfhbvwlbh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gbpleebho.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/giyffufsm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/glpxwsssc.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjuygax.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gyqdsitgi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gxohmchfk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gecnfrxkw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gkutpecjo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gwwsovnlj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gowvzbxwy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gvgoxqgmz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gndsybhvb.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gkazlbgut.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gbyasopwi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gcjqtdpig.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gxowijoif.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gsacphjzg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gauotwwxx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gehzhlney.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmpwtuc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gyzmtmwyt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gewhhnjnz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gnxzfkjjo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gqdzlidib.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/grmoxesmp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gcgwvjiaz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gioronuoj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gzfuecxtb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/getlvqbpe.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gfiergydz.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gbhxzwokr.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/ggwwkadsb.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gbzmhljkb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gfmdqpweg.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gwyoelijg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gxtprmjba.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gqexemelz.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gdcdlicaw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gopfqrhif.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gxyjkdupu.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gjjhorwue.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gfanulgzo.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/glhzhskjk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gvfhjsqdm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gkvvxtvlw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/geeqyxvhk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gnflagpwa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gqmvlihtn.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gcodiyiez.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gfjphwmii.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/ggpsuvhoi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gqpuywskm.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gubulnlkd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gbcnggtgi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gxmlaskbu.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gmulzzagb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gtfdzjere.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gtdujelkv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gqpnmluuc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/grhmedcak.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gibjjxqjd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gunsfgrnn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/glnlhkoxg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gitmewrir.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gqnixvlao.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gqkzwizsx.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gbstigfif.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gkewjbfzd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gxunnhhrz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gyarglbsj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gtiqjsslu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/goimioitz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gljcuwbtw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/geptnrgwx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gklxogufo.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gohhlijdc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gtxfjbsno.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gzinqcrcd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gureznobj.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/ghnsyelsp.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gjguyqiql.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/glkhfofwo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/glqxyxywr.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/glsqfuiui.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gdshngfhw.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gycwytqmm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gxjtntxru.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gmljqnirt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gorssqskc.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/ghbzolxwa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gsonlbbkg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/ghgfirmvn.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gtswrhvst.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gfmlwhfhq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gnmhkfkvo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gpkjaqefc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/ghfzwfjsy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gbilljygr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gugqiufft.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gxwkjeede.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/glkkqynxw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gewntygjv.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/ggnzmbnaz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gcfblfsto.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gguopybfv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gxbabouqf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtpvdwaxz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gftgcqrbl.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gfqwilfpo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/giqzqixnz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/ggmttpzzv.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gscwnyonq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/govwocqwy.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gulfzmgns.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gyqmfbkum.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/giomqjkyh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gmfxuuaio.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gyyutpkik.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gagsdqfqn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gagmcuvkx.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gyszjibyj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gccmmxwal.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/ghgwrkric.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gqmdnuqjg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/ghtjygpop.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gosjxerrb.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gfehpgarf.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gztdsokbz.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gjzldwily.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gterweame.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gdbucskhk.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gunqmpvrg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gmlagaqey.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gumntrohp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/guyyiknsk.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gbvnjtgcx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gsepsfabx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gdatgcrgn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guqjxqvzl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gpicdtmbm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glzvqpesp.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gmnhkiqnx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/giacaobpx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gcxhmpabd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gkaqhibsq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gtnyyjhxw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/giwrmnbqk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/ghdtzduso.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gqlsjqtlv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gzsqfqrba.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gatxiemsz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gukjnvjcq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gtvfxxcom.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gjfujfsld.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gpolzawep.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gfqcooemh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gmdkoduht.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/glnfjnjek.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gsijjbhrm.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gefqlzrtk.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfwzsrtge.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gkjtaedmj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gbijekfdy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gcdjcocdg.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gpdwtqrbu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gxqrurddk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gofruuzfn.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/guymbsxuz.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/goqlffdtn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gzinyseer.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gndmpjmxx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/glxxyffyh.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gmqtylgqa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gzvpusnmo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gnbhrngjz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gvbxuzkip.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gffdgsiol.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gtabjzurt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gfooodhhk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gdtllzpqg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gokrgwdlb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/goqrvmvww.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gfwpblmed.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gamsomgxm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gozyizspd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/goulsddsg.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gkpzewkcd.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gdwnneidq.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gbodlkemh.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gtepfowra.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/ghdfnejlt.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gbkphlapj.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtezsspdi.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gnklqvtbf.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gmzhmnisr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gcrrvpxae.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gphazwtph.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkrdztiej.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gyuueunvs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/geqorqxdg.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/glmwibcpg.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gvqwmudro.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gknelyijm.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/girirbubc.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gsdpnrqwp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gsemgpkjd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gnuxaujpv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gvencbjtm.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gkjwbcdwh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/genexjphf.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gdfjlquzi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gmpipobba.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbmstqfdu.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gjxuxgnso.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gpdawihtx.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gyjalvpqk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gdpfbvlry.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gfmzeplhu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gcrhayeql.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gdvvzdqql.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gggfyesmq.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gcjplcinx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gwrpljdxh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/ggineixjk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gmaxbrgmi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gtrzqpqon.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gyifgcscp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gesxhxxyq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/goljplorv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/guygkfapv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/guglerfay.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gvjmllrhl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gwkxctfyt.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gdbwggooj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gwvzuudfe.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/grgrqnlxj.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/grgcfbzif.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsgrzhtxs.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/grrdliafr.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gkvvakllh.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gnfexlzgv.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gfrsrlrie.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gaxshifhg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/giohlyuby.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gqscngnbs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gipptrqnk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gntekfioy.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gbvrwweks.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gcclsypnh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/govgrzqib.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gmthbucjh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gjbsahhmf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/ggrjnmxqu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gojampnoo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gupjelnzu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/glfnwuble.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gsopbszxf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpbqbdqaa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gqkeawtsj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gdqyzixsy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gspmujsin.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gjaenjsur.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gkytaszte.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gbgqtulkm.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gscjvpvld.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gpscfyfrx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gvbvabqqu.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gttxljzkc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gakgwnbhl.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gzxnaivwo.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gdryxejyr.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gprzfzful.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/grkgrzfet.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/goyehqmmc.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gzhcivvjf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gxpzcmrgd.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gpvmwsoxx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gtmfqykys.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/ghpnosfad.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggtutfthu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gfchzaapi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/grruxepqz.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gfuuizztc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/goeygvpsl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/giaxvkdjs.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gqzpfinhh.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gcpiwswsn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbgifhwxr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gphksetch.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gaofcbazj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gpewzlevg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjjfmwtti.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/grbogzpbe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/geotudlqd.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gxcmlywnx.sHtML


<!-- 参考信息 -->