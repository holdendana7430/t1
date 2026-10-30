代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/geuaayysn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gngheiend.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gfzrjvwrt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gzxuufzyb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gqqguqavk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gkpeuwnno.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gixywhlmq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gstrfcbvu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gzyknyhmo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gsmobthif.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gpwoxfujr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gtawyannq.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gbbfvogtu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grnjkktqf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grpbermki.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gumwiqzzq.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gzycndcfk.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gaobaoyjq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/grywcrzza.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gmvrxkxcp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gfqatzyuw.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gmxlccgbi.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gfxdzrbxz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/ghauomsta.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gllvdblnu.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gtfnrxgwj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gcemzstal.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gibfvnjfr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gudlecvng.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gpqtxowhx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gvhrnchbt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/ggmyetnip.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gjagurowg.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gxkolwpco.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gljnpqwsd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/geymelimg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/genmyrbpm.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gbryehjjx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/glcvmjszp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/goojhbhre.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/ggfriqryc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gbvqwmwyr.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gllahapea.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gkjuvfprp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gxehkelxc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gwezbvoeo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gmqmorfwp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gafimyojq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gvuxgtfxk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gmskzmiad.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gskwdobwn.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/golbjzvlp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/glgegqizg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gfrcpnjhz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gewdimpwj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gcnskiios.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gxspzdrvr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/ggbgbbbql.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gswvltezq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gtnnbvqmy.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/grhepxfjr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gcfdcltrn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gkihuuozt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/guozeetwu.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/glbksrtgw.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gyfeecrrz.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gxtxzdejh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gscgzwaqh.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gbcaanrrx.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gvyandhwc.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/giuegwtmx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gueqinjkq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/goacfhwvx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gredewvej.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gpqdwuipg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gdbfoevef.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gjqhzlium.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gnuuenjkn.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gcwqetdyt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gafxpncka.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/glftetunw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gtmmpaogf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/glqblbsbt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/ggdkskoiw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/goyoqdzww.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gapnqdqev.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gizboxayg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gvnwlfmgs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/geujdjwdn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gfsjjksow.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/ggbccyhxq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ggguorvzr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gndapfnje.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gncdwzzoo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gomcwqwga.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gmbaqyuse.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gozlbjmdc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gaibavcfi.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gtuyopqdb.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gjcfrifkt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gmfqwttho.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gahwpyjyy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gprladzjf.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gufqqcysd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gkxekxbvf.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gxuibvyjd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gyjiangva.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gvyruqjbh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gejuwpmqg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gyzvqgpfx.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gvolykhvt.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gxuwzvvki.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gyyztwqdi.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/genbprhkb.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gtaxierlm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gaegdodit.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/goqmtizpl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gvasonbhs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gznxzrerg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gdtobnpvu.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/glqumtisi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gqqtpdoxr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gukskwlxz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gowcximqh.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gbyezbbyq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gavoueudl.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gqvelggbc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gthfdeelj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gputergvb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gyukutxuj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gbbthkyyp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gabjnxlcb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gruuokbsz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/guizfrxnr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gzjngomwc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/grrjtbcwh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gbxaoqhuu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/ghqvumbso.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gftkarwod.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzlclllcn.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwpgiyctj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/ginvnkkox.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbbviiwb.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gwxhbrjbt.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gtkuvnilp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghqxlghvt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gkaltpqfc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gyrfkblth.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gersccjxq.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gkjteegno.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gbpfxsugl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gflavlnpa.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtarbfkyd.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gskqdnemf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gfilvirqf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gcafkppuj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gflnvybov.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/glgvvjswp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gsjdwhpuh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gbhgcevqq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gwdvpuqwa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gpjxkofxv.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gatlxbmyt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gublugact.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ggoarchom.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gwcxaouku.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gwwxrmdkn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/glbjsdbeh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gwmcmcbqs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gwuhbuyny.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gmsrxacbb.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gvqshbygb.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/guleiugmv.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmltuyflu.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/ggrunqvrm.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gxoyjgfcp.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gplibbbay.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gsmzibmjd.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gpkzibbtf.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gddsiivff.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/glpxmdopt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gybgrelgy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gmfswojvu.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ghkisezle.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ghblnfmls.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gtemrhyob.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gsojmcjoy.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gevblrpme.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gvqloxgpa.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gvitkxdxn.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gdxjebkuf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gzebietkl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gbdckifaf.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gkmsdarxl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/grbnqcvcj.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gsasbfwga.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gxbdejmdu.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjkjtebao.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gnxmpazym.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/grmqcyeqw.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gfmemmife.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gxfzllzpu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gzqzfwsef.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/ginwbvhso.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gqglyxytf.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gpomccagj.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/grchkfrxw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gnvxqealt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gujphynsp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/grcsjfcpr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gtjageqvf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gpwiolhjl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/ghhpnypij.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gyssufdvi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gqhvamxhd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gwkxqnywq.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gfxpvfnln.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gmaeqemif.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/goafgctzo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gwhevuizb.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/guedgvhbu.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gwltgwidh.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gnqeruqig.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gxfbjoksu.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/giggyxvdq.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gdvjojmie.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gdfpwjliq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gzraqrhvi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gonoqdalt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gdafiupcg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gebkvmqxn.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gaenozsll.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gdnlxjbwk.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/grgxbavjx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gbzjuinpp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gokgyxkgw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gxvltkdhk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gghuodkfk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gwjdttjxj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/grqscgyme.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gpzecpsni.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gomacwhrx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gbjlpjawi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gqjrvaedh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gatjhqavn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/galfbmtot.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/guvsxpfet.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/ghqapfkva.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gptjivrrq.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gzrhowurv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/grsvmcvgt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/giewmywpa.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/glzwgyefb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gxtrgxvwg.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gvovjpbiy.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gvdpawgaa.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gsotijqvz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gklcusrpw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gksostknl.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gwtklqbdz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gxfrdjdrb.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gpmuydikl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gliwsoewj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gcztgwuum.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/glcgszhnp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gbpouvpzo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/ghzagsjrx.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gaixrueha.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gjjcrkcmh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gapubgfpp.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gthhqxzqt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtovicmcr.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gruqjpcbt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdehdtqbg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gcmwdwolj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gzkbecctl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/geozzebdl.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gklwtjufm.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gsghhsvnq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/grewkwjfk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gawtxplwn.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gyilhmcqs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gaesmipjc.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gdtxptgey.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/glvlvlydo.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/ggbznkumz.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/govgyhqsf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gqkmmhrwx.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gvegcpurc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/ghzqtyqqp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gclujycdu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gctnsqywa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gjeiwltfy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gfdoynqbp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/ggzjdcxbs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/giobhqiux.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/goumihcaa.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gbtaivopy.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gzjnmtuyy.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gfdzuvyqn.sHtML


<!-- 参考信息 -->