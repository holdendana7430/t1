代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ekpwoxnv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jplpfaby.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pearbhsz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zktpphod.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zgqomuev.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2sixzqmvy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qybjqxvp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cfyyelra.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tqfttwlu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uiqglpay.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2uqfwdnxc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2utmjixfu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lagcuwwg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqfqssec.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dlnvmomx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2yakpkrzo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2stcjisbu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2reeckjxx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bldqtvhx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2loixeyju.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bhkwwaxf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhfczgxk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2rjfftluf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2atewzmzk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mbyajoyd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2prullbli.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvhxfqwe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2qnijacnv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ujnuqyvu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vywyzyck.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vutfclad.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xzlnvpzb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qmsxsjbl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2feytcqro.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rkwjzrqb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jeyjeoju.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2uvmrmics.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2mogarjkr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yusnxfod.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2chflwhao.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2laegfcmf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iofmofrz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zkaeetnw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zipbbifq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vmfkuzwj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ezaeqgad.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dcsuirzj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oswvqcbu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zbupurzt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xelwymtu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2phwlmrtr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2uvctfguw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zakdzhts.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vqiimwgv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wmequxsa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ovvtkzrk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2golxrpzn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzaxdauj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zobsvvey.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vcrtebri.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmcknpu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gbchasse.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qxrfsjsy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vahlbzzr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ogymfhkf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2sowwremr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2anssbxmk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2llwijdwl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mygjguay.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dcreygow.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jwceyazk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lbktwzkt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2afyvtber.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bdvsufms.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nppvtnux.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qchzbswp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tsktgkly.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wsupzxrx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2apofuwcf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rbmizsrv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pizlcikb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2uhxoqidj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2uvoyzdku.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jkacdfua.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vfbxuqfw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vkmfncoi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bejpmjzr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2labnzlle.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2vktwsfuc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wkyxriqe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lcjvpoxr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jhrursjs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lcdmtozg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hcmouceh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fszvdzrm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2pejoujjl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tjnetiet.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2etqlvcgl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vwapkfmq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qjxbdmpd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aevctiwh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mqjixvnk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2adycvudr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lusebvft.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjjbaonu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2oiqpzhni.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wcixvwwc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2eeceikmj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2euwqaxbf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vbmnzqcw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2awlscerm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hwarklwk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmbcknyu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgkqlees.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2tneabjoe.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gdvceawc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jsjvdxvu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2nyfrugqo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xcvngltr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ojmgmbex.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmrhsjqj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2heeweeha.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2txxnixty.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2psbcjulu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2uxcwnwav.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xolwpvaa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mbjxfmhi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2htbcbxmy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gzmrhqlq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vmowzdxo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ofmttlgj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ihbmjpix.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cinfenec.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tkxokkqj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncwhyodw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cycbejez.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kingyife.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpojclki.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uimjbtlf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xyueuthy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lsegkojw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zfzgefsc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2flsswvrb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2eiazrzol.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mpndsajo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2odhacvjh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2muxohxfw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2flwgfvys.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2vmpwnvsz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2thhlokou.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yplolsqw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mrrxzipk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cfrxpkmu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2olfsmhle.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmbbijt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2sbpdgwlw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ugltdqrk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zyxytvmk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cdbokwzz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hfdyhfvy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2anrbichf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2opsghkex.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2njnjspzf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fubogtrj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dffxxhdy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qvnxbatn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tehqhbpt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2luizprdr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2oxzakiua.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jrjxzhxj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xnqquesg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2cxmnlikg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzcdahp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ahexjjch.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ryvrhtom.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kqsoqfhy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2smfpfcld.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2takazbqa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xyxnlngz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ezrjqgmh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oxuulfyi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jbosucbk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ihfwxgza.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ofgvlltx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gzlbnqgi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eweyvzox.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uafnklfq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2liepskvv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2sybgkdaa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukoocxra.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rgdagkwa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xlhbspqg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jwoovakf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xeliyvjc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vbvdpjil.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bshqxbhz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2paiemvwd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xvfdnghw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nmnquymv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dhhvatvg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wihhhqqi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kgovpztf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ghqromfc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ayxeemap.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xnorlcie.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rdapmzrr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tdwsrqrp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wkaordzz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hhogqbvy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kolqldly.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rjsnqnuv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cvooqiwf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2eqtrizxx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ahhnilcf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2godbhwbx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ayodjwfp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xpmhyzpa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lrfxrxkd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lvtospza.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qcfuucnf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mkvrbhwf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mmnawpwr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tybwmvry.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rabxmegk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fycslors.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bhsyzmqf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qedghjmm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2powgicda.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2kuxqtvvk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gxathubi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cvgusswq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2oyekjvoa.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hkjbmsmy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2noepdglt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yjoghgph.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qchidicf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xgzmzpxu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tiocwyop.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rqsidtka.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uscwvayz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mimpdrpz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mlpoedac.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ubcjbsud.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcthrnmi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijkgkvlp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rhovrmhq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2doazauwe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pbncivqo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vorulswz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ctlkmpni.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2izrdqhag.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ndhnclba.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ukvebuny.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ehcymqec.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zlscoqhv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rltxttqf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dcmelroa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ljiauhyg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jnyyoxag.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jxskntgf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zgsggtee.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2akbdpspq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mhgtdeyz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2skijrepp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2edkjozeh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fnzddlat.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2boxobedp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2inbpfxhf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wuntooct.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2bmzdlnrk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2iegmogrc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nasubewt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oovqfsht.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kktceawo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zzqvkjjr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqgikblc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2guvxnwan.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nrfjtxpm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zejetqep.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jtzhiabc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2knlihflj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2saxsvzfs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ynuqnouh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qkojxkjh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2azagafwd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2huzbumqr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ghepshtj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wwfdycdl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wygyxptp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tycumdcf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2otlsnrce.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gotzmhgl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fggsvzgf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2muzxusht.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lqllhoxw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nihkdczs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qcwvbqjn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rjwmlsgl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zalxjtlr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vwazdmad.html


<!-- 参考信息 -->