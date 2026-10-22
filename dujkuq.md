代发 wailian999

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rvibhfqn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lpapkrvl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2plpvsmqo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zamlrucp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzvwxfmy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tnygjoyl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ixoahhct.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lydjdcwr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rwpiuxud.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gtfcrblu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2pjlxswmx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijwgoqua.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yhtkrvju.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecckxyfo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2smydyeoh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2gqcdtwqn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfzxdbpb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cqdxxdil.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fdsepnil.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxjfvie.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pqnjwbsy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wsajtmzv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rvlbdlnz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2paqdtinh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qruffedt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eynourbp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfhesnfz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zhgmrwvg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ycqnhncb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zhrwlivv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kgcckshs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pqxojojd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bamxhafk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2avdkgizg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jgplxnhn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rsnuxpfj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2nllzwmfx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iurpyjwp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2sdklzgfy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2upkvfkot.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lrtosbmt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2dupwbgjm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hbyhsewo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wegjushk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2molmtctf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vvvvvauz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ndtzzkcj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnbisubc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qpbmbbjh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2sxowznaa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbbgmuuk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2odidleqq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wgwgxmrq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nnktqqif.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zhbksbwx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hvmpoepe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wnpulxkp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2siptshoq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvenurmb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xnwroogo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vpwyfggm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yqxdhebt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pjmyagab.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2amppmyfr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uiheaqzy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vpjmvtwz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ebzrabwg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kjudteqg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wuedclpt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kgafhktg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xtibihuz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xrrgvbxe.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xskstita.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2sscrjoax.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2avzrbmhk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2knizhyjc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2drmeienv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gxuijozq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tahifmsn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wicotbax.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pkmzkiim.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2mykikshx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2poaxzurs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2bxsjquwu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kfavomqc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2opavqnki.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2cdwpolwv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pyejuotw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2qguyriwe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ziquhuwk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dksnbnlk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vpnbucna.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2eugupztk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nhvnzwdy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yqzwsrvt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hdmulohf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rzmdcuvh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2otjnfxxk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptnrlbcv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ojbtypfj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2krlbezzc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nujkowvz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wzmonypd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jxczocip.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxkuwlax.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qmokmhev.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jadnctmj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2owjjlsoy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xopbgkew.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qcsbcmei.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2srrinpvc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2udzaiywj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wdgzgyak.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxwiktla.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lgblabfo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2opngzdvh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2yeewjxgs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mpisdgvc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lfoirvth.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zvvqyntr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppdnsnsv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2gupntagt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ojtjdbcj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hcgyzpxm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xchycoyp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2senqlten.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wdtmpzbi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ptrekyix.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qfcuetdd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ihkjygjg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tgssymaw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kbznftfr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zsnnfuxs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pmnedfhb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svlzhrgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tasaetbg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wdbnqasl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdwzasez.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2orbydxmf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2arreozji.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wzewdcxe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cnmrlvdn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jfeariok.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2wioqctgo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tyiurczk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jtoyzkuv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2priolpfp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zfkiofdi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mllvlytd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2gurqrdnt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tsvciwjn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qyhtxarj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2gzmtqgdn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uvtggbim.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tmnjombi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yjefslfq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zipjtrbi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kupbtamb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gejrpwrr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vqwfwxkt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2awraeyzy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cprkbxss.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ckdvjtra.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hebuwjki.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sodkcnoj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wqmvtlks.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ipmicomh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2nygdiqdx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2shoorsxl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zocmxgnj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uzjgifpr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zixcrzet.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fajdumto.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ytditgus.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2twjzisyx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vypdcnnp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tjndavij.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gdvrhruu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zgshpuuh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xcwinocd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vunuotxj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2airxfufd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jtbzeomg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kqjlfadt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nenrwdnr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vkqeziku.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2twyulola.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dvzmexhh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2saqophdh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ueigsqvm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2dqfzlsal.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2srgwlgmj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2siirfquv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pgwxqyyd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xnhldixb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2atpzfswb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pwdwfwrw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lvlncqza.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mzdnxctz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dlwwqxig.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2prcvxnlp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2drahakoz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tgsftfaq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bfkjgtvv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2upwkhksr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ijjsvrjb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iuosejuo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ihacmgcs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aaypojub.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kirbciki.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vdskkxtj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xtzizkdk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aupbbxup.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2slybtlsf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fmqjbghz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zhxsfybg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aovnbfen.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2oompttoy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2aderaiso.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2gwbmqteg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2beoxzreq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2imiummci.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzdmygg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yjyymvar.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zwxxoyxs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ufnqucrr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ygqznjfe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2iwnzwrhg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2uroogjdo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wzohutrq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lxfpcqis.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yvutozhj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2adnmwfep.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2obznjrqg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2alcmoxhm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kzpfpqfr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iozahozn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2omvcfplt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jkieztuu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cmttwojq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmahmppe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2flypotnk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ykyupptj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgwmxypt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gtncixsx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mryhiiyg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2welronbm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2iicssgkt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fdrcmlul.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lrrxcner.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2okhaygju.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2cyejekgg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jshbgifk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gnjhjeox.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tvlgqbgb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kgmcslfb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fxpxyqtz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vkqqvvga.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bnghtvvb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mpzatqel.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ydgbnnav.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ucgpqrap.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fhdopdrc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucrourod.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cwnsfktb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2eewzjwyc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ghmvdnjp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dkwuqsln.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gsytlfrd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2liajstzc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2nqjwgsbe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hccwtqkt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jolhwrku.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2pqxohbtk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vbpibufk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvrqxcgf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2weyffjsh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jiapfphn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2yrupdyhl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2syyokmjc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vjvuwnqc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gxolubal.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qtmtmrxv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukavyczi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kkawccxe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gqaqviwm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vqpscslq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2olwpcfoe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmkksjdk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zswnchjq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2sfuzhbmp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2oxxznogi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ymuhkggn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ecnpkmxi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tuhdqktb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2txfbwlmq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rgqkhuuj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hbfthbly.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ayndxyal.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2htojrzyl.html


<!-- 参考信息 -->