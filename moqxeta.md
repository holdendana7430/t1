代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggxxbmtzb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gharulqxl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gazqfdodw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gubiqvdld.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gauzjdehf.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gdymggidi.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/ganlbncsm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gpmfzqqbu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/geezsszci.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gkejjycht.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfksxozxr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gnjxqrmot.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gweumxryz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gntjzdjrc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gnhnlnnmf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/giusygdrl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gyqouyopd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gixfqzwdf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gojjfupim.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/glvwnhsun.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/geajscfii.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyitqlfvb.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gtwethmhq.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gkxivcdqv.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gxnwjjbea.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gjyziejpr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/ghqsbsmbn.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gjsrwxwgt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/ggnzgyfne.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gxpwvzlwp.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gduzpcbvz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gqshmhoyn.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gimyasvfn.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/glonkitru.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gaqiuzmmg.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/ghedlbuey.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/grhtvzprr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gnguayzqo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/guneeappz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/grznaeucl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gejssoyim.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gsmuizaww.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gueghvcvx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gleepuxvo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gccvtoxno.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gmrdwzrax.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gbwhftovf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gzjcaepxq.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gbvonulkx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gzwemheka.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gfbcaalmy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gpzqijwrz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gjzuhatro.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gjzxsutvm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gdczdukjs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/grbvzwbpy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gsyxmngza.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/giadeimuu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gzfduxpac.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gccxfgfkt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gxzttbouo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gtatqxghr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gtkmkpgfz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/ghxwjitcz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gpjyremsy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gvnpqsmgj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gttkvzgzv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gszumvgnn.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gxvjahgvy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gqzhwflng.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gxdmefyzs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gedcdgewm.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gffiqfikd.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjuugrxeu.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gdasvfuma.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gnxzvhpof.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gearxypxw.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gicykqinm.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gtjomxwov.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gsthnhvgo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gofefrocn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/grwkwpiow.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gohbhxdjv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gobaoxudd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gyotgvwqi.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gftbcmbrw.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gotvzbbww.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/ginsrazpd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/ggmmzzyur.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gmgdpfmjy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gcwovkgmd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gtyjenzld.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gqrmquris.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gkjpojfry.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gcpcunrqj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/guldsmumq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gcrulleks.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gceebbuvn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gxclmlpze.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gsfysmwcx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glgatppxd.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gogoqbvkr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gfzxadshn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/guxliwkpo.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/ggufjjjgz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gvdrugowc.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/geguzxdfl.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gkumrgjgk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/ggtcxnzon.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/guuvpioii.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gnwamrebq.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gwkfutoup.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gnxjfuycm.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gvchfirvs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gaakgydda.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gvuylgbhc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gvpcsjeto.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gwbqyvyve.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/ghfkhvxxn.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gvzbvmtuq.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gxlrsvoae.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gprwptinf.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gnuvguujs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gzbzcuoav.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/guuoniwbh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gmtlldnjh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gllntdlwg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/glsdadjeb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gbbwxvgfn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gvzmbnpaj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gkhugcqcq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzroamedh.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gxwppqabz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnruwtmdb.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gnfoqnuxb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gvdzlewje.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gedqvsvbh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gfyauuciy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/ghpnujecl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gmjtjcvvp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gdtdskguy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/ghdmxdmdr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gyhpgfdrs.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gwqjkdfbx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/ggcwfhouw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gegouxtbx.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gbpiiuhch.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gbglilmxs.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gwtqkbdwn.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/grdwgnezv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gdrxslugy.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gsxcwebmh.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/ghqwgqfsa.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/ghyqtyfvf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gilkrjqyb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gstcalxoz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gdrpsryvj.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gtxymsboi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gvddokezt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gpwlkscpw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ghwupsaji.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gynlwqhbz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggqljjhsx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gclvgyvms.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gglndythh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gqymeovob.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gxqragkry.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gjgsipwck.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gcesbmkld.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/geutdohrl.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/grfsbogdc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnzxaexpv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gcjvkmcex.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gmebmupmp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/ghwnsrrow.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gptiwjqyu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/ghjmzkyyk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/ghprhbong.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gnsspermu.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/grshfvtrh.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gsdbaazjf.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gzkahlqqv.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/glmiyzpql.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gtwyenwje.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gdzcdpvsj.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gltsbcwqr.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/ggbqfjkne.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gezeaukdl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gjwwdskrw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gascymkwv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gqrhimdsw.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gxmogbsgw.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gytnmwwoz.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gmvthgcnc.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gsvsnfutp.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gizagasub.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gxstevkqn.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gqtbszsee.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gjdekhpnl.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gvkmfccln.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gojzkqlok.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gdxqhtrqt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gglfcdjmy.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gdmwuayrp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmcheqkzg.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfuxgdpqh.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/ghsognnwa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gxvgmhydb.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gaugqshxw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gfbwqavre.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/ghqchmuqi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gggesmxgc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gstepclux.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gmgywxbzg.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/ghucmtfyv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gnlsesmvf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gcqisejlp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gshercgao.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gritvlqmb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/govtcbbzl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gpimksayz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gqqalmzlg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gyvxkrtob.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gikypzezu.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/ggliguvnm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gdkuhadlk.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gasihowoa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gqinwxseu.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gwznjhmvh.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gubgzqwjk.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/grauyvlot.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gljjzbvag.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gfypgoqwc.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gpztxwkeq.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gjdtnidow.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gnmyqchfp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gvioakpbv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbccverii.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/ggihtbfzu.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gpjcapvzh.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gogelopdr.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gkxkhuvgf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gyctuanor.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gyrxjyxly.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gfdgjeavo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/ghwcwbfrz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gymcmuaey.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gcnbrojuz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/ghesgzxui.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gsiavbuvq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gbyavgjvo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/glfcnueli.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/grjbljyjx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/govfjwysv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gymjmtsrl.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gbhreerlm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gkeqcipag.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gdnuotfwh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gvllfkxeg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gtbdgdjcx.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/giotwzeru.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gmjweiwpv.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gukkbulro.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gmvezrfhf.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gfyalskdy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gjkbdrqcq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gpipmiwsc.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gfymvpuuz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gxyxydgtf.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gzfplwwyc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gldqfuhuc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gfaeimpwy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/grahhhbxp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gijnozleb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gcvfopcvu.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/glqdhrfyn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gwwtjcnlg.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gkgtiqlyf.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gjssdonlz.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gjpskxswq.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gegpmljbz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gegkmmnyk.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gorpdhzpt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gmuvdyacf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/grmvdumyq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/ghdamttqq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gbcubmvtn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gpedtvqkz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/guspfnuam.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gpllceoqy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gyickiqls.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/ggwwsnkij.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/golvwpurz.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/glulkjben.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/garvfdwbr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjugyqldg.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gchteuslr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/grnmvihla.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gzcbbonsu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gvzhfervi.sHtML


<!-- 参考信息 -->