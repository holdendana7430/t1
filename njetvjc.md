代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtptsfpbl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbxcqocn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gozflmehu.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fanxiaobao.xyz/Article/details/gevulpmjg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fanxiaobao.xyz/Article/details/gbxykinct.sHtML

[C03] 可变参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gubnxrkor.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpozbtuwu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkilldra.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrgewqfx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczxkecpy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwssbilj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnffspszc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fanxiaobao.xyz/Article/details/gytqblnhc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzhobrvi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmofkgsqg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaygewdgt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gganjbvdv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrzgvzkh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxngdwva.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fanxiaobao.xyz/Article/details/grufynphz.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gecsklsqe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqrurekji.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/garugadim.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/ggbaukhsh.sHtML

Py:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxmljoka.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvwdudrb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkctaqhp.sHtML

TS:   return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gjlwupghf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdrpujba.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gwrtdkjbc.sHtML

Ruby: return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwvzsbzm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gqogayxin.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmuuunll.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxjxahbr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gtopzhqhg.sHtML

JS:   const square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gcyzaqdes.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gfkidbdxj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybillezr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gehmzptuv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/grjenqnwu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/grteweflv.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gucnhkfua.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwprjeii.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjislvth.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/gjquomxhr.sHtML

TS:   arr.map(String)
来源：http://mobile.fanxiaobao.xyz/Article/details/givzxchwz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvacnccw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoplhxha.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvufmsotc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gqygteskr.sHtML

[C08] 闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gmjgfuvho.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/gwdvmvycu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmexssyv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkcilhsb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gblqqermq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fanxiaobao.xyz/Article/details/gskdevofd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwyexwfk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfdotjrz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcdkxssvw.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/geeyqisyk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlwmmlyl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwllyoovi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gjmzzwlcv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gpsujxwaz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/giuqpyzuj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjshpsro.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjqrmwyvn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gltzehbqp.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gyxdifrus.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fanxiaobao.xyz/Article/details/gfqotrsde.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/guswdkjne.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/glohylmlj.sHtML

TS:   同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/ghfzezegu.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzdsvblj.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqdnoert.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fanxiaobao.xyz/Article/details/gebirwjeg.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gqtacrbfz.sHtML

[C11] 模块导入与导出
来源：http://wap.fanxiaobao.xyz/Article/details/giiiucoae.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gedevyqam.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzaobrzh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpwdcyuj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fanxiaobao.xyz/Article/details/gvpozrkes.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gahopxhjc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fanxiaobao.xyz/Article/details/goetklsvt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpklgwmue.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwivwxzg.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/ggxfqwqtg.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fanxiaobao.xyz/Article/details/gackiidbi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkponcdss.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gmiqfksmb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhlvvsdc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fanxiaobao.xyz/Article/details/gmuvfblnt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fanxiaobao.xyz/Article/details/gcudhqcbk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbzjbxwt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdxccdaa.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fanxiaobao.xyz/Article/details/gffojhrve.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsrntfeq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjshmiaah.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gpkldlhjc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtaflzrm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmvuzkgsk.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcktbvbu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/gwwsedpmd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fanxiaobao.xyz/Article/details/gawmjpizp.sHtML

[C14] 泛型函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghspdgtml.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gicxglysc.sHtML

PHP:  // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gjyyyrexs.sHtML

JS:   // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjzytogo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqodqtyur.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxclcitgg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbtzcjsz.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyijtnjxs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwgjudej.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/givrhopyr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqvfowkn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gjgukanje.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/giuqvrykm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyarskbdt.sHtML

Java: // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvcmxtir.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gtnxnapoq.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumllaade.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fanxiaobao.xyz/Article/details/gllopfrho.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gyauyqsoz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmqguxwj.sHtML

PHP:  // 无重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcybgbkmi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fanxiaobao.xyz/Article/details/giclzofuk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzolftwi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnlxwlxtm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcqvoxkv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnvbzuzp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/goqajjtan.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggqahlejr.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/gesotiegy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gydhcwics.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/ghxvcxajz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fanxiaobao.xyz/Article/details/gcpnvohqr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmoeaatn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/goiztuqxm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gultiyzob.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrzgwxjb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fanxiaobao.xyz/Article/details/gomcfaool.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjonimgm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/ganooraxm.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/gfgdvpsfn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyjgwlyr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fanxiaobao.xyz/Article/details/goiiohorn.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyfyiwjj.sHtML

TS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gitbhejhf.sHtML

Java: list.add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozzisftn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gprxdegda.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrngralf.sHtML

C#:   list.Add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gnpxgzpgn.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fanxiaobao.xyz/Article/details/gjrtwdpaj.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gxpgpereb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyyzijtf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvmwpdoo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqslvzur.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/geiafokot.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gshrhjpbm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gblaprhsi.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gxnygvrsz.sHtML

[D04] 删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gmogpylct.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gojuchkda.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaucvvgwy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghipjckau.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqijbqcq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoeyujzv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnjxkryo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzziihmzg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwmihzny.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmgvfskzr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gjbevmamw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gkfpbndhz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/ggfymjjld.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giubkyhqq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhusswsn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gawqgefeh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gnailxtyr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnadbuwu.sHtML

[D06] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqudbviz.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gywmtzhso.sHtML

PHP:  count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/glfyktler.sHtML

JS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/gckbufieh.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxamyvcg.sHtML

Java: list.size();
来源：http://3g.fanxiaobao.xyz/Article/details/gxmvvsjgt.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghdqnflmr.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gcopkvwfq.sHtML

C#:   list.Count;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqwvvaot.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzkkmpgh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzgmklxu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnlujlyy.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gguoqkvrv.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqjrqpeq.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwjqbzxbh.sHtML

Go:   arr[1:4]
来源：http://read.share.fanxiaobao.xyz/Article/details/gppxbnfgx.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gqwnsnsst.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqjlwtgh.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxhaovco.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpjwyeua.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxipdlrhk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gwspohldv.sHtML

TS:   [...a, ...b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gerrbmdqj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gmoyaemef.sHtML

Go:   append(a, b...)
来源：http://blog.fanxiaobao.xyz/Article/details/gruqetzyn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gadjapded.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtxrcajp.sHtML

[D09] 排序（升序）
来源：http://blog.fanxiaobao.xyz/Article/details/gmdtwhgtu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fanxiaobao.xyz/Article/details/grwyourdi.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmqmlpeu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/gyqmbehyi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmjccbub.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgdxtsvz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gleccifpw.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrefbwhu.sHtML

C#:   list.Sort();
来源：http://read.share.fanxiaobao.xyz/Article/details/gllaahjyj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvteeefb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwsngllh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgncgrju.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpusdfcp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gbsyroztz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fanxiaobao.xyz/Article/details/gmazctdjr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fanxiaobao.xyz/Article/details/gygnmtvqe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fanxiaobao.xyz/Article/details/gfsmqilrq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswlmskyq.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gsceceybu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfezgmpu.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbgxroqx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrntjvog.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gsjljqkcn.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboyivvra.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjpzemoc.sHtML

Ruby: arr.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoezkzmm.sHtML

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gfhvtfnls.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyukjxtcb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfejhgst.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gemspqgxu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjomcjwxd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gazbiiugr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/gbaxzredx.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gakckimhq.sHtML

Ruby: arr.index(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyujhjipu.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggimqvfdd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fanxiaobao.xyz/Article/details/gabhkafii.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/grpzhvjjq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gadnwmtlo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfshthru.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/grymtqubt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gihkzatps.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdrdzkwi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gftclmrky.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcodpckyt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrypntbj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdapaatnp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gvsbxyhct.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjacxbfqg.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gslgoxcys.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gqongtfvl.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gxovhenrw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfhepakb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkqyhnhf.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdjhidfh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gbqmrvqlw.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghainsbzj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/goopzfthu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/grhxvwsii.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakfbbfmu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyfjtkni.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjvrstrs.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvdespcj.sHtML

[D16] 求和与平均值
来源：http://mobile.fanxiaobao.xyz/Article/details/gehboixhk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/guqbodqns.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gvgppgvro.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gonupzpun.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcswynguy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzrkybls.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fanxiaobao.xyz/Article/details/goimvudmi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbevrlldr.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fanxiaobao.xyz/Article/details/gokhzbrku.sHtML

[D17] 最大值与最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gzggervvx.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gaeivbriq.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjkydqvu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/glnelplkc.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxpmhvrt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gayjqqvli.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwgtomngp.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fanxiaobao.xyz/Article/details/gorawolrs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsppzfivw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrqfngkz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/gdialemuy.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/ghfjqkkpg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkrccruq.sHtML

TS:   nested.flat();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjeiduco.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfublscm.sHtML

Go:   // 手写双层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gaerzchiu.sHtML

Ruby: nested.flatten
来源：http://m.share.fanxiaobao.xyz/Article/details/grmtihpoz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzibkzgof.sHtML

[D19] 按字段分组
来源：http://3g.fanxiaobao.xyz/Article/details/gkecjlyfs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gguwmgcjy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtqveqjz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/gsnytkpbl.sHtML


<!-- 参考信息 -->