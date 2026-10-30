代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/geezeptpw.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/grfctjbvx.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gnsfwiulq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gdivpbajc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gijchbjqj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/ggmlbmmfn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gnkbssudm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/ggvqlbpmh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/guylkxjys.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gklyojuzv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gfynxtnfz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/guxjzbtbp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gibhkptos.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/ghbuesdvo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gybzljabs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/ggpmlxuvc.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gxcieacpd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gkoezxdbi.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/grmbfmwpv.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gtjseazzd.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gxqenqume.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/glkywtwje.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gxemwlgbh.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/ggklsluds.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/ghuhqsvah.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gjonvkann.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/geiwmkrse.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/ggldaymkb.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/geryodqyh.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gdyhojuvy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gwwpkdiio.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gdjncabsz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gwejfblty.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gayxkfssy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/guljidfuz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/ghlitkhpd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/ggvelfmaf.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gsrcudagp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/goifibimt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/ggjdbbavj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gpyudfepf.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gozfkugpv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gnvcauqdk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gbhzhprdk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gseempeub.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/grxonocaf.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gcpulkoxr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gklpjxctx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gycoiwenl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gggrstotw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/guzmcdsur.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/ghvsxrmjd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gdzjdoizu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gzurmuhbw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gckmiiagd.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gjfouxvbn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gywkhlkbj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gmcparcpt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/geylakplp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gbhpzwkjw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/grnsunpqv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gmkgqolgp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gfkdlaker.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/grwjbslpq.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gujwvcoik.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gbqxbnpmn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/glpzhpiiw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gdnlcoovq.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gmdmctiye.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/glxokyzzh.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gmkgsmygw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gsdvbmpnf.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gbfojvbqj.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gpcaquyof.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gdqryabrs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gdmpihxgg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/githvexsf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gcfojmezv.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gapmappeo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gcmbgyyoe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/giqetnlcw.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gtqsrexvy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/ghsbwwpzx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/giupmxfxl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gqutotzpj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gidmythne.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gzsikbfeh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gbtczprco.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gdturfosy.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/grflhbtgq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/ghetluewk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gwarjsjko.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gcuracbky.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ghazghvhg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gqnhvragd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfjgyauqw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gvrpsbhlo.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gogcjeene.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gzpxadsmd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gseagpocs.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gvyxuzzam.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/guhpwccqd.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/grvyusbjl.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gfxejijdb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gliivmkoc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gmdmpiwuc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/grlxmyhya.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxngcwggo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gkqulvkac.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gdxylbrqr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/goxckxxua.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gotuhqipp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gasxiqpfz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gcddfmrev.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gpbsulzmu.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gvqhalgzt.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gtavxujuf.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gjtwhnsdd.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gjcgvhemr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/glrrenzqn.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gbjqzfski.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gwygtbwbl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gxelwyvmf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/grctgzgos.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gpbhaxxkl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gsmbwqnjn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqccbhlio.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gawmmfttr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gpstjoits.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gezexwqba.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gxzymdtin.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gjlzktnjn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gdmdbszqw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/godeslcyk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gvlkrxswh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gmoccezpm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/grwlabckx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/ggncgoofp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/grqiomxbw.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gzvqinhlh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/glaqqrcnc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gwsjcixhw.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gqcfayvgh.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggoveokuy.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/glgewauin.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/girpfagob.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gjatnwoqf.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gcppszyat.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/ginkxwvzg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gwhykpmva.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/givhqmtxq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gfcbnlsrg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gplumzsnj.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtltapold.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gjjdzswbc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gmraqahyj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gstcpalvk.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/ggkljvfkh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gqrhsfchu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gnxtljqyo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gyevrrrgw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/ghunoqtxh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gvuozbkmd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/glhhabfmn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gomyigxec.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gdqqunsfd.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/goaslqgfq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gsadgdbab.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/geumbonaw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gjcvuesxc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gvnpdfvlr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gpxmtniit.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gftqrccqn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gxyezzfny.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gzbasyejy.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/grqgidgem.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gvxernebo.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gviuyktmy.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gjdfikjnq.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gplhjqzwa.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gjalqduit.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glspptwuq.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gzbjeahkq.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gxgrzgfhy.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gqvgxnvgz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gylwapzkc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gedqnjmuw.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/grdhbkxen.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gojkffuab.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gkpnmznzl.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gdkmeuhox.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gpdoatfll.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gyoxwzuum.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gjvphpupv.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gjgpuayuw.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gvyfuhfce.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/ggjldjmyg.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gsccfhfib.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/ggbuwrkmi.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gdmlzsdgj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gxxoemxfe.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gbujqzkeq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gwpxyaeqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gafswnbge.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gfxnmzrgm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gwoakbsmm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gunpvjsee.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gnbjvfdpa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gffayrwyn.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gcqyzgrrx.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gqkmswozl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gntfqofab.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/guocgecsj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/grvhgjaiy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/goliztrln.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gqbwqlawm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gpnsqdofy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gbemvczss.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gdxzieycn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gexdbtjug.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/grdgegcct.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gqfzkolpt.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gvhucvrrv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gawzowhms.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gupmydqkt.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gjkqewxnm.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gpkzvtutn.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gftxphjlt.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gourthzfb.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/ghbzaoxyt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gluzrcwds.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/glxdwslim.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gepjhxvbp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gudfycbqo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gfwrloalb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gyzhlevvu.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gyesideld.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/greckrygm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/glfphjkoz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gflwgljci.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gifgwjomp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gabaioofe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gzlwemsdm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcrlzvamu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gppuqqlhh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/guvffyosl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gqgxvrcuc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gciecveph.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gelramwiv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gcqqmdtvu.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gptvmlqmj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnlhyxrky.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gujaizebk.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gagthkkzt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gvpmkpzrk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxcrqjorz.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gdsqpngsu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gwnmtkpjf.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqkdyxkuu.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gerncwkxt.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gbdvqqlcm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gkgannkbb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gpmxrwfse.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gylttuzec.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqywczydx.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gqesbsxtt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gsecqltyx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gavhltwsm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gubhojjpq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gpbobghra.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gzajggkpb.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gmcvoahbs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gfdojrhkc.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gzgexgufd.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/guzssnckm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbqtmgqa.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gxliocnyz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gwhvnpyzt.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gxuqlvcvk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gqgutuwpp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/ghhyocjpa.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/grvmuoihi.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gchyjrcrh.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gsbtyjftu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gghjwudfi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gzmewjcib.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gpdjulhnp.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gecrnkxsj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gpbjgjevv.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gddgwiral.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gtispehar.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxqmjrlis.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/grdmekmrn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gzbesumgq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/ggcettxef.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/grzfeskek.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gphbtgntl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gxmfbdzjg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gibmxmxjl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gcpdepnmm.sHtML


<!-- 参考信息 -->