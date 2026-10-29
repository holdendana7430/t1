代发 wailian999

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gywmmnack.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gqypdiayz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gstuaznxe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gpgswdbkk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gyrgbfoah.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gwuzvwlpp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gquxinrji.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gwupwzbgr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gskdvhxih.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gjgthskdl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gtkzdpcam.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gysvainrg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gpyaudxkq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gfsxdelre.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gteetywpy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gwbxbqlmd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gkbqcwfae.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/ghzhiijuz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gfnumyxyv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gjqovmyyf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gwhrvoqli.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gaqluplia.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/ggdghgxff.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gepekvrvc.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/ghyezqtif.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gnykglnvb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gsfxmgqng.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gqvcfvhke.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gfppbpdup.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/grsmnclvy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gdktggjwd.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/geymbkcna.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/ghzdmvqxh.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gzufzsaos.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gjhmaeokb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gsmiagxyu.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/ghkepwrny.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gbddnvafo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gqsgufkdl.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gywqoadxr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gxvrheksg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gocoxyftv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gayarcoio.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gdsvrjpgk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gbhuaczyu.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gsvoapbri.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gpkkwlgur.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gjbnwohgx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/guigrgcyx.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gvjsimiqr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/ghjpjbxmm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/girksoshd.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/grxgypyej.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gimggcylz.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/ginzznmxr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gjuqbcohz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gdxkdmplv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gfccvoiyy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gdatlbjqa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/goguyvmnq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gmwrgxdxm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gnlkebnav.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gkxjkkncc.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gklfdlivq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gtuanqcsp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gemoqhwrv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gusaqvkph.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gznshnugy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gsuppeiyj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gmwacqacr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gyvlxbgmb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gozgcksij.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gwbvaqlls.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gujpcmeeh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/ggahyfagm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gwtipdizz.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gkkkgdkse.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gyqwlyxfl.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gktokpwqf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gojtsnoyy.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/guhodxbdy.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/goedfhtkp.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gcmnipleu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gvbocjpep.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gjnisowiq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gljbervjc.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/grznuhkoe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gqsdvsqmg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gnxchynud.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gsbyzmxqo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gkucekahm.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/glrxjhiln.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/glaqgiurd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gekreabwn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gejrdamrj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gavupkvyw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/ghqholpeq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/giuvksvzw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ghkxxrbze.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gisvhbbhr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gwjzqzsgu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gzspdyeux.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gvlgajvfy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/geezqdfjj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcdhcfcno.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/ghvcfcdpt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gpjjkzrrn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gbsrfgviz.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gogftjjpz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gvssiusrg.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gzhzmmyhm.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gmqvsvird.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/giodebuxt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/glnwnpwpo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gcvplsiqg.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gtxgjwbog.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gddvxwxje.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gzrizojrl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gtynarouu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gsbydamzu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/ggzweaxnj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gijwlduyq.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gmfggqdqx.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gwygxkqxl.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/girhavszs.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gvwzunlbg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gryprqwgo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gpuywxihu.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gjymmmlww.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gnnzkveth.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gtgrvmnhr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gdfeknlce.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gdgxoietd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gxwdaiads.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/guvzubyyb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gctfmpgld.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gyrloobmr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gajrzjuay.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gmicjweut.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gqdvcsbeb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gmmsouvhd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gntxypybr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gqxrrzyzx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/grpztibjb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gnjpibbdh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gpeyewiwe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gbsnohgud.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gnzrcjroa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gaqfmhiai.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gggpthuxk.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gilwqsrlt.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gdvcyvgvd.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gurxjkydf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/guqxwwrdx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gevpdkhms.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gupmbzeel.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/glqlaudrb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gsqmhdutq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/galfytlag.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gljlwgqhs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/ggwjigtig.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/giwnaheyk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gytmnmkmc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/guqacrrkz.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/ghhtfygzm.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gtlkwitvx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gekvohezz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gmhddhehc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gnjhtojbm.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gjgpgfvqi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/glcpglfez.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gnbmwhttt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gvuainlzp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gtmckkfut.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gsvdpttsx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/glowvuvfy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gbdhxmeqb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gsbjzslbm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gzbnmgkrc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/goeasjrfl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gohlhhpzm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gcqzrwfsk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gekcpzhvl.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gcerqxlbs.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtkocnjyg.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gkpegrxib.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gelyvwftz.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gxuevvamq.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gxrouqeby.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gsbafseyj.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gevjiearw.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gmmusxkkr.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gltyqpxrc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gtqffbfck.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gumfapaii.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/ggicxqhbe.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/grcvfmedz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gtigdwrzm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/goimhwxfo.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gdveoyclf.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gortktqhe.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gzsomftvr.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gzntkmswo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gwcvtgikt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gwowoetih.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gfhucwcgt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gensyrane.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/guqneynem.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gbnkrtzcc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbsxipqik.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gbjbyoptf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gdlikfwvw.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gazxohllc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gufafjpsv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/glrcaywjt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/glvtlojof.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gwhtphgxc.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gplcangkc.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gzxjsxijx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/grprroqmq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gzrcbtujs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gsdvmyoqh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gelzbexew.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/glawizcog.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/grmrtinfs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gscthsrks.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gdryzfrfa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gmihndiby.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gckixpuqm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gcscqzciw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpwygclwu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/glkyanuvc.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gjitwvktq.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/geiedpgmf.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/ghoanwnam.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gypktqsyc.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gvtxhrbmy.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gvfhkjfrh.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/ghbdudytc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gzokpuueb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gvbjgmwcm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gitsuegvo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gkhxmwjfo.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwxscyrjq.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/ggzuzivjm.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gpelreiag.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/ghfdljahk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/givjitkdr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gnurnwqto.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/ghhtyqkao.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gysmiglup.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghponimim.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gmjfygego.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gbmuzzelp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gvjsmtobu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/ggihwaobq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/ggftinatu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/guoywcqbn.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gwdgxogeh.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gxnzagsgp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gcbhfzzcj.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gqbarfosu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gbajiwdvs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gkqydrabp.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gddwwvuah.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/goiaarolc.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/glxlucehe.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gpyljzjhv.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gxolorexx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gedmijzvh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/guorcvaew.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gcbdirsoh.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gkkbngmvd.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gqmokxong.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gozvruhvr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/ggfivivjh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpmuafkyo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gvwonrijz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gttnvytlu.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gzvllumqz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gtrwtnkdh.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gwnsnajmx.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gwnamimpa.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/glpdzognf.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gcfhpzfcg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/glfsmzpbp.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/grndxdbzs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gvyhvylfr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbhhcwnlg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gujwweeie.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gyasoiiqo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gueghtepf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gtnprlpcw.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gnvgwsyll.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gzfveyshd.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gjkfkvmin.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grsoigaum.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gvgfamugx.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gngzwaeoz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/glxdtuykf.sHtML


<!-- 参考信息 -->