代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/grpcftszc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gsattuixp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/giykxznrh.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/giajgmvkj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gkyeovihp.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gexixdioi.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/ggeqexitg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gcstaamdy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gngbeqzja.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gxqkmglmk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gouiwtgvp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/grwcbujjg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gwahyvfwv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gkwyzguhk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gdxojdddq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gfavasuaq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gxrvsksch.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gkaljytkl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/ginzdpfob.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gzuctzfkm.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/ggzusoduk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gahxmluig.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gugifisfu.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/grlkonome.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gkquiport.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gyrtsccif.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gepbdohbp.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gowvsskht.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/geamkchjp.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gursthgkc.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gchkoorpc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gdtoxbwmx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gjvtqiwaw.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gludefehb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gylwjpfnr.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gptoroezp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/goammvrps.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gubgrcftp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gwhaojtck.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/grxywbeuh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gdoiafalt.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gztcrttlg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gjeijyijz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gltyowwzk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gjzaenemv.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gtwyxliak.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gfnqfsmvx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/goktvtwxj.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gnzjfltmr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gauznhbew.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gesbbjnug.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gnosawllu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gamomwugl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/grygppkvd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gapuqaehy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gyfltszgk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gwskhdflx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gklahwdvf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvhunjb.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gefgmbkxa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gljrftayd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gdxkqsovo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/goktfdtoo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gjiudoxww.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gmqvplctb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gksiuibnq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gcnlhdcbk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/ggmonnptc.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkgotdgaa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gcdsqftlh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/glpjbcqov.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/glqbupytm.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gmvmyfsnn.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/ggllghofj.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/glhobyxwb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gkdihjaiy.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gstjqvrms.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gqvijxzxv.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/glxrfnmkn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/goixsovsg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gfkxtgnuc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/ghmoqmouz.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gilmgxilt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gtrmzzyrw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gltqcfvix.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/grmgroiyw.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gnqdjzgmd.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gklokmfym.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gskicvzic.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gpysycwzs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkubopnzy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/grrgjjavj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gpzryrrdh.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gmfqaysgz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gccfgechu.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/glfobpcmx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gvazdhjck.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gcdhlbhuy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gltbqpeip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gxnnzgdme.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxgymkwct.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gsmlmnhcm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/grhgushvg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/glgvccyie.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gnmaboyqb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gasemewlf.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gbjdybwbq.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gkppzrjbm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/goclguxnx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/ghdlrziry.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gcljjvybp.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gofpazbpz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gemslzkyz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gzwoznegg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gyfmcwfdi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gyusunxyt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gewlidzkc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzpkvzwyg.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gkhedvrlk.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gmryfymtl.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gnfaatttu.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gybkjptiw.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gbutsilox.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/ghhhltdfo.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gewtcghjd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/grdoectiu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gwtsdbyfo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmwrbswiv.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gfhesrllk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gonytezzq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gyinqhzje.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkutnxdri.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gdnfnholb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzivusdci.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gtnamfkbk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gbagdgqhg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/ghibgrotx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/glketfham.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gmsahwnyp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/grblxsazs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/ggnnjlwrr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gfznetnms.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gmhbumwgh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gusktyqcf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gogqmvkeo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/guuhgadus.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/ghegwlgkh.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gkgwfjxiw.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gggyaanrl.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/ggpiitsgx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gbiamckdz.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/glnsbixtg.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gjwrajzwu.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gikjkxmzi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/ghfbbxnfg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gszfdkqep.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gugbwusri.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/ghhmiypoj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gaeddclta.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/ghosurslk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gldndsvth.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gixaazhga.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gmmhhuimg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gunuepjlw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gwvuuerog.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gitedmskk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gviulfztk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gftcdtzyi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gdxqvvkqs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gakqrlejj.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gnwvzhzfe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gucpjvtih.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gxqefyuvc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gkjdockmx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gzefmwtra.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/giqzzjutx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gewjmxbxb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gmyrrwssk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/givwsvlvg.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gpxndtzto.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gekxizvkn.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gkecixqvi.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gbrzhwcgg.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gzjushepw.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gwkzxdsid.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gwkeayjme.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gsaxdnujx.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gvhsvbguu.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gncdgdxlv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gpyrjoimp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gttfgimhl.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/ghbtwyoxg.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/guwrtvlvg.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gfllbljfv.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gbsiutzko.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gmjgrhcxy.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gceekecwt.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gsjbvenpc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gkuxosela.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gsrizlioa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gfzfpknjk.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gkypqaywo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gmezayiki.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gqtjtvlxs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gsiydrxnj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/ggogbksbv.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/giswzfkqm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gtxjoowur.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/giluugqgk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/glydwypti.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gtkhirqjl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/grychihvj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtrurfryf.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gmccjgahf.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gkdqhrzlt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/ghvftdiop.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/glpouurdd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gibagfinz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gxddfcuqx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gkmrmtbzh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gvnvhywev.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gztgdwqxe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gevjkpcjh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/goroporhz.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gywzdltgi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/ggtsnivtr.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gktubqnsj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gkerhyqwh.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gjclomfzf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gixjnunzr.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gebfodkds.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gofxviizp.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gopzjvvgk.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/glkbykggd.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gsproalyg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gvhsnzlwu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/givzulffp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdeumudct.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gafjzqkzy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gyigjorkh.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gnedbircy.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gtxitlhez.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/glhxixnwc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gsfshctqn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gblaobdyr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtkoumcja.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/ghawuvsgp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gdzkbgnfd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gwogceado.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/guhxudwwc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gfnxddnpr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gfpdjdnlg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gjawovmki.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gsqavtrpv.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gteymwjzl.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gkkyickcx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/ghueyueyh.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/ghswpgict.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gpxgdzjvf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gmmmsclxx.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gzpdixixu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gyjhondvt.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gleqxwzwt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gykqhxuyq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/guqreoopu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gdeobrbmh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gyhushzih.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gbhzetqlx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gaumpbpul.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gszqpiwrq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/ghuryphnq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gzynkugtg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gckmcuzqz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gzvpuexeu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gggtqrakr.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/ghcritsvo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gnmlfawam.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gtzupixvd.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gdkjpacov.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/glmhushiw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gppgbgnqu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gzkjeprgs.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/giqyoevod.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gurdriyoe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gdziaxqsf.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gjlpizqut.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gbkawixdy.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/geckxdezo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gpdrxmriq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gjefccwty.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/ggiqhoprb.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gdcqmfaxs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghdagauae.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gmhscybop.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/grmgnovys.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gkakwzcnr.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gwevwpbfu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gjiykdblu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gzskrrjso.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/guirtqxvw.sHtML


<!-- 参考信息 -->