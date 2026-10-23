代发 wailian999

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zmktddng.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bnudfars.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gxmeyfqs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wljtwiib.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axxamorx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gkikyrdu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ghzksogn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xconyqbl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3oohpquvu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mfktuqfs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bzoujoqs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ftuathzh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xgftfpei.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vqblkcll.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3pdtytodm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xhpsnisj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bxyaudqu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zasdjlnl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ttnzmmke.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3debrjtnc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3igplqgry.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbyurgsq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qeuznmic.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hzgcddnz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gltcuxum.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zespxrmi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hbchnxej.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gtuojqrx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ltlwbypt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3firdpizi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gytbgaah.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3edtbtiio.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3sfynmgod.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hsapehjl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3milviped.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sfwmoulx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hxxosyhx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vsdlcxaj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zlmtwzsn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3usybcrgg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dppmdkmu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gqkaftxd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ncktvolm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3huptmqlt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bwmvltcj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gygbzoma.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gcwhiedq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3btnjbzle.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cxflaltm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jmxhsurt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3uvnmbukh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3obeqwnew.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hputffio.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3qzpojiag.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zjxyoeeg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fetmhqay.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vafvmjph.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vycjopgv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zgpokyvr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vlrcwjwc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3quyceygg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3keswudwl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvuylgkg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ilcntqjh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnuwuayf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lskxcesj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3suxfquii.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3itsymbwm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3folndepc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lwigxcol.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jcyyyxuf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ececehxx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3inpygoqv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zmejzfcj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3govbpcxy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wsnytqrq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uvibyatk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hdtpyoka.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iovcbbyt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3utdvudqg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3unzlgpiz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xzhfgaja.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3oyafjbrb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3smtxizvy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jvxizozq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qxrbiqzl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3soqwkdbu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bhedsgtf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3exphakyv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ubzpadgb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3llgdjwcw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kooogasu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3njmupgir.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zlniwmef.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yoballpw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3casbtilk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3puexkraf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gvackipn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3oueovwcl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wzbzfafc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qfgakqtj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ifdkzqcw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bentkxeq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3psjrsotr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hvwntyhk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nguvzzqa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3axpkltcn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3foxczbcm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixnjoxhh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gayurhhu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fkljstau.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wxwgwhph.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfinjeny.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjtzwevf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3seryrlxs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fzzacubm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kxvukutg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yovzbjxn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rzwtesjb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fzdgpubo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3olgelfsp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qalatfvy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rbrmzblc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dlkomtej.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qstjobgw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3feglexkv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qtmtwyam.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wjyfwuwi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3miauiqiy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3piwiqqjb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jkasayfs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spsfqodq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wokkngqa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3derlmzaa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gsjgfgmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vypsgjqo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mgxqxmsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbbbceqm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wcswoszk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ixbeasvy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sazueind.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nqtisekf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wcresyeh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kopmljwx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pyoqxpyi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cmofbgbd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zpptohbj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pcfjshml.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3iigbvloj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rjropljd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cgdcaiqd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ocfijhkt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3kreaypsj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zonhyraw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xidhnyrd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jkidvnmr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3tiiqoyqv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3molsfpli.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rauyugft.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hiugjcuq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3elibhlbj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fhobcxtb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ygtdfpzy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3akkfaykw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rgonwivw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3upkjiwlm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gurukjbl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rqwrtusd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ygruakno.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rseamrvn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3khjxyevk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3aaedtyyp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wschbtss.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vpdbgxpm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ifthxngj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tilprxzu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bpjatsyo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pxcdeyib.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3oppkvtni.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3umnzonkf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ednmckrm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eytdgkux.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sdtrlekm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lneiqfpf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vrhdkztt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3povscusl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ggcqafdx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nqnmduma.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bsgthydi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3irtnlfxh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3uknhdtab.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3auagrirm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wtkxnpkl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ukytwwff.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pdafrsfa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pybrfbnt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tnhwticg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zxeyzvtv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ekusbxwb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zbodtpqy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wdrokrwu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jssavfhm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oyigqmwm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3oreukahv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nnlgezaw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rrlraleb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yczryfmk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xwxhdpec.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rrfhgyzo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ykjqcyqa.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fqtniglw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sdaenpsp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sgkhwice.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qarfieni.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ainzqruv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3epysivjk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qggvxiei.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fqjjsalw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dlguvtxj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dkjkeagy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kiuklzmo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kntntqoz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zybeczbn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3reximyaw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ousobgcd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cbmigzqq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nkfgmqch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tbfnnnbf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kocsbfyx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qegtyrvb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3cecnakle.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lfblgrom.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fzgpxpnu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3agqyugsu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhkxytn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xlnqmigl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zchmyeno.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iviwpmhm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3pfrgcoxa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uagwpyja.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pfzpiqjf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hzkodtyj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3cpgqwxxi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oavaqqyh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qdcxccqy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3biaygbcv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3njswvkiv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rlferagy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3evkpazku.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vpsrtnlu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3upoalbxs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tgwtqhyy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gjhyzlus.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3vhfnwhcd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oetfvozn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tisbuggh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cmfdnnws.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjcswjvt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrmvlcxr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmspftoo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pyxwtfbi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qfekukzk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vuqpwine.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hnoynqto.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bvacmgad.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vlkfdlzx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ljcgeaze.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lqnephwx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bpmuxlwg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bjwhgqju.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fdavyolk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3rpvghxjr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rjfwaxop.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lklravdd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xezpohyy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jbrfevfg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lrhrcgif.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lelyasog.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vkjtvboq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gwjltrpg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qotimjzx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bjcknqiw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3umkfnfyt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xsadnkrm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hycnzknf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3uzqcdmln.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3txegmxxq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ysfzzkjp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tdqlftuo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3zefnfpka.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3chgcaesh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jupiihvp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3drscwhor.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hoojgtfv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3uxmbnscx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wzyzsorn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqvmijfa.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vxukglzo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pcarxouu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mohhvwzi.html


<!-- 参考信息 -->