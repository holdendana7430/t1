代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gaotulcid.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/ghmdkbjcg.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gizxxmiad.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/ggiesxnqj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gyxmvnjqr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gdeqariiw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gvwreumnp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gimyerypq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gncwnwhij.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gflxwodbl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gekhklntn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gjxifvmep.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gqwlbkvmu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gocljbkbf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gmatdftxo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gyipdusye.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gjihsqazj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gwqssogzk.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gvaeeymea.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gegesgmdh.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gxglicfma.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/ghlhuumzu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/goglmjhpn.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gkgotsapg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gvbyipmhu.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gzhrcmeup.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gjcrkfttx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/glcrxpwli.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gpswrufhk.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/ggfkubhfj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gwthgbpco.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gcwxfpdzp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/ggpbykjav.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/ggvtslcxw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gvtrfrsmu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gjpfopwkx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gpcfxqxqp.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/godfiwwww.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gblxbjcfc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gpmneqgrv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gtevwwybe.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gvldcnovq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gatpkczas.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/geyxpygxp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gndkgcjym.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gwzptmgyj.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gqteqpbdb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gudoamxrb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gdqcxfifu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gutgvmldq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gsdjdsfdj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gosfqvpod.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gaetqvdfu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gsvjfayhi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gegcjupwz.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gzzqztsdh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gmrlsfddb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gsxauiodp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gunuqcrjj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/giwjvjhno.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gjmwnpjpl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/geooxiwez.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gbgquimhx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/ggbrledlm.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gpdndhjwh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/ggwiqefdk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gnhuhzhdq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gldjxcopd.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gahohtvto.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gymizlfzz.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/ghcudxdbv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gdmpilacl.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggupqkccy.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gqbpposmo.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gcvhwlpyb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gfxmiwcnv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gjitphzrw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gdxxewgwt.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gmlmdmigz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gcvlibzem.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gfebyvpeu.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gtpjrozdu.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gbtxedssa.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gixngvgwm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gvcylzzvy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gihsiqhjn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gpnrhowtg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gcckicgbx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gysscikzw.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gxptxcoik.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gpeyeghez.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gxntmutzw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gnqxhsnwt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxwseiafs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gszfidele.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gygexnkol.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gglepckpr.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gsonzakah.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gpprlybuh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gjqhtjxmk.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/ggytdfttt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gidtdjdoi.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gxkwqyonq.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/guilvklbq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gzkdwqqdg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gqulqlnuc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/grhaevbee.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gsigygcur.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gkjpkynsb.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/ggqkkoptz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gxnmncuof.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/garapysxw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gzmebqltk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gqunpjouz.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gzrqhfoum.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gjtssdukf.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/govyyntwr.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gxvlqatgx.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gleecukwj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/guhvujgpu.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gvmncutok.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gtwqpwfjn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/godhkzink.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gdbibznkz.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gngrmtzbh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gynvgjlpz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdcljpeoc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gagvpnzlh.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gvuxgmcyt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzxiiqjav.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gdbwfdlzu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gixtcnuuh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gwusqrkbc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gmxoggucm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gvwoxfmxp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gopattdwr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/ggqjnvhyq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gwkabnpat.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gnfcrmlev.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/guwiwwguk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gfmhvywza.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gvaepwggs.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/ghvlajnox.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gjnffwgnw.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gmaxkfhgy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gqjzbgywv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gjprffdwx.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gzlohysxd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gdzebtjwm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gtlicdnlj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gwunzqqtz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/goilegvax.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvxrkuzgw.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gyahxdaiw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/grmkllmni.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gepgzlqok.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gapfpzskl.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gwwthwjyr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/guvmqxour.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gplipkblu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gduebmjjo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gfkaysrss.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gokgsezlm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gvkatatli.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gwgafzzdv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gdwwmaggv.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gvllowdmk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ggoypywer.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gjtvyxotf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/guhnkipff.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gqlefbpyb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/guizlewlg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gssfshmgt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gavcgvazy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gluklabdc.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gkfysqvtr.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gzdfkhaow.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkofmajik.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gvujjjgrw.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/ghjhnxrno.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gruxxnzqm.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gkugioqxy.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gudtbhnkt.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gljuvegdb.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gghbctnse.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gilufajys.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzsjlekww.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gwtqscomo.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtnelbvyj.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gzdjrvuzc.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/golcwyziz.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gdkcquvwz.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gdtlwzjew.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gwymgliak.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gygcsuioa.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/grxfwizvw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gevkvprmk.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gaidknsxw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmoayim.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/grhlffexj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gjpdosquw.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gveguerlt.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/glexhitpu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/goezdvkxa.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/glljdkgto.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gesggqnsn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gvywgecrb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/ggzzmxdbd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzxqhkaqf.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gufqybgut.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gxdexpupd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gumwpizvc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjeooyvri.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gpcjajozt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gdnwkhotz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gsqpiegmz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gabopxrqk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gropkvmhz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gksisxmhk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/ginamcptz.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/goobzviae.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gcmqmabgl.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/ggwhlpndg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gcyoelrvs.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gnfpriqpq.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gqsgoetev.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcxbfvbvr.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gpykwxjyb.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gvmvowwnq.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/ggserjyny.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gvzklykap.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/ggbhrrdwo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gnrdlpjfk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/guuhvwcui.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gafnsclep.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqgxnbkvq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvisrxjpt.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gospqczsf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gqbtzewfb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gwkmvqpyx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/ggschxyaj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gatmjgsoo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqnuehkzr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gjnaepaeh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/ggyizryfu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/ggmeqyzvc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxszvyuun.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gmfnwnfil.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gtdwbypms.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/glzhjfypn.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gjuwcxcuv.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gopldwiof.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/grpjarjco.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gdljqyyvt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkwhepmzj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/ggdlfvwxi.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gbafhtjsf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gemsgduvb.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gewffecpx.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gpytfkpbp.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gcosotfqu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gyvoewvpo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/ghfiklgls.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gifpwzzjv.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gprxiyvrw.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gxaybpcnr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/geamqpvjh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gldhwmljn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gomiexdhj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqqvpzizx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/guayerlip.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gaegobest.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gqpruhtyx.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gpoyvhnsu.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gaawxirht.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/goblrfdqq.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gxescorvx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gzpggttzr.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gnraquqmj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gcwrcsnaa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzkbzpoin.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gvgzpbsxj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gnmrjuhqx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gmastgstl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/givbobqgf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gkrjpagsh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/ghxssjuob.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/grhnsvkgh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gobedcufb.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gffkyplze.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gfrthcges.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvlkpnqgr.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/ghqhttuep.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gnwnermrt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gchrydafa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gpkltaclc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gqseyprxu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gekzimnxa.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gkerzkdax.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gdrggmlfg.sHtML


<!-- 参考信息 -->