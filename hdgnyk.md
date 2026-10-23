代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jbtttccw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3lnmyyfmp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3nwocfede.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3aaqnuyol.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3lxqjwcbp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3edvkmnvt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ajuxfujo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kejdlgqg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sznsfqnu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmflzoex.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmagzdmt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3sojokfwl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hqxzyjty.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zhobanld.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dsxbdyyo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wyocbymz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dnixwrbw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ztnpafxk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ltwegohb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3aaubmlnm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gdecqgnn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orlfdasg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3obanfnkk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bvgcrkee.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mwwzsjfn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nbswlvlr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dfjefdpu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uezuceom.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nwurbrvk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3olvrxvxb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zqhpemid.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ajjccard.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sartafeu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3alrthhvn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tpjiyvkj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bgiaxswd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3susrwqjh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3lvlewgek.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zcfcpage.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vvykamvv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dwrfnnxz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ycejxbsn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ltlhbfij.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3spxzeetw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cxjgifdh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dsjhjjax.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jwejkqpq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hksacfzg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3loonebmh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3adqzosvx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nsqbbwno.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zmknvlde.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bjfwfdur.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzaxqkbu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3haidppay.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3aecbpjkl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lhiozhlh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3exckblhy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pslwvpco.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3knlgdbav.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsktmodx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fhhjrtqk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xuenuekf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kjuclkkg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsscqjfu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3loiqyhnb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgabcnf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lirqbsue.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3apvefniu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3pmmjawat.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hpuuvjkj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mwnzqlnw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kczqnktr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3znheltpx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zfinbjox.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3whyadzft.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fqirvcmu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3uunmihcf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tulpusfz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3iftbydrg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3trttugmw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hbcbxrjm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cmvpwlzg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3nlasvjop.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tyefcsso.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xaihacra.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ewspmywx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3llvmzttb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ylminjfd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wxweawiw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xvyetbfs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gpqyimhn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3utrqcgtk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ejbzhjhv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rggnsjdf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ojyzblzh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ildtafes.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yumezwwx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ygstjfnl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzigjzef.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bwpijftp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3oznbljij.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3omxlnxwi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3sfytegcq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pcfjiacj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3odudbhet.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sbsughhs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vmudmoyg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxkotoee.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrqkatuj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kqalhqgm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3svrzavza.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gmbtblwq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fxjenwaz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wfumktbs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nciazzfu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hospxlql.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zoqaeclx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3putlzsrd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zqhlaqid.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mxtrhvzr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nerdhvms.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3sdyzfbzr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qchaeybv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3laxyrwii.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mmwfacmg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3picweuzg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dugvqtcx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3inuquxat.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3leuhznzh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ywfiojwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olthoqpd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sizwqgzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwryetlb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eeelgbkq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3iszcklna.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3grptsvim.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cgcaywda.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jrbocgwi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lhvxvobq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wntltamp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qgpvyabp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ntoobjsr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yrtntwbs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3arznbtnz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3raxfnxvj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rgnoctmq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zqfpxcoa.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3kcfjsjsp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3llpdudbw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3empeqgck.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ptqrxoze.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dvdbdugu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zwxnsfpl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xxkcgnul.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lmbqepll.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3govfxypg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wsdthwep.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nbzsmupl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mesfwbmk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pkbxlbae.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vmkxsilb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vsoaivcg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdouaral.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3dnhloode.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xsllsugx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3clxvsnaf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3cvosnfqb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zgquxpwx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nbkfkvfz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tzvbgxwc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fniorduf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hwiffljc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lgmkraym.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ajctyitq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tnuimovs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jmmghtho.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ipczicoe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zwbmrwmf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yojhapzs.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nkoupnzr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nobckgrj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ftfleonv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qdeponyx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3deoehtxi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eukhjlpw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pgthynbg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dxmsssqe.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vetnmpwp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3pmeexutk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ldzymjpw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yaenqtyq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qczwvxxb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3exqoarzy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ddomnvkp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3otswsqxx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ojetwipd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tvdsqlge.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3avfptxpm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3feqnfmfw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3yastvzus.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qgdsfrci.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rmwzmhyh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jmfdyskm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qzypomhl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zcdyneqy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3sibgkuur.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vibyrowk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3aaicyypn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lxxtspjb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rffvozzh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3lnrfmgmm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uqdduwdz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jgbcvgga.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tslxdjdg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kvaukhty.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nlhksgky.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kslwkvsf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vvjbkzyd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tdkkfjkr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jzdulgkd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gjrhpmdg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kxpmnqbz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ryykdeci.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3plosxxkr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ichrmlge.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iogoyxlj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3aeeozics.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fmspnspc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hrmhbehs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtrvlldy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zkupmemb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3roqivumq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hoprhhuc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3knwotvml.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gywpeefm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yusdvrhl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hrbickrz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gwixxzph.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eoztchqw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoafrwfz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fiaysxli.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ybqbitnf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fykwgdmw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ixkdibdu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sglrgpag.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zuafgddm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mqhnyyfh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3inlnfrow.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xhvntknx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ccfuolxc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pgbasxre.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ldfhjukg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mtmecerb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iwcuiqzd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3abxpnbmu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bekdzfng.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ukicprob.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zwfxjdro.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rlvnyarq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gdzvxsuy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uuaymxzd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3offdhhbg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gtbebbfc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fwcibsvl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nzvszzqn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wyhcpkfz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dqorxetd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3pdhzgugg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tzsztrdu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjslyrvl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ltjiuazj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kedllnxw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pxdsckph.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3eawvrtfj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3dxnrwgin.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qckwtyma.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3udcqxncm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uydwhxir.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wvioblqm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqtiftuh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dxwwrdag.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rqvszant.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kunoweam.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sfzoudoj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3tovjotdr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3tjdaomza.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3afhkzyiz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ixilmker.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lkbffbst.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xfffdomr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hpyfsdgb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wwjbgvhw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wlwkiepw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3frupeccq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qqkxbeye.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ohgxcptw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iahvntjn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rvixilrr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mrpumjku.html


<!-- 参考信息 -->