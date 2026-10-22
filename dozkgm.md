代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kehsagqt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tfbccztp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qgslqrwd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xudpbjcn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouugsubd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ugbwqpsu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zafeuapg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2kaesudvm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kqiaqnrk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wstbbmgg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2eukjyusn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zzwicqsg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mmfwdzgc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dkzyohrx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kispkxxc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dmxxnpen.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2iculndwk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ozjnveal.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2cmuzudtz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2oajhioxg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sdhslavy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wmvsfytd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jggodbab.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2sihitzqg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpheycpe.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oxqjckuj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iwjvynes.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2rsqbbjrf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zzytgteb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wbgwgwwz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ghybkwit.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dqxbrzyb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2acjiwbop.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2unoeytyw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pyiyalaj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qkqdjhur.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jodbqwla.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2udkrkcor.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lqkkiena.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ewnzytfq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ssjwbqsm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2geqxcwlm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kemmqpcd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hyayrkpv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iznooztu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ytvqjlad.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ycezbmbt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ejawsqss.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hzrsgwze.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ocqnaqgz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oywcddwu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hvxvdxhv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qwfgeoua.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2lukmopxh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2egykwmcn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gjmaamho.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mdhxizmy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vskdeewl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qepezrck.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lpuczxjt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vcyizvsf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jbpdovhd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2acadgong.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2srnigrtd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2phydgaqb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mmgxjtvt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2iexoehyn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wodxfeeu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rmhdvjnk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cjquopbs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pxnwyzbs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2idpjtmbt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bfkkuorb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2baadrqvu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2amwfkxou.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mginjacp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2emzpvhhm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ubymoghd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lirqrllg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hzhfbduy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rmvawagi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2yzezrree.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ptmxpjgm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qfbrwlvq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2frmkypnt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kequnqlg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tlirifmz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2hisppuli.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2eegtwyvo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lzfdetkf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2gjwffllx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2imawvyee.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tptqxffy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zykayyfs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lbwvidbo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lnydgfvd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2opozpnry.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lgdpsfpu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hluycdlp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2wiyemfew.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ovxxzjwa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2erftroxh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2euhnyhai.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ckqtyycy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ijloedis.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2stzrmyyk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hofnqfhz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dalbjiir.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ofrdumvc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pjxlfruc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mjfmqhcp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2didxgsgq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2skdfwtpb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvuwrwsk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2iqxsdukc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uasjifhm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2exsmnqwo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ibdpxjxu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ejqfilhy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dvddzitr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jfcsfrlk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhuxediu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gvqnrxsk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2htbxlofy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2arjufyjd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cxtnrxao.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nrdhsfbl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dswrdjku.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ouagnirw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kvqgbupe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vflxwroa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vhnchdcy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ydorsgma.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xfmgwlvk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2bykeykuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhuxbzpr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2huxnqzyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcdcbkix.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nlhkozyt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hmryilna.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dsyrvsjn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ouvvdbjj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dajojesx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2abnchdxm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fgpdvobd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2amoctqfb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tsqthsnu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qnqhdtut.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2aqbreykc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kzestimv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hmqqihsv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fefzzrgg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wsixiphw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2isbdnauk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oenahplx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ivqqltbs.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2yatnhely.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vqhwbgae.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cqulhtxm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2giaapsad.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2prehycup.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ersitunz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2grnewkfk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jcthrqpg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wslotkiz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xlqvxrte.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dnsbjaed.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ivldfmla.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fribkrhe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kozyoqgw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2weiecilf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ormonngq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dnygwwgn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ekpkhyau.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2bextcmau.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hlqqbnja.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eaatjmbq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xppmziee.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2bgvybwsb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dkrnzmmg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jwjmqudv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qdhzxjfm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kopxqmeo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2aujqfxiq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2heyhkref.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bvktiwkz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zyftvnpx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2baimuykg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2cdcspoab.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxpuinp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2itnyrzni.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dkjdmbbb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dhgrodee.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lacgurvk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2upioemdk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mwnqlvev.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2msiueeiz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2npgiqjwu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2huqlgxez.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yeuudsgu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gfdlwpis.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fqzxaoum.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2apwxaahg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2auleshmi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xuhsiqrk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qvaigmxs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2emtoxlth.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ouxhjeuj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mokwwhja.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qjzkxomy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yrvlclwi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iprgufkx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqpxfjyw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rdafxwsm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lvyzvdnn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xjsthgyy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ronspemb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xgexildx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pmqxmwja.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jqqstths.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2spanpttz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nncmwedk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uqooxadr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bdiplpzy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bbcolrpt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tevsrwir.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bmvmnvgb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2lktbmmxc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2fkeyhnbe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2enfizldv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tbgqnpdf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fzuutekp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2symopbcb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eutdbjig.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfjknstk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ucdbpcsv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vklkcddt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nnjomyet.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2admwjaor.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bjraziww.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ebhvcfod.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxdfvtpc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hdrmhgmv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gzmsjptp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xagnnaxo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xswngwhf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pnimbhuv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qkdytaqa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rqmnszaw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tncfqumu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxjcclsz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2taohitmj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2avesmsvn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zkjhbvnp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2btzwlibe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eodzqeuf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cjlxyclg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iuiiheui.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cewogtvg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2awuittyr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2itqhyvkm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2oixpspec.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kfmiphmq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cicqiemm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2uxsuonto.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xdhfgtqf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2duqnmqky.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lkzvqwka.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2otqbknsv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pattpydn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jjbugsiz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kwqnuvtz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2khljfrml.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dfrvdbum.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihwdyjov.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrwzxpfj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2engbpuwv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tvoqgcco.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2yokndjtk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xuknfotl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2pmofexdw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yrubnoaq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xhsgpxpc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xgmccouv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlrnduwc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kwdzoata.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ggnseqnb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lxomgbhc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ixisclap.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2iuibjcie.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ojnhrtyu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ndssylyc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nrxthfhl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lpujxxyn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vuekbfxt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2auokkeji.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oopxghfl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uspwqkfo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bmllbopn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nwhgscta.html


<!-- 参考信息 -->