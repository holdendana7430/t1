代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gsrkpdven.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gduaynusm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gjziyxzyx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gueatfkex.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gehskkoaz.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gxhyiueio.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gllpyjshd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gshxrzdlj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggdxesjjh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gviefklgo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gsutlhgft.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gpktlqfes.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/grwmrmufd.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gfdckiwod.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/ggejnnxdj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gblwyqcrk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gsomboiio.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/grkujnyuu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gsvoaqpgt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gmaavimij.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/grwtzycyj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/guahynkhk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gzsqcvzkw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gerpsgqlb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/geszsejdy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gzlyoqlgr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gxockgrra.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/galzftpuf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gnzkfpgsr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gemhurnun.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwramyiyv.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gfhqnjnkx.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gcstaplyx.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/goxupkamn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gdlwzkdgv.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/goggwbjkq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gricfohkl.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/ghefvgqsc.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gpsmouccy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gyskpmrki.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/glnfzjlkt.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gdebljqlt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gelvdmocy.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gtsdsupga.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gorzzpaiw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gigfukabs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gawaravot.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gianeknqe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/grgohlmzv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gzoqjistd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gammadqjb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gkzmfojxn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gtenxejbo.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gdbwpunox.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gjdpgrzon.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/ggiydelnz.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gueycthjg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/ghhtoikgh.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gagrlafox.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gtxembnzw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gxxszbnrc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gdwlgenke.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gajqeuwcd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gznlzygho.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/grviviisz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gsamvcpzp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gfdrjkple.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gnmblounx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gqfjylwaz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/ghljmbzxz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gutcxebiw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gwdnrjice.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gwixflayz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/ghlnnhqnj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gghfzndpe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gbvotjxka.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gecfcvvoo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gcacgekoi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gitodwuur.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gaetmhvry.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gxyrjfxmz.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gduabehsm.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gyyoqlcjc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gotcdisho.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gvepxusla.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gcmvghxpp.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gcabqxpvh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gzsufotzh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ghiwtgaqx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gtimoerai.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gymqhqvct.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gcwqwclcv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gxcbgymfy.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gnvgcsahf.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gcpjfwjgx.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gpgpsxcjf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/greorzeqp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gjimcuogv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gbalfsboc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gzxzjazbr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gzajpcqcq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gzbochuay.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gfzheljgo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/ghimwnteo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gmbbtotdc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gsgzfnmlw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/ggznkzyjw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gqhsbclfw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gpwwjszdq.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gbcpngnin.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gbxzuutom.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/giavizcjs.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gsgkekjqu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gifvyvwkt.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gqmgkwvbz.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/glgrxdeji.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gpzgmhtfw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gsdwwbzlc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gaxqowoxa.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gvmdibgit.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gauswoptz.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gyxmrqgau.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gsmfelmmp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gieahlosn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/grqtqdciw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gvuoetclz.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gvxvprmvu.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gapffnetq.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gzwczjghl.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gkavnpdco.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gnnpvimvo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/giexakkho.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gjhvcjxcb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gphtromdi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gvtsndouu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gttbwovyh.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/guwioxdvr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gifbgoufg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gipyajeym.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtbsrywsd.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gmwqxxpht.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gadxjxvjd.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gqjmmxhgo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gdcgimrwv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gedghxcxi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/grymuffqc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gmpxqefgn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gnjgioczj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/guknzgidp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gindkchod.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gypessahv.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gofvbnztr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gtzlcwpip.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gtxywxsxa.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gzhsbztxe.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gnznfspnu.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gvhgqpbkm.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gvqicwzdq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gniparwxu.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/goqobqndq.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gdyntnkkq.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gzgkiufqd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/geydikneg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gbidjgcua.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/geyrjrqqs.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gshhxatsr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gpeanbwge.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gsgrmdatk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gqicirkge.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/guptawysu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gspqbtagj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gzkofwriy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gmqxilonu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gwaauutos.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gshtqpquh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gwadnnryj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/grhurvoqd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gfjtncuxx.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkcjssrjf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gfmznivib.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/glbjumhwr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gkenypyiq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqoitjx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gmbvujmmu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gehnlivha.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gxljsptrs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gavzydoyf.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gyyjivicm.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/giprennjc.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gmzsbuhbq.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gualndrhv.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gfmzewevz.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gaqmnfars.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gcgwhjjdx.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gqhuybtly.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gjkwfnfso.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/givapirho.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gxxjvketu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gbvhduuee.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gxtdjbgiz.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gtsgfnpph.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gajslolsz.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gvagtdhfe.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/guxmmdtux.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/ghijffnrv.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gnhieugug.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gqxgiaeds.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gdlrgwbuj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gutvwcqvy.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/ggthpklov.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/grymgezpv.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gooyqozik.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gzsffnmdm.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkcylzgaw.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gxcucdeew.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gtcdauzeo.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbgygiseh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gapdeamxp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/glpllobit.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gcgkhfbyr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gqtwawwls.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ggaglmhto.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/getdutohd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/grmketlis.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjtpcrwp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/galrawecu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/grmughfaq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/giwiyglbx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gsxxtslvt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gocqaftpm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gchstnalp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gefzgxeok.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gmkwqhfop.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gbsauhthp.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/ganpgyzrr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gfpsnnbyk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gdahmarhg.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gwkccbkqh.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gfeehulon.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gxdbdtcxs.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gsmzmshap.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/ggoizkayc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/glfixvwui.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gpnswyuqr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gbmlbohxt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gfgraxxis.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gyololmxr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcignkvka.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gyfmcscls.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gsikxwqea.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gbowtscbw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gdxudlfkl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqlawge.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gfiytghuc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/greagkooo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gbkyyjgou.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gmwunxtul.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gxbkfgcxj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gaicgrwdk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gpohmplka.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpjlbtsgl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/goqpojmzd.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gdmografm.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gjdkwapma.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxvskvbtp.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpzviztmg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gmzxbtjsj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glciyjqmf.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gyvwwbjvw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gjicnopww.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gwrddtxup.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gbrqwmghs.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gucpsndwq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gwppxqqjk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gedmriirh.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gkkfgoboq.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gtmpmoaii.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gfgkhcfcp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gctjnvdaj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gfwmzbgca.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gcexaxbcr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlvjdmbd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gipaufxpi.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/glwpqjsuw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/geteyeoqy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/glddyttkz.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gpbtyccii.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/geecvprxi.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gjccbwnrq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gjougmfnp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxzylxbr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gydjpudkg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gppudafgq.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gwuuhmici.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gkzktbcsc.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/guiioazvn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gcwyyfnpe.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gpajcbymx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/ggazawphf.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gssvemrjs.sHtML


<!-- 参考信息 -->