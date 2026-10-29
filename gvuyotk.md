代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/ggqrefopj.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/ghnhjyncr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/geidmfmpb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gohaszndh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/ggvahtwfr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gpaeprxij.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/ghiskjnqa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gchbntgkt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gynmhixrw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gpxlvlhfw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gzlwheetj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gtjinnzdo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gctxcxdgp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gmtidfowb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gwlmijlnu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gbuxhumxy.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/glwxoboxd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqyfllvdt.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gqwyehhrv.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gxkhdtxyx.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gjfkiuvdg.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gtrxgmwyt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gicfzaerg.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gtsxxciyv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gueucnkgx.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gxjkhbhru.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gkonrprza.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/grdrfvdqd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gcdkitonk.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/ghesevtmc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gmmltlhms.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gtaimfcfh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gisissvvx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/glapgvbqf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gorwiejnb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gbclpgxbh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gmhjbobsz.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gdlpvdrpw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gidzkyvii.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwljjgqnp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gooqyovmd.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/ggqyweggg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gdsdcdfpf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/govhkhfvf.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gwvifbbwj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gxxofwcue.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gobrnlxgr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gzwyjnydn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gwbtzqesg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gxqugajdo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gluonhann.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gbtcrthsy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gzedkfkez.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gwbsgzkrg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/grdvaivvj.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gdfqagzgm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/ghhnkgphw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/guapjizha.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gitpsvcxs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gvloencta.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/ggfnfkgzc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gcrhckasu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gnysbhdau.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gbrtgflfw.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gcviguafk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/ggspbpikz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gcrfylzif.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gcvywswul.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gyymyzunf.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gtdfeypeo.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gpukwtcbf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gpekaacjc.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/ghgnpjzyq.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gmgdkqvok.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gxenffhrk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/grguxvktc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gyrctyczs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/ggyqhvqjm.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gjaoexoeo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gmreoqntu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gowmlodmv.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gmmhbkiuu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gjevrfxpr.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gclnownmg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gskqxvhbu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gtdtovjep.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gcsrlvizo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gbhwskeyy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gszfnyufb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwkmfjr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/grityeuhw.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gtwhqbhzc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gdmivqmys.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gweyalsgv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gvfomvjhy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/grshhgeoc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/grywocysf.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gaogjyfdu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/ghckmflop.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gwkqakwks.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gblwfxvfn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/ggjraktdm.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gusvgheid.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gthmjtfhy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gwboxjuve.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gwtnpfofx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gftskvshj.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gntplmtfk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gyqwuedmv.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gorqlqxmg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gxocnhekc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gmajhpxnf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsxhibzpl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdbuapmbh.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gkslgpgqv.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gmpshlave.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gcwyotlij.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gylszzkvu.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gkfzjckap.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gksbbnypr.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gkpidmals.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gocfkkrwb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/grlacfwzw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gwseqfmuc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gxrgekdco.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gmwevbuxx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gszjqxppv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaaoknhxv.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gwiwhoooa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcvzkoryh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gwwycxsad.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gpoqldilm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/ghmtwbrem.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/ggrpnpewr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/grbyhngbf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gsjdwokwf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/grwlbxile.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gfmcyruei.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gdxdpjada.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gciigfusp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gdbkvyaka.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gniukshdc.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/goetektga.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/giuthvebr.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gblsoxlnb.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gvrsdyykn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gjwjzatqx.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gjzrsjudr.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gowccslwi.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gnmkqtsnq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gqiqkbepv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gpbweqokp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gdcdvvfvv.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/grjxczxjq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gpincwzrd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gbcjhsqip.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gvafvjvxt.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gmchtdjoc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gdanftnmq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gibmzluge.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/glfkabysi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/grgrjdvlh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/glefxlbnm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gsrjqeihb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gynsaaxgu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gmyavgasp.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gtqtfnzyp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/guvxokakx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gzdfhwjii.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gthllqttz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gtnfwsnmw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/grhtgkgsb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gwnaxhvyc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gblrfvbxg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gljeymruk.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gjdxrbnbo.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/grunhyivs.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gpogtssfh.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gseajtbie.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gfabwovjc.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/ginkqewot.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpudogtgy.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/guxbdzehn.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gpzmxgsac.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gwruiessi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gzuaiapco.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gdjwxyxbq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gzidzmtjp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gmbegfujd.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gpymrwhss.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/geaaoihtm.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gxwvzghtu.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gwiojzdbe.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gejyjvhuy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gaphmrsxa.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gsnpswzzy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gxoacxect.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gssykljlr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/glkdcgwak.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/glmqhxywo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/ggcscgmzb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvsrsxncv.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gaojfqaah.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/glqovnnvo.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzabylwkv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gnyszgvmp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gjjzyufhn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gigvfqhbq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gqrylqcfj.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gjyyssmhs.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gzwtzhzvp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gaphpbsse.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gzdbecsyn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gtyzxsmvw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gudnwrkwa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gmzxozmnt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gsmmnkfko.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gwpfmueqc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gueykfthm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gzfwilpai.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gsfwizqia.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/ghznlwcfr.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/glgqdhyoa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gwejpukjq.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gnntlrnhv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwcrcctnp.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gymytztyg.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gymoyafdj.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gfemgcjev.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gsmfesusl.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gvsjhqgmu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gegkpcgha.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gddgvqkux.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/glrgbhydg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gdtapojoi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzhhgphe.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gygwclxek.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gjslciagw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gkmgnaaes.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gpwasawto.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gkxobjjuk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gsxzqpfrc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gjembklbh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gsguzugrx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gjqzgfphc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gksiagqfh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gyjsannvm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gnbndehub.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gmogyuxco.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gcbehmdbu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gpbelnift.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjlkmxcdq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gibfcetki.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gjebdtonf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gzcjutsnb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/geqmfajfi.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gzvhtrdok.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gfzhrdbys.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gjjpzaraa.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gqvvugbjf.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gyhhpoihi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gxzxwlmxf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gblgcmtit.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gzkfwpagi.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gnpmkrgvf.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gkqtdaesx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghozijufa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gugwoqcea.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gavcsbabh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/ghfcxqfig.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gbtqhltyk.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gflqxbbeg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/geljxkewq.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gaflrnzbk.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gksdoeoiy.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gmfxgqzva.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gybueemsg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gdvmfcujr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gguuxpmdc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gmcijizeu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gbksutusi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gkydrgfkz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gxajunnff.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gbenkhnfu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/genbxynfd.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gxpcfweyc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gqnmqsfja.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdrsmuz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gvieqzgwf.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gtezviivm.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gideultds.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqwuatfka.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/giqgyuuhv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gmvnoimop.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gnqfjqyhe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gsrmqclcy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gabfiebsn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gtgfohzrq.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gybmuzgqo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/ghvnugpxw.sHtML


<!-- 参考信息 -->