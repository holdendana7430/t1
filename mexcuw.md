代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuhjznjp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xgzdfztg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2roduwcpd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hcuznxee.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zqzxbagf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2uqbuzuvg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jgjbrkxv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nmwfwbti.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdmerfqp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2yjgqyphz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yrjbwpvj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ixfjexyb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yatfpqjd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2iqxjbtqg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ysymguip.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqgqjbns.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvyadrri.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lkqpmtbe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tnqgwapv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jsqerblq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2bnlmbsxt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vgpaimfj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jwvtkjcb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ybvlfpuc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2aqxvopni.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiionxlf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wepzexfv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2myeydnwj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ckohjirs.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfbsvcgu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gbyifwue.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2joeoryls.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xfppjvxj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gckduvpa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2foykrgvf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zqfylmkf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vekdhclk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nicxhrcx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2feoqeitm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lowiudno.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ahyvgaan.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2btuvbkiu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2znnbjufo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2awxgbhap.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2idfywklg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cryyzwem.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2caqvxwbi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xqgigqyn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rwahwqmz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lpcacvfh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2elvyhyav.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ffvoiznn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2phsuyido.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yqrsmxda.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tifqptyk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hyiqdttv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2oeywwehy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ssgyrccc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ptopozuw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2setghaml.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqustsvy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptbxpcap.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyzgzkqy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ddsyizlb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cwxjsvwn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2eyvphvmz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dhzuavoo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2yooujgbp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hvtwjrmr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ccwqgvhr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hjyasaak.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bhpguofm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdhzyjbw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2pelxzebm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2omefqicm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2elhomqpc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kagtwuxh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2owonufvl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bweyjrbf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xkfdtmlw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2smurkbot.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nyiirraj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2taocvlbi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ukcpnyjd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gygfwuld.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fnstwisi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bgydvnjj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2vmoafkjp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wdioxnno.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2opirhdjj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lhgmbkub.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zwftunez.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gyrxcvez.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ykewidsk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ljvtzavn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vvezuzwe.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zrrfcyhd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gikeehin.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wshznafe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zgkkstgm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2hvbcstyt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2elboeehb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rwauxxao.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2axvfaxpl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hrwsdcuw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cdinlknr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ilsqteyq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhequwwg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjzgpzlw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2tpirxotm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lzszntso.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2byvbfraf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nfnltrzi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pwrkokdm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vzmdbpku.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wntlsubi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2abxkahyw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrdrpmoi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mhyilcvd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tizjblaz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ihbppeiv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2eexbekmm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zmqgklno.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2vuptsmgx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ymgkdfnt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dvuziaau.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jsqcpskm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uwgbarmg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2usiledcs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lctfxgdt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tnxsnbgg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cafmxbxj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2adxpgbep.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2afcmuddr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2teldyohi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orimemmw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vmfhejsc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmvclxhx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hwcumkdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjgcbvih.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tayjxaqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iohchxje.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fjbsboif.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2weypcbdy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kjixtege.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jisjklgd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2woqpdnyu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lponqhlb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bstqnssq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wuqncqmx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2odfullma.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2eklvehnk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wkmxdozu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xdrrifwq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2potvnlwy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2afvfkaxx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gspwaohm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2monjbwvw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yogygsug.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2sgyldshc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2aehwprly.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mqoqrqqd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gexmvffu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qxzpsufa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2onhiqffn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ehravwab.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kmeoxzwu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2onhovwhs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2aswitvwd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2tgxhsoyq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqfzfdal.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hotqiwkw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qmeccbnh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pnmhyezt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwrvxoyu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bvwcwvww.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2knhiflbb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2datneumu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wiipiwgk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zasqpymr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2muzzsqzf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gzmpqsrt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2htukxzlh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jrgqwgdw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xjepgxme.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2baprrtzl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lursribt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dcxmuina.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nffasydk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2viuhsapb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ujezmqqg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zgxddarw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zklkapnr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2newxxgaw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zugmjlla.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ctznpbtn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qvkeious.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xwuduqhn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cozlgaht.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vnoatzex.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lnqourok.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ynirqcpo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jhtxosmf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wtyxzbuk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gokmptdt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2exnelhbf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfwfuuji.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hinqpxbi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tzgoeifh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jluierkn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rfpwdfev.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mywzwrnz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xuchvgge.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fpouabeo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wapqrrdp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2scwoezxn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fzaxtsni.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2imlxgmxo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dyacmkbi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2famkauhp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rluudeny.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gcydlyrj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2flyoecfq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ldtaeqwv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gyfpiiui.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2knjwrtdg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rgcssgsz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mhxifmkh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ofmcxiby.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vpjmlmmr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dgkyrsba.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2prrcntjw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2sjdottpk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kmutlmdo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kyorcxvs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ybwhxgux.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wfthlajw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jfrsopip.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mijegqpr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2paqyrhqn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lvkmvjim.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pdpepblv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jfujhvbu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dpfuxupg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsqcsqxr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sspvdhxz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2sbfzrndq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgplzxqj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2oermgdpu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2conarglg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2dgilcell.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2djewxufh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2eecykzwi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jnaeiyao.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2refzddfu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sovwvdmu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2nkkufvmg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lygttoni.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dsqoggfe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2awkjfepd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nzfjjydo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cltafvbq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bylgwsmu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sntwczrt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2akjvlwgp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bwrztpkg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2joodavqz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jnpabcld.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vphqgwkf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ydvmgtot.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yoivcxfx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qybgfcet.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gxpqqqye.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jqnxbsvr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2sglljide.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2eyodcmua.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ozlsxnjm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cllovjfx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owqleoib.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rekqkqkv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2amufxuok.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2niqixywd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rpssgxxy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2iosblyob.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ryifqvyp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2crjwjcba.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pthtuqyv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2myhzxopv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2merjmgmu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fpqsqant.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fxdudwlh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sbvhgkxq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2objfigpq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2yqilcqws.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zzjpmzpj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xppqidrh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qxieqybr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dnfamwwr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nbltklqq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gddtfjsx.html


<!-- 参考信息 -->