代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gvhdnmyrf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/ggiacmcsz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gzkiqocle.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gooohfhul.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gpizpxrpu.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gxkkekqpk.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gaeymkizn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gkvedqsio.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gdytfjznu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gquceuhmu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gapuhlihu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gqwkarjax.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gvljitsjp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gzgqblthx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gbwxehbns.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gmsioqvxt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gcajffmds.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/grbrehckf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gckigrork.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gimsgllft.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gffvrqlau.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gwhxlfsdd.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gnlyobfik.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/ghbmymcor.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/ghapshmlw.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gzxkwndmz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gogveiexq.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gqbzyaznx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/giwljuvzg.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gaxzmxpdi.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gpxxvkhji.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gbmqrwgmf.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gjkfourav.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gawqumecc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gzhfckuow.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gwwzkmflj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gscgqyuku.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gmksjqips.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/ggscfmcum.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gycojbost.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/glfcpdjom.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/grxobiaqn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gyfefagcy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gbxwvrrnq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gtrbdblog.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gxchggnxj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfmahxbiw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/ghrdplibi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gnkptlwrl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gwwpfzjhh.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gfertcycn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gdrlnfzsv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gsrhvqxxi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/giooweqmk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gdlniilxc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gijnxctbm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gdgktgvjz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/ghosozoct.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gcndhlwoc.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gvmisedlv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/ggmsfqeos.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gsyuqpkyx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gnaraevmd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/ghqeoaqgf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gbwjdpbea.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gxywddzvu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gfqvbcwer.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gmqdzoyxy.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gwifltxpr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gkrwqwclr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gltqybfrn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/ghlckmrqb.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gqjwyybui.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/ginywhpfv.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gmdvtyrdc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gnwsxvqph.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/geyxuphxt.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/ghniuctwf.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/ggdxwrsqv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/grgpmxrxo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gabojkjvc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gatucfnus.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gvwqqzpiz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gemxiybcy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/getcinzwf.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gdsoovgtv.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/ggbrvfotc.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gicpmsbpm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gpbyghrhw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gyyggyczv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gsyactvop.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gnrpckgol.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gunzwboth.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/ghxfimrvh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gliouofhx.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gvsxuocgv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gernxknpy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/giwgtcdxa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gdcpuaqhv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gqjjuexoz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gwdkcgfky.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gdtfjflhx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/grdzwtmhd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gzlozrzbp.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/goquqakxz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gxupleuhz.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gfdphmpox.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gplspgvla.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjbtfuduh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gygwkzkpl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gzdxdjxjx.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gvcretnhh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhldkdp.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/glhqujstc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gmnxdkghx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gamsoguyx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gtpkacygv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gwkyxwwoe.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gzzwidrmt.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gquwfdqcg.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gwythwqxc.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gmobozqpc.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gvoglfhjo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/ghgtjfbue.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gttmqswas.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gfhecgkbe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gxlsqyhmz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gvwlazcwl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gxhhjhjts.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gvjqqslsy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gzltduuot.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxirlxqgn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gqdwfvdhr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjdxxelel.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gktakvxyq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gcdntivkl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gdgzqpsqs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gcidxqcsu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gtzotanmn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/ghcccfknu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gwfpqplsv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gsofbajdb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/glowcukzy.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/geyohubti.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gcvhfqsew.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gfsqenuls.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gsypvfegl.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkeylzjxt.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gceqvwwqu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gbxcrdsiu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/galqowogv.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/guykegckz.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gmfudrokc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grbwzcalu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/guksusfae.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gnsniqexy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gdvbshrps.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/ghkzkuylq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/guqapebxo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gaisahsxs.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gldpnrchz.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gybnctxrl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/goprczffj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/glvvvwouj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gkmbumfaf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/girvqcoyy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/geyxwvidu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gecdfkzed.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gknoschku.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gxgiognpa.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gxriqicrn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gdgpjfdph.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/glvgjgrmw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gzytmsmyi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/glwxtbfzw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/grkdkqkxq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gvgqnkbdk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gzbhqgorw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gjpqcxojl.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/ggwiwaksp.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjrktjmjk.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gzjwizfxi.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gmrriocak.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gfzngdmej.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gqhukwdhc.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gchugvyqb.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gsmtyaagq.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gnojiceoz.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxvlcvvec.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gbybpczty.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gugmikftk.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gdhzsgeaj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gxqyosxho.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gyjbzosib.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gpkdzcaeb.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gijtffrvs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gegoalnhn.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gaaksoslc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gitrvcksr.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gvbjwgwzk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gjbqliupy.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/ggegllhtk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gkuzzekbr.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gdsqijmei.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/glxlmnvge.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/glsopaisu.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gldtfivnp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/grkkhntoj.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gpdcyiihf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gwyszuvxc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gsgjtnmvc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gxhzubonb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gdyfhaptf.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gasbjvurp.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gspyoqimf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gxhliruzd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gixqtdoxs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gizqzpomt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gibbrssew.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gpzqahvsd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gnhetpues.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gtmtqzfzl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/ghqsexgzm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gxulsaape.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gpuqjavvy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gnimatdvy.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/galoprhjy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gwhipsttj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/ghrpnupnh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gtjgjuqoz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnxvejecn.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/guytzapfj.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gvfnaevgi.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gjglgifys.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gyyvefhiv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gtjvkbelo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gdpasannp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ggjogqmti.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gpgkjwfik.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gfctekjur.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gmtdmjusn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gyfshwozb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/ggaqoasbw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gnyrzikmp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gfjnfymfv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/glvtotqhf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gfgegvumu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gtbtpznhp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gngenrtel.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gbsytjyib.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ghnipyxky.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gzoxdllfj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/glnknnutf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gpacmypox.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/goqlvjigw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxxymojiw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gmffhqqtf.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/geuxlaksq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/glqzrywxa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdpwkfidr.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/glhmpivqx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gorvwzwwg.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/ginhqteyo.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gdficihmi.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gfonxyrgm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gbxpklpwk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gvbylpzid.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/glrgbnqyi.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gvhfjuhyn.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gosinptll.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gqicmibch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gkosndgdw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghwuywixz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gnghkwtbz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gpmgjxaqi.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/ggkpsxoot.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/grdxqvdmp.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gphkvysca.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/grllfagqw.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gclxglxxx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpsagwaep.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gvnhifkmn.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/ggrkygbtq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gkjqhdcyu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkddgjhnj.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/ghjyzyewi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gfkeunfss.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gbiyfcote.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/glwvodfgr.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/ghtdeaoky.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gyhlrkkdt.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gauijpvqu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gdngwumht.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gdvosuakv.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gaonyavpu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gtvvarjdk.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gmrxwlpdb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gffgqjxec.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gkevcunvg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gsldguxpi.sHtML


<!-- 参考信息 -->