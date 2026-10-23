代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uohicozj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jbubzaod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqicdkgx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3blsldhzs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3tuodlhsd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yzbltgjx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoknjzpp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xbfslrcz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyvjkygh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yrysssye.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jvgzjwgv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gnjihpcb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aytdvrrb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wxgboahz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vraamjqa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nickzdhm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jyzeaefu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tuhidthu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wbgvgvte.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gmcfsnng.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3alwntvcf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3anznocru.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3phhmgtkf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3njuhkdxm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hujmvbul.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tvomsflg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3spjuhnrr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zwbgteom.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hmkvawch.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3vjbodapd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3cshrqygh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wiyujztp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3aavlkgtz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ehcrpabe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qohnhmzn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dectltie.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gyzrlpix.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmphrczh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vtytqbdo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3sczbynfx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ttvzaecu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uzywdquw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jhfwetkw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3luqczqpp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3gtptksdd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rnqzesol.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3sifjehyt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3wyuzllai.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mpmzoixj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3mfxxlygq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gnnpgfgi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fjjmahnx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qpeljezm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vyugnwxr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rfgadztr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cmwlmman.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wtgmoyfj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zcjecvsx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kzkhdhmz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lhgoceff.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rsmacxvv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rbfubmit.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3usshqqwu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hsgpbrco.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hiruchsc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jeiwxvyr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xckzdzum.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wbcgglnx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3czywhyxn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipltjygl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ybevolus.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vyaykhja.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yjivadoe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ybexinpj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tsgkemvi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3zurqeiok.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3spfnxodn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rerqawip.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bttqclvs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sibrhhnu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kqxpjptc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3rdavfjol.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ffmuwnqu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lstfucud.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hreaoyyx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ykofvbxl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vsbpomdo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kjpugeyq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xybtxfpc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cmcfaulp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mksothmk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jdwtfojt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kehtmofo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jiwmfxnw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vwffvhac.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3spyrwfey.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vcqznvnq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ktosyozy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3oaqzchpg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3imwfvkif.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qeihyzmc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wxvpigiu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3plckshpt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wydqsfqm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xswqeitw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3asqjmoau.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jzqwlgpo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xbqtbjhb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3aepfnveg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ifjflrsk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3mfhvrkuk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xjwptdya.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pzsfznlg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjllulqz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bcquuxnq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tagoevzk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvjojbtk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3grgglqlk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lbktyqbc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gquuwise.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3rxyxwipi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dmwwlnbd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kzjqtarw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vipgdthu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hghycpzp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckfzcqdq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kwxnqspp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jmnagbhq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lkuuwmgn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kxispalq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fuysjmnd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gdqkppmn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyawizru.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3odvzhwjk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dxvbsisj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qcwncetn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tjuytrgl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ujcbolvw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xtsidayn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rhabldwu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cccimqrp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3iirzthia.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3iqymnbyr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfjmjdll.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jhsueapm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dghqrsox.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptigedvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhtrfjnc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qzvdzecs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekhrypqz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xsatbxnp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3oinzbofx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lrlfxcet.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wicnuoza.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pmwtvdaa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vbibhrpe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3mbvcftln.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tdahnsia.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mtlxjywr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eosxjvrw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lfopwcej.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3coaktmgl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3guiywdws.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ptfgafqs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cbbbdaev.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bljslobs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vrqhkvgs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wczztvrs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rabidbzz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yiswqztu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kjbjzoex.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vvkhxaqi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jzeqrrcc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wlgblpml.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tdqggqmg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmpvdxat.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qabmtzlf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3iterycys.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pkhigzmc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hraygugw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3eeipblqc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3krufrmrx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wsmzblrl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tvctxzsi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lbyzapal.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bzpkibmw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dqxdvzzr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tseqonwp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rggfllms.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3drdplfcc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3znhpelwz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3dyetjicj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gflevclj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3usemhfki.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lrzreuog.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xvbjdqwz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3slqxyuhg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ftbnzwyi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bpqkaagj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vgyhjjxj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dciqigbb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdcjgexl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lvephqmi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hcrjmpkd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3diptohot.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vmtdreaq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ytbxlnhj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uxigdxsy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ksmhvjuw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3siuymkwm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3yeylpobs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ethkzdvm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3utvuyycu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tyhgggbm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lzptocfz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ustmljxl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mihomhrg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vjdnjbgu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qldqnpht.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bjpkslsh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ryemvduz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yblwofav.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wwqlzjdy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ldainpdd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hirdxtye.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3orpvrylq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pytzdsff.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3uurbrjch.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ufcbduhh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3olfennxh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ctwksyth.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rpbdzehu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3efshjtpy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pkpdhnhf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fijdaqwa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zysunvvf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vahytsez.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3dcquotff.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yzwwzxbq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qtyidvgw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3evkcqlao.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lbohlqdz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ezfcbudh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rujwmslh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lkjqhddo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3idzvodzh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3clgodiew.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ntzjztra.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zdcfgzla.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tmrfoqmr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3npaqyffe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cawtucis.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pjncsmok.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yeuwqsag.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3scmoqfuk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwlpitkk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iviooxnw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3oaszxsrq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cwmtkqrk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gfscprju.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3sianapic.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hxvwjvil.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nqnmbrnu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rrgmpown.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vvbzqcbf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3aylbwwsw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ktgfklbq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jwuourmw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jztfyzks.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rjfysreo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wvwmymhy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rgcztxtl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ckssyzhb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gjrvtopd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tnztnokq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rorooidb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ummyhbdn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ytkljvdh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jtfiefes.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3khysdzsq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kkvocscm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dcvoiznu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kgzeoaal.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yldzueyn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3drtqihmo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mbhgvikm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qiuppbav.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tspjtqyi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3exjmrzki.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jtantgwl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yiiipibk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bjepqvoh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vzzgoshd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3qqgdinoy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3glcpwixz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rzmxujse.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tzchxrby.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3invloyjq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dplcsqza.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ekvvtmov.html


<!-- 参考信息 -->