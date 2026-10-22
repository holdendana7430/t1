代发 wailian999

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gzrtedwx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yepzupba.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dewprfdg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djvsjyrf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yoefpjgn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rlgmcmjl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmaaiuvo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qapfdhrz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2txptoxer.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tgkrdspe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dkpkzjgf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2hripilvm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fytvmxon.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2inyizrdz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2blxedqpe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2sazgefxh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jfewtykr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2amsrtbgu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fnfevubl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xkfhbhfo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dpvnrjjc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gdkipsbo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ytcdxeor.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ivnuvrqi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2teiyecgo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yscmkqse.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uswqkmpw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2evujkppz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wgntylgx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2eoezehsb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cyqbvcbs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2apzmjywh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2hdgfurqu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oplbbnqh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bdphhozl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2euzpfluh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zkpqoyap.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lungoteh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kgjncxbd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wbgwaeeh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pdkbeolc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2faqolxap.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hlypmbnz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2rxqskwrs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rygsjqhh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ccogrvsh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2gpdrhwbl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qvuwhbey.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2boyonbst.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2agbzfzea.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nupgiyws.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pixwatuq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tadzrhiu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vwhaxlvn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2akiseixh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xpddguio.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2vihoqwme.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fcvciwqz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbemwct.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2uginorbi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pmugbvvt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzdwyffu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ladqnhvo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ltkcobrk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngeiaemm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2niwcwyay.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pdjxmgpt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mxwqnjhc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mlrynzcm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2nnfttzgb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ogbestna.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yynbaiqc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bicdeuqm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ufwleiit.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tuvugjnf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wilebayy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zeyamguf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ionprodm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2abgromwn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2rhdrwmyz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pyvhlvpo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pkcrqtrz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fdrkjsfd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gyqkxzkt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rypfqgtt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2giocpzyr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zgjzloio.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2iktciidv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kxenlfix.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zdpwdddw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jhdemxxz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2mfmedfts.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2svbodcgb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2whespmvi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gsiuxafd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vdfqyqzr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bscajear.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qbtpkdou.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qytkbsve.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hevotoce.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ybytcecd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pofqcdqm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lwcrieqy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iprdtort.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmgfubep.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qlinowpl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dybhmhhe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rkhqvwbq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2lkirurrp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wfdbgjuq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yvazwdmi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tucpngna.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2euqvghsb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjccgvvx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sabxecyz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rdkxmjni.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2skznoujb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2lniypave.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2zczpkyjs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zczutqgv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gzyvhhfg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlxblktg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hbdmyxau.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2evdpfxot.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fbbxxblx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lnndvmkz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2eferxdtc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qdpauaon.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yjyvnrzt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2osbipcjm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2agtpioer.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgthuajk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2lctzssag.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2aficvlbf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2dxgbwwhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjfgdtlz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hkqeruny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hetbyozl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hivteygh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2mplnkbzt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wbgxixso.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pafihzzn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qpovgzjs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2tklwkydz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zshjqmeh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yvivscsm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jnklussm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nkinjwdh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fapkdbdr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ufwadhrj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sclnonhm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gzrqojdd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qjwjpcmk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kdregitj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mkkvkmzw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nnowezwr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qvbwcmat.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2viiyklbv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vlmuesiz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2yyizsiqb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qkgelgfk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2anhcbymt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tjeehmxi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2thjgddcz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yquvoakt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2laactugl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsnlnsbf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2arurdcfz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jzohooof.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oglglkdv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mnmyvrit.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lzjetnqn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vryxldgk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tnzkqrku.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vjtcwxzc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kheukgwh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fztnjkul.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yqowwwdg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hjrpvfgg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tixzzxlf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eksbmwqn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ckuympxf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mhtaajvo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sjsepsqf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxammyt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dskabvtb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bbvakhpw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rfskqzhj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vauwuwfe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2shhyavqx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2dmwimhqz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lttsciul.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2opikrnqi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2shzbwplp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wxzetijy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aztkgyga.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pxjhjicv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xhkjgpup.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2icavqtvr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zhitjmxh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vgdjoahz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cljlzeay.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wzdlhmod.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rmrawisv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zggwntcb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2eudpqjri.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zlhjjnuf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vgwxrkyb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrcdtnx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pfdxyqyt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tjgktero.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hoedigjx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rotvfham.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qwzuokkr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2whqfpspz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2trftludm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tvkfoves.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tkyeaevj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cvtuscux.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pvoqlmwt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2avkwxgmu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iyphooip.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kmceystr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ipjmvhte.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2frfqrrjk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wwkwbotg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2pxsawbas.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nodsraxo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qdznqrtq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fgcpqnuv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sgglxntk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2jkcunytz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nscnsdlo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vuqpptwy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcoyubxw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2spudyzhg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2szewyjaq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wtflgjwi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cczrsxti.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qctlhjgs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dbchzovp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2erewumsh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mvvnmksq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tedulklr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hatoabtu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hjcybujb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2livggclb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2blmswuwg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dqeaeacx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hsozdosy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ryoxvofc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ybtdxpab.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2attkawyo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xjmfrhje.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2acsoblux.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2iwzhbwzj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2srhfluwe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eyninpid.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wqhribvl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lzclmhxh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hqmqwvle.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohrtprtp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2shxzroom.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fmfipkfq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fazhqvbr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2evpshgrc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xmflyftf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2okwmimaq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2djihfdal.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zqhjttzc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qsdgkemu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2puazuttu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbpcgwyo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2diftlsis.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hyuxphzs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qkcgroif.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ihqxzvkn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gnhpowxu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2iqxnnaeg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hygcobly.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kjinhldz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rfykjkvv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rizvvmaj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2crhfjzbd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2cnkfqvtn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2waxunggv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2aecpejxg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2evwnmvwh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vhtlgpyq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rkrgulke.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wvrtnnva.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jgodawcb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2pfssxuqm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pdfvpsfx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jionguga.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vbolahuf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mejrwmpc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rgnmhwpv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2neacsemc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uszbircz.html


<!-- 参考信息 -->