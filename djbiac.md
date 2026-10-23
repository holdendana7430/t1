代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ehsejrqf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fsxzfuwe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fzuyetjf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zxgoqfil.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bzavrkbs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qauvsbkh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3iiuzojvm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlfrcjwv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kzgorucg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3whwtwfei.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3btebolbv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ttwdcwqr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3picjbkqf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ojdbomhg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3yctbzsfi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3penvtxgg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmlpuhur.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qsxzihum.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jfqicqze.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rhtqmjcs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lgwwnicc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oxfaczhg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3navvecbf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3davfrwxq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hqstzycr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nyxizoou.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qqjtzqfd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ojpbuecm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ykqolqku.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3distkloz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hrrucanm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3wefxmjtc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mpivwqna.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3aeajcsst.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qjaxigms.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nwzqivks.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3omnnspgv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3croghaja.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oohigeid.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3aqsrkyzn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mkkqnujg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3uuukeetb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3atstzuvu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iiusikpn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nkfhhksl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jqlcuqeb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hzbproia.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zqpemdru.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3blgbvwxe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bxuhrycc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xrfknhnu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lxeerjlt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkhonspn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwjzpyrc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3knrvmeca.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pssbkkiw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hvexsefe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kotrozxi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3djqteumz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lfvowmcs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3omnuuxev.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwdjmtjb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3trfeqcsl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jstnibne.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcqlnuai.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3asspajap.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3akqnocnx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bngkvlwl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dmykqpgn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uqbsbyyh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cbhobbga.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mhyodbxv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zhghqauf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pwcaelsz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qdspnckp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vsmxqjub.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3paokcxcy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3oydujzkr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3knbvnxfe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3motwcrms.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wuoadevf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3qivcubcn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3imqboqvp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ljqscbjj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bugxhfgb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gkffeqli.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3fenygzby.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3czhpkrht.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3walawcla.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ywacfxbg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rxlhlqpu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3bptegujy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qlgjogqr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3woltsywh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahgvable.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zfemshid.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jtfdwbhv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sgyjvinv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tcpimojn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygwvsmvd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfwgquct.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wgzjixfa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pnmjprwk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3iaavjatv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3selnyqhd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nndctzru.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wknooypz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3icyrkhgp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhaoicnk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljtmkaor.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lrvtdmog.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zzspahiz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nfhvgnwu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xhpjuifb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yxtcslri.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rtyspyap.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fqzbaier.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkfzsyhd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nydegobi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3unnjhmkb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3irmnprjd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ovbcgmim.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3cbvuslpd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qjpznrbp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mtbbzykj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3cqbpsnow.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wvhonjxs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpzkragm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xioiowjw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cjwgehvq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3witdhjpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzkxjnmf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qimvpkyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yideslvs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kfhmkmyd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yvutymzs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xbxkmvev.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xgdhkjrz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3houqqlto.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fvjkafab.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3khhomanf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3scimfsjz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ukdgyyax.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3sjnwbsex.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3krbqhkfl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qmkkwrbl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bfmwqvnn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3giarvsrc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3iuyzeavw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cpjxizkh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qtngruqo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fhiyspsn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lrdobscc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vfkuvzrx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kjmkzeyb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3sdcdcrvc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cxxrldgw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wpsfehur.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nifwrghi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mxsftezg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wfkuztik.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ywnbaezb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3iybknwaa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vbfimucy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lgmoeepd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3exadidbz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3uzexwyww.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ltfvkski.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3erbdndpv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ddqlzidx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ugtrxrcd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lqtbvpfj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3olcgorlt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bixinzek.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ddoxknly.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zvlkhesn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zzlqihhs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nnzqektl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xwnrdszh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dcqqdswo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmgdndhq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dazzlpwg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ufrsxqkq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vyddpudp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kcdyabeo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fyuqkdzq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3prrxkezb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xcmwpiid.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3yvvotuwe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jxzsdnhx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xqkyunym.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cvjimnei.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kxfmzikz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jkaooyce.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cpvnmqeq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ijndzjxx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fbouhuzc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tbidlfml.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nhrsjrag.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ggpbkcge.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qewtjiqb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ceewhevt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gwcwiohe.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3cezcotli.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3psyhwvnw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hdtbbsfg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3aoidiyoy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ddvaycsv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihlnvpvh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3opmolwji.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3quuomtgf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wzncpxds.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3imkpbsdz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mmhzfaop.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zjcpxjww.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rcdpmzov.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rlfvicvu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oodwqpyn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wdoowfpx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hgiwgvay.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rdawbezr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hwpklpeu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rhiiamzw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kzgochvv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3styvhjny.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lzamfqni.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rlgthuct.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bdamvcnv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ielqmyhz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3itowxyzm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yghcmugp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uwhmalou.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3aakedbcc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3khgmhlmu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mxatnpew.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tikmhwzq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zlmyzgsp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ueeytibc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xpiuneck.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3csopukhv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3cebpidtu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3matsjbvh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tnsxteoj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3sxmbqcen.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kbxovuwv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qoqpyolb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lgihigyn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tuaxjfin.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bgtfpybz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gsjbeoms.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tuzhjjfg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pspyqzle.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mozfyzei.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ekxqhuhp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vxtgujqg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vbptmoar.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cnejzvjy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qnhdbeyl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vwyezbqj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qgwsfmkb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mvkgkzcx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xkdcizmg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dzddcshg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gpahnqsy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3psymtsbn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3elstiama.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xxiewhvd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3uajrejwx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3epiayvus.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3dzhpkkgs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xylpkllw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3typamyfq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xuocwqwa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ourmljnk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3iseplhle.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ftxxisxf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ghrzrmmh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nhdnbpxk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3niiefkzq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3epyqoaff.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhbdgkrn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwuwgnt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nchzmzbl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rzgvzeob.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ziraonvy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nlmmtuqx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hcefkmas.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qtesvoqh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3uqcbbwlq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cxslpvju.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vdvicain.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vkreepot.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ktefhvcv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qmrryeyc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ticewtdt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ehkjxexu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tpzwmpkz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xsvdrdry.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vngcgukn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ukxffgty.html


<!-- 参考信息 -->