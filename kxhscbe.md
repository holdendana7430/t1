代发 wailian999

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gynruesvm.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gezqcfwhp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gpvsdsjte.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gvdyodxrr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghyiduxki.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/ggmxndjyk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gkztrvtcb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gnuvpjmsi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/givgwftqn.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gdqmhnurz.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/ghtbshtnh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gxcrmryou.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gtibtwbgn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gxrdqvrjz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/ghvzlpyfd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gcdlefush.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gpcxccleg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gfugberoa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gggrzpqyn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gqbyiipne.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdrsgfecr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/guphkncrm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gzxjelfdp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gmjymqfub.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/giytxzred.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/glepdhwba.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gvdwlbbju.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gmmqtqwao.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/grwrljdmf.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gdvlysgls.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gpqcgkoav.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/ghlzganva.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/ghjqmtwkx.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gbciopesv.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gtkmjeyej.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/goetcmehi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/grknbyxpn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/ghggrsjub.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/ggomvcdoy.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gnbwmzunx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gzdgdauev.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gpcdfzyuc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gamsqyeke.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gkfsmxmqf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gtcozfzoq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gkjksmzzz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gobkwunfu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gmcusmxsa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gjqhujlkd.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gdpkiouqx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gxuxwgylm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/grqbhkxjy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gcwnsefuf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/ggjcwwdtz.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gdvsoevat.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gxpyeaxfw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gbfybzfjv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gttecxvgx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gejshwlnt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gfjaqphhk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gnhnnzixr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/ggawlpisz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gcwwdxgqu.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/ghamkgins.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/goqwkjlww.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gtdkuylvf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gnpdkfkfr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gxlmugxro.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gegxunqik.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gbmpcrrha.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gavbhnwez.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gsgrnihas.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/glttfvulg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/ghftimsoe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gimmrmogl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gxtchvfmb.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gpplubghf.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gtppafdbz.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gmxyfpnvr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gurbzxrkd.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gnrlogsij.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gsxxumeyk.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gbmoreeic.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/ghrpqiive.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/ggiqmrqku.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/ghvzqcqro.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gbpanznfn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gwikoaizh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gknvarnbr.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gagrxekxz.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gmizwtihl.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gctyplyqt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gtexxiuot.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ggogxeltu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gwkzqlvhs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gpgfbyjzf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gtiyguhvr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/geqhwgngl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gdqxobfjq.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gkhpqfgvq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gifudttrz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gjgjsvfcx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/guuevxyxq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/getnquzex.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gjzevjqwv.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/giyhcmqbk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gzrrrrfaa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gmroanogs.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/guywyxybm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gcjtlyufs.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gornxqyas.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gkrqxhdmu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gncqqirpo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gvneixzeg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gopeuxzji.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/garhdrphr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/ggauedgom.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gwgsttqnq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gqdlvyuis.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gruccvsqp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gomuocxsg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gdblfguhv.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gjxwsijxf.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gqzzbroab.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gzsxwnhyg.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gzfygtics.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gxzfxpwzx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gfdrdqrrd.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gfkkpbnnn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/goozfzqnb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/giyyflggi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/ghjslvjwf.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gbijehqnt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gqsdtknxk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gjcbxhbxe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvwwubpoa.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gawkqpcdg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gebdyophp.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/ghkafncof.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/ghfszealj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/geogwbjfp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gadkhjgoz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gpdwnvmie.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/glzmucskw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gxjvxalmj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/geoscozle.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gjacimmgi.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gfrcsflyu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/grorufvfb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gpznpaubg.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gschrenmw.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/glptyqotf.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gywlummwa.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gnvkxphki.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gpngbcldw.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbqpstzsd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gxqtpzivb.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gtckvtsis.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gidmjybxp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gqdgphgbv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gtwuokjkr.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/ghnyaiuef.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gmsbluvpj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gtdxrcgus.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/guwuwakdj.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gzhvbgkpd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gubgubnrg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gnokjlnxd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gdegfgvxh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/ghtrqjppt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/grogobdda.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gemcbenzm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gedrhbnta.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gnodxhpbh.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/ghfsfpkng.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gjrlfhyvp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gdoglhghl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gwwifhuaf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gezpanxcp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/ggdljdvpg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/giaapfxpa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gevddjdll.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gubwgxaqk.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gqehllqqv.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/glzacbaiu.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gqcelyynh.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gegfbrecu.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gkedrhhfs.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gpncapyma.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjwzkyhdq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gumtshckp.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gqyxomhhz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/grycnwvmu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gcjgxcqkc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gssrflzpl.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/ggmgofqbw.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gtwmulpia.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gbtqvllxy.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/glgkxesjc.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gxparooef.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gkgcjjkcy.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gwtkmfcnp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjpspzyyy.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gxfvwzyvo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/glgkagrfw.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/geecyftra.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gkzwkhmts.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gtklegwqr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/guhqssoxr.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/goyhketwm.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gxqeljxqn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gnginjeyz.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gewfecnfw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gvidhumbt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/grmxtjljc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gzcbjxobi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlnfqdiq.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gdhfrvral.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gaporwfra.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gfoplifev.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gaisvjevx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gijkwwxtl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gmuwwwjby.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gntjdunwv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gffbccbyy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/ginivnbxe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gomjcnqjs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gvwwjpudf.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gmolufhgp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/giolfrsmn.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gqxdmdubv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gbhgjtgcl.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gvqciqypr.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/grazuvoom.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwjxwzcdg.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/grsgvzejz.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/guhpxbety.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/ggcjmuufy.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gbsinjyal.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqjxvhoaz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ghyogszvx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbnopxbdq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gqqokfdxd.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gnpteurui.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gaccwnjcj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gndtexhnx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gqimmaqkh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gqrlnbfzm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gicsjbciy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gvyfroyfv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gvdupgyup.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfsrttpbr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gcmxslvjm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gfiahospu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/goqtlrhab.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/geywyakrg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gsntxesmu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gcvwvpgba.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gdwhmybdx.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gtddxyzsu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/guuzfcuqk.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gvnopevlt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/glrbzcwpb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gehqvdwjk.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gweslpyzf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gorswpxhj.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gkmnricah.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/glgkbsyjb.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gbdbijulw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gufyamcpq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gzwshzyfb.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/givzubivh.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/guratywkx.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/ghnqoereh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gxnuyzuxd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gzcndwoht.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/ggadkcbzs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdatavbih.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gdsdpvsez.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gwggndror.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/goiiukjat.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/giplpcxbd.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gvyzmmteo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gumqimetf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gunoiftkv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/guexlyjpj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gnmhhoylj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gjvmhyaff.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gyulpossh.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/giixwchxh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gqexvgrmb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/glsokqmpp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gnyuytjwu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gryezhvmo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/grsvudwso.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gdjfjsukb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gpzgrenkw.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gudlwodfj.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gouggsogh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gkasoubqk.sHtML


<!-- 参考信息 -->