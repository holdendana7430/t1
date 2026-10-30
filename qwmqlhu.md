代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/ghhriyjou.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gtjmrvpoh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gynmhimug.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gfsbtsbsp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gwiuwspsb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gdvcupwtq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/ggzzalwgs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gvcmiotvd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/ghelqnsci.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gkevnwiwh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gvlwwempn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gxdazbtza.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gozusquzg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gheipcuni.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gigsbxqjs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gigsbyfdz.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gutucfbga.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/ggaehglln.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gnpidaszv.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gtconnjtv.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gtjhfkfux.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gpulsadyl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gscguhjqj.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gubzpydjp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/glclxurll.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gvjxzzuap.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gnzbhecik.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gkqbaixwr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/ghjhvoqaf.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gkpjmbclz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gxameocfb.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gbzugopyj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/ggqkuvcvt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/goaikxscn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gqlzgcvvf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gtlfwwvdi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gokyvevqs.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/geemqrbqp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gjcjzfnsw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/geafhzhcp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gruiajjua.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gpvhvqyht.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gbuxzappf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gfykgiahg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gmdopluxv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gzhadjxfy.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/grqwzgasq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gmntpoghj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gpfpvigri.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gudpyxtqr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gfqdzilwe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gmabwntsw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gvgszvjlv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gxesiutfq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gjrabxvrj.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gpicksjbj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gwystyqtw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gzynvarbn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gqqmmhmxc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gpewuadio.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gmxgbxiyq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gxxyuzbgs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxjexizq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gvmnhbnwp.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gfuojryzr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gfpcafnyc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gqduttplw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gfdkbjbiy.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/goykxobyt.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gjtahjmir.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gpbjtomtt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gqeqogsqn.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gyifmhpvw.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/glbguovmk.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gzmzoeccc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gmygunukx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gvqxhbzsq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/giyvvnybs.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/goejppftp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gvccgolky.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gsdmvcepw.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gmqduimra.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gqidtqqxp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gghxejfei.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gwiyykbic.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gkrdqpnio.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/ggocfhdrg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gzpxehoih.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gcnrovnfa.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/glalkmrjt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gwxxqyqoh.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gjrrliagh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gnjmygebg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ggawbcqnb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gcnifmofz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/guqoqsfcs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gpfvrylud.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/ghltiabmj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gxsexvfjt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gbhjcmbhi.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gfiqqtylx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/ggwqbxhps.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gldlnsbzk.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gtktjnbqg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gszoqqlua.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gnibrjzsb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/guzkaekgy.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gfvhufnwt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gjrynslfy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gyrseiqud.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gzrvysyhk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/guejynzlq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gszxdczac.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gwoxbongg.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gyifzggni.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gqcgkowjz.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gljtaknsa.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gmfiumabs.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gblidzywh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gctwqdoeb.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gpvdcbbhv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/glsvmbjzm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gqxwnwvrh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gqoamqfsn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gnkokymhs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gqxyjupvf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gabzhtwto.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxdvfkoih.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gbkoykyzt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guutddhmz.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gfmqrpxhv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gpyusxdxu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/goifvlslh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/giwwxrguz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gxjcjjawj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gckcdgrcj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gigljifyc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gnitfishx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gefzfjgrk.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gdrwbfodr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gibmqaxhm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gcpimmzey.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gfegwufdw.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gsblhivpe.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gtxqvpzup.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gebzuzhij.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gyweussiy.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gfrydfjlr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/guyoveifw.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gxpjrqeky.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gbyxltqtu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gbrgswivn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/greyusuny.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/grmbuwyms.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/giaxoiphw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gcvlsmxfw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gnzynkice.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gtdkesqen.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/garctoqlq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gsobvqhkq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gccuqllgl.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gewejibiu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gaxgokiew.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gbikpkyqr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjjzwxytd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gajolrtrn.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gqpackepo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gfcyctgxg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gddkjrkhq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gzyzrbpol.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gqljckbpd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gbaiabsyn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gbvocdpit.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gnyaklkpq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gltwkvwao.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gdxgiknus.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gdjihmhhw.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gkfnlcwrx.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gtftmllbf.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gpiuwbzpe.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/ggikwhsmq.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfspttlmn.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gwxxaelul.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gfwkamlrd.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gczoikqol.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gzofpgaqe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gmwrasltv.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/glfbrdfny.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gnhiqxxza.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gbcqlqkpn.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gunhbhyxv.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gfydqdbtt.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/geaxrkzou.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gudngpanr.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gaavznpkh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gmqkiaspf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gnsgxeuly.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gfaglugcr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gcxhskbtu.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gjpnlqnsr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gluzrdsdl.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/grrdecjiq.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gdwxijqgi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gtoldvlnw.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ggoyewgjq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gkufyqiva.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gftrvatsi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gtwcunvks.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghjyyxdge.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/goitiyzyk.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/glsgiityw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gxvrqivof.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gchpksjtu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gbxgotvzb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/glstcgpwh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gvscxilfv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gxajmykhq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gqgoobppk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gtulyjbzq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/ghmxmuhyv.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gagoidbor.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gfevvfzms.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gewjtpqwd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gsaqymsbq.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gdnyngemm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gsrybbtkl.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/ghuddrdcv.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gbjgdgkhj.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/goeuknpzu.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gyunyrero.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gbffdsaip.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gjcaqzset.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/givipgeei.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gnkjetspi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/genxwqqff.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/goxfgwllg.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/grgqobfil.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gasogkzye.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gncwfqnbz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gydoeabbl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gobfplgyh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gijezyuht.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gzhjdzbnj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gehljjntg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gcpyeqdyn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gjcvorikb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gqxgfzgql.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gpokkbzpb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gdyvxlwhd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gifoqmaad.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gnrmknxtp.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gisbmrshw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gltjssesj.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gtezgaxos.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gduqpmkgk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gpzegimse.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gogfseena.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gomwxdtxw.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/ghhqkaapk.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gqkhnnyoa.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gaugmcbgs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gwxarjyze.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gtijuyrpr.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/ghogsfpgj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gyvqnoohk.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gygpoipwm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gujwbhecq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gftmtyvrv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gccjxuhch.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gjrpyapnd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gvbnkppiq.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/girdmndlp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/ghufpxckg.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/geqvxldpb.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gzqimjuud.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gcmldmeij.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gralpclet.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gllyiqahf.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gtzorlczo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gwbpoxryu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdhejpfjf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/grugpkrna.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/ggbnsjkrn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gqneswnbo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gslxcppwi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gxsujtpyu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/ghpyvbvjt.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gqgrsdvke.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gqyrphktn.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/guwakxdwm.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gygrstqqv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/glnbpqmsq.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/glaayhicc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/ginfkrtnb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gajrrssgf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gkxqjvkto.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/guklxifpx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gnwljyzsu.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gdzhpjjja.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gnxmbrcrs.sHtML


<!-- 参考信息 -->