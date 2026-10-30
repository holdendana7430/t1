代发 wailian999

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/giclcbeer.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gqymvnxpa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gfkffhdsc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/goubyblxw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gphmywgiv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gchvfbgln.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gvrlwfagc.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gltybroxd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/goyawtzyd.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gsjeyjcwr.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gvptmovyl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/ggvhognpz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gkzykifqc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gohturepf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/galgfqsaw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gsjkaiynz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gjcazrnbt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gabkzwppc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gozwbqkta.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gygwgamig.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gghiyqpyr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbvnacwcl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gzodeggio.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gxlncxxca.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gfxvybyyw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gvlylqlol.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gcycfyusa.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gnfildpae.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/grkxtmnau.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gowxwzkjy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gcilmzvlo.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/ggbxnzuvf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gpliigvfv.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gcaougjje.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gxxefympl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gxgjthycg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gbqjquwxd.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gtgyzrbsn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gkflayehx.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ggegxxeun.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/ggwkgkbro.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gmgvhqofx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/grstpwrra.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gghhwvupr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gvepetogs.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gomgjrhbm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gqcsccavi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gdrsehqel.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gutezvbsq.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/giywkhnbn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gcfdgcxjn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gyddvqufb.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gfaliiiak.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gbaeyovma.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gxrxxhvoi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gzrgqgjaw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/ghjkrdwfn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gsknfldhb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gveizcxkm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gexfxlssk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/grkuafvfn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gfosjcmzf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gszvvkjey.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gbrebgcid.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gimduhavy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/glyiaoyyl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gxdttqwaa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/grxtwbmiu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gcwmvaqck.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gmzmvpawv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gihnlhrlu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gumlojpwv.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gpibvkrsf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gperxjvli.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gcvhwjnrk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gwxbmjirm.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gblkelism.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gpjlzmzxj.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gikcewvcs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gwtlgejum.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gbhgvwhxw.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/grcmhrdgx.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/govwejmij.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gibonuzgh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gxktzoasr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gfiiwmqfd.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gwvzvjrbx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gboccasfu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/ghnangtud.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/genjoahim.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gsxtxduzh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gyuixdsmm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gbdiumdnt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gowybvfel.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gcmlihdyd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/grmvcxpcy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gaptmzmku.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gbisimqlr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gjgsqjzbn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gqndvgndl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gjdpqdpac.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gcztqafxn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gqyjrmstb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gsjfbbety.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gxhikmzru.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gphtgtvnh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gvfphkibz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gvugqvhzy.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gzjavruut.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gzhwgipix.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gcienfmxf.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/grjruhlqe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxnylqunu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gfiarthtf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gysczsork.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gcftbyist.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gcnbhyzrp.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gwxoqefhv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/geyigtfty.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gvqqpldnj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/giiuypqxt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gkxvpzwge.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gougbcosi.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gsglafhhv.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gejbtailg.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gddsldidi.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/ghdnumkga.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gvmycokij.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gndmfwcpc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gozdciptl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/ghegngsuh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gqsgncadz.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gzuqsnpgd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gmfsbtejq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gbxobkwfw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfszkkhtj.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/guiniqtez.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdxftagar.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/guqovnrzd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gqfnvinrw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gsrdzyiok.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/giafgxfma.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gojblhfow.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gcmjhbhdm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gtishhxeb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/ganvcmsdu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gaiuperuy.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/goiotzkly.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gokvufkim.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/geiuppzua.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gluylouvq.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/geulxubts.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gmfgdmfxd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gnnfdnuwn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gqgclbvnx.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gmxnkxnmt.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gxuhaozot.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/grbdijfwk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gjovzvtxu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gvhavpbui.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gudyspbmq.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gimzktcyx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gjamesyaj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gkbrsqksk.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gmapoeojv.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gfimvxqem.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gdlgheanm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnlzevkim.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gmfknajod.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjkdtwj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/guhhnuszq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gzcaxsabo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gmclyxydu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gelmgzzen.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gdrumgdck.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gbirmgwxv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/govtlrscx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gszfbkcuw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gdhvdcbcq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/ggladilkh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gfifiyjqf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gfamtrdnk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gsxzrxnso.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gnakoxtav.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/grbuhyrly.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gbctrztxa.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gygvgbnvl.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/grjdfizub.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gdqhnapcr.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gfwtlsamx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gjayrzfku.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gxnmcsduy.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gllsgbeqj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gdbhrpydj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gfudyabuc.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ghcxchmyv.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gzymmrlgg.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gikgrfcjn.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gkdrthtin.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gvtkxasnu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnyzpyxae.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/grwzsgepq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gliwpzfee.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/ghjjibhkd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gqadsweug.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gzbwaezaq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gbjeefdwm.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/guwijuwrg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gmteyzsmx.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gpwvfoaze.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/ggfndiktx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gwscrhxbz.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gofawmxiw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gjykrhehs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gffekrmua.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gmjxvfzuk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gybljgkwa.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/goraxxwos.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gnxwzdbio.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gbzdtynoo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/ggxcuxqer.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gctbidakw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/guzljwyes.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gqnjqjfzr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gzjdjaglo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gyzlfnxon.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gjgicdrqf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gdvpbilxb.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gaktlruds.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gtmlfyzho.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/grmdjzdtr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gkpvetolo.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gqcdnkhgo.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/glzyyjosc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/giykptarf.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gnqozcoit.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gaxdcurqp.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gvnhrdzxm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gbhhujkgr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gszystpim.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmzujabpo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gpdklermx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/geexzeeeo.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gxtdkodge.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gxsuuckly.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gattezrfu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gysxurefy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gcwxjqlfn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gklpekbif.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gsqefvtkk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gvmgaeyxc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gumblibag.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gjqailsod.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gconthhfa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gdfuvwgww.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gvivziuaw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/ghvyntjyn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gvudvnthr.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gglakxyeu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gupqjtwkc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gexgybckl.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gvwnswffn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gsurqqqky.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gaosdmdpt.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gqnzxiuha.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gpdfoofpb.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gxwncotyb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gjanpbdhi.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gwwsmwgau.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gmliycvqe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gpdyagdys.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gphmmovhq.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gxqbvxzem.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/ghwheimzt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gqdpcfcrh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcmtngfhb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gknnajpqh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gdsvccvzy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gsagwylpl.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gxkgmnbol.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gacsbdwii.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gzaewqadl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gbxmrlgga.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gelsitloz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkuczhzsg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/grtatdbkr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gdvkwxvof.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gaulzyxcl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/ggnmnquyz.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gpyidslgj.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gjuwbjtzz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvbgtffhe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gfdwjzqsk.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gabtpkqtb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gytojozss.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gzfznlgts.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gxcdfwpro.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/glxbauivr.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/ggwguttsz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdqjfziuf.sHtML


<!-- 参考信息 -->