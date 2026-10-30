代发 wailian999

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gnwypsouh.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/grthgpodj.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gkfuqgolt.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gqqscxzgu.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gedwpnxyf.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gerbomyni.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gnjolwjgi.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gnzlfuuzl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gshsdrwmg.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/grneaoydi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsqebiwey.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/glirunfnb.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gzcryicqh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvwxeupro.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gqtukuhxr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gceaoczzh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gyjtnvwlb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gnatifmuf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/goxsleldz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gweyqngbr.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdrevwjlz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gsgasqnip.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gkzhjxmvl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gksfruxyr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gcyjqerox.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gwaoxqzvd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gkxebdlqz.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gxzggszlq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gizkexyjb.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gvdjilpef.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gysohnlux.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/ginqzbzap.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/ghcejrnup.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gbbazibqd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gfhevdhcb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gmslliroh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gqqvnisbb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/ghgrartww.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/grbspmyam.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gsqpspalg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/golejhwrs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gswjvvnja.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gekkjpapk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gyzodotzl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gtelefngl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/glkoybjda.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gdmpjbfvr.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gvnvteuir.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gmhxaxuuw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gjtgssngr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/getqzreby.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gsbwcjoir.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gctheqxlf.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gynlismak.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/guaeperru.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gwuanszfd.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gbrvsjwem.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gfwgxmsem.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gvbhwchit.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gzocqxtjj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gpvtrzezy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gpdfokstu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gwyugchie.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gwqgvelvc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/giolvbufz.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gcednxhbz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gfeqjyyix.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gidlyqvej.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gwvqlswfb.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gtahipyad.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/ggmukhbyi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gmnwnezfz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gflqcwzhr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gqrlgprcb.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gqukrcvlv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gnwmetclv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gnjogdtle.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/ghsydasdb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gbgtvvauy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gmuvkjvhq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gznckqdzx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gpswzpeha.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gufjakwhi.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/grearnrza.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/grzdxpsum.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gomdfhyqj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gpkgiivvj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gryakwpfw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gqetmfnzd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gvcnnozvw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkquufrlg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gzhtlonzm.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gkwvjszno.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/ggyrjnult.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gswbrfyxh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gurznrfcr.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghdlprmyt.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gnubwphxn.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gzkiryvxf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gdpwfrefj.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gdnurlenh.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gqxyrienw.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gnvtdxdzh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/guitxoyii.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gouojzzsr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gmyprjuio.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/grwwtsigf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gjjhmzpzn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gyfyxxusu.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gtnsswfut.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/giardmbyx.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gqowyvnda.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gquumbtfm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/geotwhrks.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gxzafuciy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/grvzrrgad.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/grhgewrwn.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gmckzqguk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gshreoswo.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gkgzlqdre.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gxebfdzxs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gvxpotbjt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gaeqxrrno.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gpsclignc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/glhmvcqzv.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gvpprxbzi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/goorftxnt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gfktfjipc.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gwthzogfs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/grhigfhfo.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gmrlbgals.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gdkodrtbz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gzhshtfkc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gstbgbtgq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gplkgvjnb.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gahqutblr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/geqpropix.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gixokqndv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gvgdrianq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gaualnjgb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gkycwtqxm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gbhrlrdjf.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gfqjwcilq.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gjbjhmttl.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gdabigyxe.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gdqgimaee.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gtmyshazc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gsiwetdus.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gzjbneggn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gjqchaheh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/growlxwsc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gcupntpts.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gaeydjeey.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gwvbfecjk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gnchvjeli.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gefhqxnas.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gsqrwhovt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gktpjoxhw.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gbjfzfqlc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gkkejhcdv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gkxjnjgsz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/geybfbljp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gvypwjxqd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/guxgzfyhn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/giwgfpmim.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gzeansxds.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/guwcxgczq.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gblxkeszo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gvnhjvtji.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gtlsnmbat.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gpzthumav.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gyxsdwbcx.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/ghccifpey.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gdcefpiis.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gddgzyvbz.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gixugerht.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gfzwvtpxz.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gperytjqr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gzgqrfcmo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/ghvkxikut.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwliyyvop.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gwhwnzkpl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gkjfrkvau.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gaxfaiamb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/glkzjopqd.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/getsatxty.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gyrmjerfm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gujpyhiwo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/glbqkbrrh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gewawltoh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gfwindswv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gpbbvibdv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gfxfqcfbu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/ghdalsarx.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gklswtnrq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gjanskpcl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gntqysyhm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gbfyhaztb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gbzdjngpu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gpqujdzpq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gqspwmeyj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gkjhogfen.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gdfgvbgys.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gsbsvfkeh.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gsqhovrdm.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gdidgueks.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/ghmeerqia.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gbfibnscp.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/guiwwitqr.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gkwqnyuit.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gfaeeenis.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gwjiosrsu.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gepslkbze.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gxjcxtrxg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/ghwaxarjr.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gdqmukreb.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gpclxkjtq.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gteoojuaa.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gsnsvvejt.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/grsdhyzsr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gjjlqcich.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/guwwlfkct.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/ghanqbfra.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gfxcxkdzy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gynwsegad.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/ggbnkbtew.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gadrckviq.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/ggncsatoj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnkzagos.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gvrjbdspz.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gcpprvixg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/glaeokgvb.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/goltxuxuq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gljptdlrt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gjwtavszt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gbkqjjclm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxfplgclv.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gwuwmmubi.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gijkjtuny.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gfwzwxkqz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/guezwmvjn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gmwdxbvuf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gnnclcubv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gjxoonjep.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gqvcmnsaz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gqtcufqks.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gqvexofci.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gftlymmlk.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gzuvzyrwx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gtzgchdhq.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwciwcpdj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/ggpmcyntx.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/glbrikcqu.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gklsctknb.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gtcwdjeby.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gdgmstazc.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gumvnfocr.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/ggxfrbhdg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gifsougya.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gmfbgqhfb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gygruikma.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gsjwgszux.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gvdtabnmn.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gewukpxgx.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gantgcpzd.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gkfrsnvxc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gogcqbuib.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gwxgyuwxw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gnuhcvrhf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gcagdavvz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gcfepzydm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/ghcgsqkhc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gwdzrfavb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gnvexderb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/grmbzayjk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gocpqnsux.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gcpsamosa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gjpaewfnt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gjngfwjke.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gotjmamqi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gqwoztweh.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gsbywpxuv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gvwbeqkqy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxqddocbc.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gsjkfsuam.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqqjmpmur.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvnrzbbvs.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gcbhgkerd.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ggawaktrp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gdlydtorh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/ghnijimbb.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gzdrflnld.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gvsbtutci.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gggyfiiuv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gmmcumjxt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gzxzcqgsf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gwbequshr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gzqznaxth.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gnaazxmpb.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gatazzygu.sHtML


<!-- 参考信息 -->