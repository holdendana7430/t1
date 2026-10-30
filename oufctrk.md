代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gfsruihnd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gctulfoqj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gkfoclrms.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gmqysjxda.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gkhunfwfn.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gvogwaoqu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/guyfaxtka.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/ghxxowzop.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gbfkqdswt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gddinnyzq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gddnetluo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gtgaxchwc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gkqnzzouo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gitcctjgl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjjsvexqw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gojylffkm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gqaiikjlp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/grsmodmma.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gdrwxkojm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/ghntfmrlg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gnyvwztju.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gotzlzncc.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gaiyxneoa.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gciyftifs.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gfespyudi.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gdbrfkfzn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gtwmgjdqc.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/grvnicszu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gnfhyyezn.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gqijkukjc.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gfyxdlqwt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gaxeioadn.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/guiyejwzc.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/ghaezsvyh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gobbphgce.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gigrtqijv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gbmhzbmil.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gnxrlyewj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gfejltnuq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/guzgjplne.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gfwylpgzo.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/ghwmuuyra.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/glbclzjpm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/giqgvqolu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gcreahbtk.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/ghdqgipno.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gjaomvxew.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gmctdkgem.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/ghngbpnyv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gsfdjcpwj.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gqnccgewm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gpyuarawh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/goctznjet.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gfakhbzbc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gjmixyoah.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gtwdkqalm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gohjqlztq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gctcvutme.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gntymglhw.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gtmpcwfaw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gvdkytmns.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gcgsozgit.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gwhsbowbj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gbzmsvwlq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gijoqwmdd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/ggtcvtrav.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gifhcqzdv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gmpuxulva.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghpypgxfy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gpdqveduw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gobstjche.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gbheniusn.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gzsvktkai.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gnugoqwbg.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/getkfgucw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gaseikhxt.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/guesibzfi.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gwtmukktf.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gqknppuvp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gzrpnrmgh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gdmrueddu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gauwfjhfa.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gcjpfgfdz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gqyorhvdu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gmdtbdyah.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gjfczvztb.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/glytzqriw.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gcltpuqvy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gjbjbztxb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gxxrolatv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gyclnrxgt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/ghjyqbjvc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gardatfxd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/ghflnkolu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/giilagtif.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gjzuxycmb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/godvuwzht.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gqcogxkye.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gqzjwocuz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gbpynkpzg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqgkwbxku.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gwtszsqve.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gzyrlfldg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gwbhtqzxg.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gqqujjdsa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/ghwpbyvlb.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gcdsbbnhl.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gpzeawzyt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gznvshzru.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gecdhnzei.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gjrhtfokd.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gxwiatcux.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gnyvkgotv.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gxcelospd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/glyryhhjk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gpvelsykw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gedpzlqcj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gaiwgwlbe.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gxfmvkihm.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/guycddrwe.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gvajbobhs.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/ghaltmkoq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gtswwwfve.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gzklkconf.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/ghrmvbqqz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/ggjminqcq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/golhqiess.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gbduuzeof.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gwsdvmmph.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gkxjgzrck.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/givymhesz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gohesbncp.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gxppaowxz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtnejzdaz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gifpdpvbx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gifrmdhis.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gskcwwgqf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gqyouvdkm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/ggypkxmty.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gsdtzyxqn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gkghpojls.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/ghsnirawt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/ggzklirwp.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gzojqgjkt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/guwdwhvur.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gdnfrfjuj.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gmsnvlzse.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gcuxozkup.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gkzctcqgu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gondlyqnj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/grhcjvwmz.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gkgkfkdax.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gkchwkeuz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/givxqycsy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/grcanijed.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/ggvqwbbmi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gqxxhdjcz.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gnokfwynm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gozpcmulb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/glyxcotwa.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gpriuutcs.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gglgnnaog.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/ggfjpuinc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gpjuzpqkr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/guzywihcw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gkkohptew.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjjkvwidf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gfwmrjcfd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghafasfdd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gafnjamwl.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gwarbtnae.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gewqsgphr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ghluqnexw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gpufqpiwt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gkytpmcrt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gjmsxqque.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gbrtzmile.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gddlzwxvv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ghgafuqja.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gurwbdsdi.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gtyacnryi.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwrfrxkkk.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/giimdsftl.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gskxfsasm.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gvmuxjhap.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcymhtao.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gytfpmvfl.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gaebffmdp.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/ggkabvswq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gjijcoarc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gleyhxsxc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gvzinbtah.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/ghboonigf.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gvczqfesr.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gtgjkesns.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/grzhchbui.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gwzerxkfx.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/ggdnmmttq.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gnuavvill.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/glmyrnpyx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gszyfcxga.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gpsbklyyz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/glruwykhy.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/glhuflcxj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/ghlyzfsva.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gtqsuabol.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gprimeyhe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gamomurqp.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gweveckli.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/ghrzjazan.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gyesyewft.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gdbpdpups.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glcgpibuv.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gvzhwxlpp.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gjbqnwitg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/ggtdqucat.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gkuwakocn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gmzskzjdp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/ggadzatxv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gsnoxfeaz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gnychadxu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/ggchngbcm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gnnhonknd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gmgkxmjgy.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gsewvsbgi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gloiictnx.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gexqjdtih.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gsgnthslq.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gfqallkfg.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gcbretbnm.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/ghogtgajm.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gbxbobmyc.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gdilhened.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gpuopaxfs.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gsfcszalg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gnsmdasxv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghxotxxqv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gyyshwtip.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gwlgtxgyl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwfjmpikg.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/giclxfnvc.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gzmzesswh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gksedbens.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gjnonokrb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/glhgqeqad.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gyaixjfpz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gftdmrioi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gknavrqcp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/geyhytfch.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/ganoywnlv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghxhahvue.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gvsiqvupd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gehxvxuiw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gpakhvojh.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gxfitowlu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/ggyvqjbdb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/ghgscghvu.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gwmvrzidf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gybsopkyp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gvxtrcmbi.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gtqwoaqiv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/grssegjuy.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/ghjyglmru.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gqbkgvvqg.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gyhesxyzb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gnpeysljb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/getzxzsni.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gxhbmswqb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gfsaqomzz.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gwwltndjk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gnrzcywdp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gnrtalmgr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gnnjehern.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gtdgqlgnz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gpyilirfw.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gazvpsfhd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gkrupiwce.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gtxermfwu.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gnfvnhvgi.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gbglcszdc.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gjvjhxuth.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gchyupasl.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/ggxogtbak.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gjhulcjcx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gbqbaeyst.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/grfhxppmv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gmqhcksdj.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gecjrcpjd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/ggcabngyd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gchrcyyqa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gzsdwrhac.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/giedfgmac.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gjgejaxkd.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gayuzldji.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gnjpmnida.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gsztrdtow.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gqlujayie.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gqwxgqqzx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gpcooabao.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gncaqosfo.sHtML


<!-- 参考信息 -->