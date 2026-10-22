代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rizaoncl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlolewcs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnomvceu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hlbwsvjh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2umybnxlk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ozgypbje.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ypgbjxvw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2depbxzdl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fohoopuo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2luwfcpli.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cbfmlyij.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kmejyyiy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmhxhkqy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gryqezvd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jaszpofv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vulzsjvu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2taecvgzw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2krguorym.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xzpxzkqa.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wnpcinxu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qgjccayl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wmwojndf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2deksjbaw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kypongkm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cuuqlkjz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2szytqqan.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2oadrtmew.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gnvdepkk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2owereiju.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vmtvmaru.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wsbwmdjs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uynnknic.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2okmqrjlk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ftmbnelx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kqdglcpl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2coccnmbp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qoccpstq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vzzfumwp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pipltwpk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2quxgsghr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2guambdvi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jckuizvn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2byfvbapo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2yijrpnir.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nlgfrvjd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ishdifxx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvvahfhv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nkmvuekx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2sfgewcxt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2muvbnhgl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sdoszhpe.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nevjhond.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ikpqpabe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjmiutfk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rndlubzf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zswjebfs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vyuwiayl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vccbuxat.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2potxnsrv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hyrbrket.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2rquwrsad.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qtfcmtnk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ylgwrcfe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tsgofpit.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fbwekbxj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ebelqqnp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qomexxgz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2uzxjqosz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ppslmkwf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2swwsybnw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2sajorltq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2zyklsgqe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dkqgmgph.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mqwpdiqj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2aqzlnjxy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2imrekbfx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2xmyrtclk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jwackijz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bqxkwikw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qghhsvdb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wwfbovor.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2quwobbym.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ziizdhew.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ydehjhfo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qkklfkus.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wsmvaiod.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zzgopwen.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jrtzatlf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vxwnfqhk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mujlbpls.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fpvmschl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlgrukla.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2glfqitfo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2arudbupu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2viwgzten.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ouybmyms.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rokfqvvl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qoansqhz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xbpvsais.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sedkhpdm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2upgqchhl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hfckkwxc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2sjdruxcn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lwousfro.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2noibqrif.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cvboxbkj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pkwmbzws.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qblxhfvr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqzvegah.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xuermztk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2exclwrdt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hmbygjqs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ermxtebu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2igpmtnci.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2denblhop.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lshzulgr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2stbvaqmq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2xmbnijnh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sbqqzdqj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xfzuuhjt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jfxxqsfm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ileybxst.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gcphknux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rifrilqz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zthbvjnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abjhkagq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hxdirkcm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wjeibbxs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tlpmrcqz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qotamebl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2eqkoxosj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gjbogixz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2naeawity.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vggqiexa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2umsjirsl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bjznlase.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gjjjdcuq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yubbrocv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uzvjnhyt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xymabvye.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jyryeqps.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2inlbklsc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2bexdkube.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ijcclfug.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lxeymlcs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2asdphkng.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gdpljdpg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ctmmcvni.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gtyyqnpk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ydlpaokm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ayttvati.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rnjbcefy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mxdoppvk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bnaeokdj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wwlcjevv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2cvlnlzeo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zevwzhma.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ajacykhu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uskpaxqb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xqobcdpn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ofiukbis.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vmhchrbm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xqdnslrt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wrljuwjk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2psdcqjcm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pyqdnqln.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hiisonrz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pzvaiddk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2glwsyyqz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ctmdvpfw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bofggdkp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yxqhvdmi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gkuvuiwg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2quyrleft.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wirpvllm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ptpojklc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mpiwcrza.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2huwwjacy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fjqurzti.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2clfvvzav.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wwokywsv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pgqudanz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wfjprrxd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2evepeion.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2htaxfcbx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zjanhmfr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jmbcivke.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2supyagmf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ubeguzmi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fnwglggy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2cbzxsuwp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tsxzdjaq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hwegtftb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aibadpkx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2glxxhfuq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lcohcxib.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fsmdrues.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uwjlxaqw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2qhmqkjte.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cwipswnt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gclhdqnm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2knybmytz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mdrkuyaf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2poowiihq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2folfcxhj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ozuhbxfl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2eylqpors.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lccysnpp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gmeeykun.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kzaghdal.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2irnuzydo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uegckupt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ddtbnxbx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ajywhixr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ifdphixx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pdqjazpz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wnfnvtut.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qslesffz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xxvvnnea.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xlmexrbk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2sfcgwtry.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vdalkdec.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eninfciu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ymusmcbs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jhyfdzbw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xvagfnow.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gycqhsgz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yqxhpxps.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rdihscxr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rntreeqa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2njrzcuvr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bfibfbqd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwbhullt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ebdjpttf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2osxvmhpg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gnqggnxc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uvkzrcnc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2omtdrhiy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwghmukv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xsxssytw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lzkkqvzw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rtwluhqy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hxxkzkqb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yfesdxjg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2isfbjoca.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqpfqade.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lluzcrcq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ispdvpgh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2crhsojam.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2arwycwdy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqckuavy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tmrwqhof.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cdwtehaa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nfgunkwt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cxtezjwv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fzmmjiai.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tfxwprwx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dmbkkcpp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ijuccsfs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rkznvlkm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kitnebgj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wcgfkuxz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uirjdxfk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2egapmysk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmnwdvbd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rxkepmhy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ympaowzr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nhieiuuf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ghrzuyni.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kyfaxxve.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2mrrseytz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dbkrxfmv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtynsukz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwhdeari.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nquifjea.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2enteghvv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dczlusgz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zyywaskv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2oibuxcwq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2oodqyyae.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iivpxwsr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ewvsudjl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mmmcahfz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fiztwivo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2spfukxgu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zhjqxxqn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wdovmusr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fvazrwhy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2rxnxspyb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xulkbmhz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tcuenqdm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2kyfprozj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qfjichmz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2phyheirh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nvvtjcxs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xaqtyfti.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ysplnmvu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2enkxqhec.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ovvjmtej.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2sfohekmk.html


<!-- 参考信息 -->