代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxpgtldu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2sajsspuu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2domgxbtr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ompjwxft.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2romxfyfa.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmqsnary.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ltsuisiy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjtvysph.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jzrggyzm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kmquwwam.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jeknzmss.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2szpuivhg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpebrnhc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xyfkqopa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ehvqfywk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tnotqufe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xksqaofc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2snmpvrms.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2sltydgav.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2oqiykmrv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jygmbals.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmrcznuw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2itcbyxsi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ydaraoxm.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yqnflimu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2uvhrpuug.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rrpnmevp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2aptgxiqi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2esptpbbh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zrwjqtgu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fecgcnrf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xrqnuosu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kfhwcdee.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pscdhmhs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2wasceasr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nazhbawg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gvhepepq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2enagwetl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ezgdlona.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2yfwprzuh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xlbxalik.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dhscctal.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rsxluern.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2apoyxfqo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2acsblown.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uccjhrqy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2prpooans.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ftxiaemp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2spvsyneg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2shgktjhe.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hcsxozld.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2cmlqgaav.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yapmbzkf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvxqgwie.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bbsslykz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nipluhex.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2quyeoyis.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2virlitvm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsjlzhac.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cmazyeej.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrcpcgo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cvaktswp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rdrakcfv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xggazicc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fwrjidea.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2osyplxle.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tqnscyvp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ijecncye.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fxsexhfy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ajqxagyz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jhicypqb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2cpirlugs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wbkofcgs.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bwoemnie.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2exmrdqas.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gqsydesb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jnfkqcyf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2wlrqtbjm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2aeicpgpp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2drqwxbry.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2irkrqnda.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2hcxbsiss.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2syafjvnq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2tnwrgqad.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vlsmzonn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pjhegzib.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kfvipqbh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dndrkqbd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dynrkkgx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qnrjpgoh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wzmkbgoa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ipvrumnj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ybdliyzj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2wbpasgke.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljafcxef.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2mjujecxu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zbksytdo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkpnpscq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pxqkohme.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgaxdvkk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jeizzswo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rddaohje.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bzwwirhu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bpjhmhzw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2eprcuvko.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gmbyhiqh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tankbvdq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qbcrcptq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nulparho.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2amzpvyox.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dgbzpgzw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fwhlrwbr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2szzqlplz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2shfisrdw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hnmfyied.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mbokphnh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ylgqlvap.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mitshwbh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kwlgxowk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2whuhnxsy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2huuvzfgo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pucfissz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mlrcsfxh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ahxuninz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2psosajpd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jwqvhcgr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dlvmrwaf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vavmefdg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2abjkdtsj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2txbwhnap.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jliehfsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcdrxtyx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xytkounw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrtdgtae.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ahppevmk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wxmddtun.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gqyhcajv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nxmounxj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qrrutile.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tbtmndbm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zkzcfarm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rmtrttob.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ulpxlshg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2izgysmpm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nxqnddyx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wrfihety.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2syibersb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fhhcpvhy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pingonfl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cjquomtj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ovrlyxqn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2euwvhsso.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vvhhwwpv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nhxyttqp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymmsezue.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2lvlwusns.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gixymdbn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ypafwyze.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mkfdpspq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2onkvktql.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ilrcrjvw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fkxjuoul.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ocyaklhj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qhnluqcs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tboyhrsu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2calatgtd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hxevggfs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bomwovic.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nnmatxwv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2judmvswa.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2aevmrcgd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xhduzbhe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vaijxtsd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2khegbojt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2moywdris.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2iiufqotf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2khacgobo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mzfrpnta.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ukcdehir.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rokywbxe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mhklfukk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rygvtofs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wdkuurpy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ahwgpbmf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2hojpxvsi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xosziggw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tmmyeglf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mewmltjb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pscskwza.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2utgsvesu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qbrdvzvv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mzbhdmpi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iycvzvfe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nabqpwmd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qjpzpuer.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hwrivcow.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vmiewyew.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qawhskbq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vdntypvh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2narjfzsp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wwzrmgin.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mhhctedp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wkvqqcny.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lfsnlilx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2yuzwjovk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wygkvhxp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vfgxptvq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hghwkmao.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nudgmlje.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2khpsbzyi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2sschcafn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2beucypcn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qqbuidjm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iylqenoo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xewsycwb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pflzkauj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xkjzskpj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fxrroqqj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kdxcgdqq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fpofytfc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wdwraukx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2dtbwemzl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gomecbel.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tsfibwpm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zhpbmurv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zhiixneu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bqzovwdr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ejnqtevm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gkagrwaw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2blhkzatt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqiofosv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2herwcvmy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rcispcxy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ijndcsgw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rxpxwppd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uohgwzam.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jykywdao.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2oizdcwni.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2mclrtkmj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfjvfaov.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2buuczvpy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xzkfwhbw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qlknvfvk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vhsngmst.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wzcidzhz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2csjbijoa.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvakeuyt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rthpxrqw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bkyugtcv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zcxycpmw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wydetotz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jcybradh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fnvfbevu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nfovevst.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpnyhnun.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ijacwqea.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eljdqlhk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cixmwhfg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2owuvorzt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nsrlmbnh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2oovuxjxo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yzerdrcy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2sgvvobws.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dyuijjzi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vzaatzfe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bpbriajf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tjtjqzvl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kwmzeugk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ifwlqjis.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wegupvfo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wjzanmvd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bmtykcuo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cwglnlhb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wtvyjurx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jrproacj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nilupkee.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2brrwcgkk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wvizlbjw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wlgiflcq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybzbhcpu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rkiqbgiz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2muuyjdsz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2njtrczwq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hqldvqla.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jsayvpay.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2baqxauxi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zaywrupj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ylbvjrsp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qbhnwpjb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hencvvfc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vbxxcdia.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fxcalght.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbifhcrc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lkjaxquu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rjprvaln.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ftlaythi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2uateakbs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dttgaguf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2umrrnvys.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gbcrxxem.html


<!-- 参考信息 -->