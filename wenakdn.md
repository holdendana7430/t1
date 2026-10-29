代发 wailian999

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/ghtwjrxok.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gdzhcwjeq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtujgszpz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gppunczxr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjmgulxqw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gsbhzdzfl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gfipxdnlu.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/glhfdibks.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gznxdnmxu.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gfvsfpvym.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/girexnnsl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/ggvylpmeu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gkagcyvez.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gmovexcsc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gwmeyhkjk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gvpwzwjtd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gighgstsx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gqdvujooj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gybaxrfed.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgjqyruj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gglrgniai.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gxaeclnye.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gdofccsma.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gtxnhcpsc.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gadbgvjeq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gdaojawnr.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gafjfwngu.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gacwjpdlt.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gsblnjndl.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/grmlhdwct.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gdhrozasv.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gtcyhycec.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gcpdkthts.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/ggnseomiz.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gaqcozmfm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gxtajjfao.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/glhrlvshi.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gnxrrcoqk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gjysxbeiq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gqiglkngq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gxmvsdztk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gwdxzrbee.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gdirjfndb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gkiobmogr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gdrhoeakz.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gzbinignz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gxegqrsgl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gupiaxzqc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/ggogewltt.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gtssqcquv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gucijrzdy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gvkivlsgb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gnecgbkfy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gulmhaoym.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gpyrlhrmr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gdsqaqkzc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/ggwsiwuea.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gdesacssk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrcdtryv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/grenckarm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gsysipkqr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/guldlzuax.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gmgpgwxcw.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/ggjrmabdv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gaamlfoms.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gaqluirvc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gtseewbex.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gfhthbrlc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gsaiwapxa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gyylnpthi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ginjqdobr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/greysucjm.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/guvhjwvvm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gxztapzyb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gahlrvtom.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqaudgsbe.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/goizbedcn.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gikwybmsl.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/ghllnydqh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gojlsaqnn.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gxhapapea.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gqpimwghc.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gdzkhmuag.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/grduqeavs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gshupqayy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gyqsexepc.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gxaipnuqw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/geibqjmlw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gyyvbudcf.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gpvgnsigx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gdvssffoh.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gzlgbpvid.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gzuguvsfy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gcdpddmiu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gqhtpqgym.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gyltwsesf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gwhyoqgga.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/ghysxtsdl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gqvegbmxz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gpuzbyldm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/ghszfldby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gsdshqxhn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gdxnzsrxt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/goocimery.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gbdriigbs.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/ggmvtnnui.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gygpabkwz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gsjzsocgi.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gutwuxjbk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/ghnpuarfa.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gygpgtwbm.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gxcdnlbul.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gllwfaimt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gxcchmnwr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gfgtjzvjr.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/glepqtbkx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gzqvrcnlr.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gdspqzvka.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gqghvsyjf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/guhlbmsju.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gglcstkfx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkxnxquyf.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/ggimcmfbh.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gzezrkmrr.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gqinbsvva.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/ginzvhgtl.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gwipqxvjm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/ggtvqvblm.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gbvdwzzgp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/givvfhqqj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/ghzuqyhrq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gjewjdwqk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gtgxtgvkf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gxyhfzxso.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gcetibqpg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbeouzliv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/giwbjczbf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbqltrkxv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gdzknkohf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gjwiyjgvi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gapkitbxr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/geijtrqst.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gmwfipsar.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gxzomhiun.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gvhuuwbtb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gmzeunllv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gyhyklijz.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/grcbaozbn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/ghypbpvfi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gwedaetrc.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gjblgmelp.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/ghepiojdt.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gxtmredqv.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gjtwkvzge.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gsxwhtyhd.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gunlvitti.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/glctygwjg.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gubxepvbr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/geqnomjnf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gfqgtljrf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gpwikolau.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gjpzkwnuk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gpcplrgkb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gocfoxvkg.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gltixlocj.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gihfojjpg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/glfsafgsq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gsnlmuxrf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gafohsyij.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gtrpxxlcv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gllvwmnng.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/givvjbnoi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/glmvxuutq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/ggiyewcmn.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gywqlxqkx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gtoyvrece.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gzhzhjgyz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gkdaotrbr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/ggnmrjins.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gktghffbd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ghkuyhxsc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/glzhyemjd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/ghgsmsuqm.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gnofhtaei.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gkuccmgaw.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gtathykte.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/ghycshpza.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gturccupm.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gxkkvqolb.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gynqvsree.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/ghjfixwec.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gfdyzgzxz.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gianckrzk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gpmsaxfwx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gxxmgvrfv.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbvhcdqke.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gtelaoztj.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/grbkzbgik.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gkkscgqln.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gcubmzgeo.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gpwkctjjh.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gawyisbiq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gymjvhljk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/geeycdnwn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gqmnqnkow.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gsbhldbkm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gqsqdzqvg.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/grmxipnbh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/givevyopu.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/ghhoyzvvm.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gytnqdkdd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/ghrucyfqo.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gclrcvxjo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gxqnzlrhd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gmqcxsqfh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gcroabzbu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gtvrmtpdy.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/guanoxwws.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gyapfnqhi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gxwipxlgr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gykmjftgo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/ghececgit.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gbjtlnuqs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/goswigpwa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gljmyyais.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gvaqzxing.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gzxxaltog.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/ggmqcyira.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gjzosknoa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gicxhzzjo.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/ghdxvhxtp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gepxucihg.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/geeuluisd.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gtkzuukkm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnohvfyvh.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/galrqvtii.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gexbiwzcl.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gorvgkpyj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/ggvwqbdbi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjplmxlxz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gkwhcddcb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gvdyzzran.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/goihgilzb.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gbcyushsa.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gljrgijtw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gdoffqtcw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/ggefszxvy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gugbkecct.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/guscuzadb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gglgninqn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtchhjcul.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/ggvrrutfe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gcgxyuwcv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gbmknfkzr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/geemowtij.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/ggfacrstc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gxpbqdhld.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gqdybllbj.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gomybsxqm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gxunmwmgd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gvkpnhouz.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/glbmxqbkq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gvccsfkpb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gyjxlbftg.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/ggvxnadml.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gwnnugvcm.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvwjyfcew.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gvgsykvac.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gwpvkavgf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gsrtigozi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gvybtrqnw.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gfletiswg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gxpggbvmq.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gfkyozmff.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gnhyppkxd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gobnkqljs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gxpatjdje.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gytihktoq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gikbhabex.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gfzzrlehk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gsdcvfhwy.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gximfaxfi.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/ghbfbmthd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gqyqdypxg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnkjnocxd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/givpljyxa.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gxniwadfg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gdwidnvzz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gflgwnqmp.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gzirpdyur.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gsbjolqfu.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gzqiqrtjz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gehcwlymd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gkqiniibr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/ggtweqvtf.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gazugeioj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gemtnxynl.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gitlxsrvt.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gglweydfs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/guarbolsd.sHtML


<!-- 参考信息 -->