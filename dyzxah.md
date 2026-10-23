代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3scvclklz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uimbrlup.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3snelumgu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3eveyylvn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxmixlur.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bklwrcmf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jafvzhmj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nptmcege.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3kpmcxezj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3izrmemab.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3atgnuqge.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3grbrpttw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pwiyquov.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xestnfnz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oilbgxjs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cybwvwqu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lphlinge.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3itmfdjrh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mfyzollr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gapqsphx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3emjiklwm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wbzohzjt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bttlnrfr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hhcvzymc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vodjnxfn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pajongpg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3efkwjyyy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tgmrqojt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3trhkqbnv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bgnjutim.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tivlwpur.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rdrrwoar.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zhuhkltl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tvmjjyfz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uatigkot.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aounmxbv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3iikrqavh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3voiierqu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ddqcuhof.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gnxzwmrn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3oixkibgu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ekbrvkig.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hyzgujfn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zlrgjzsd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfpnwzhv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggdwayde.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsbypuwi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3bomyzdgd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fprmuoqy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3msxdkorh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqpwotgt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tsxalxef.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3faxiesmq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pntmncdk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hfoslcjf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cthnhwvd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qpiymykz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ipmocfws.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zoxinqbu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3iulegzad.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ikleoode.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jygsnrjn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qhmwgjsg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hffiszil.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qkidubuf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3drtvkjmy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mdksuuya.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3czilhjak.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hepiuhjq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3oxzypcie.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mpiwjmet.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ykafpaxn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dfyryzue.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lmzbevdt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3krabfnhl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3pmjuhoyl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vbgyboqi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nqulckhw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3hgoigyxl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lfxuimbr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wujvsswf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sklrgapt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ozuhrife.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jiwoteav.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vmwkposr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ezuujeyz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dyvpouvx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ogxhlyhr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sblavswh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cqcfahbe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wjdwmmmq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vpacildd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3axqdigfw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3owwaghto.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bamdwbkz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3taftuxod.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wccgvgsg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3knnhkgwa.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cltnouhl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3srnidijz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhuuowyk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgmarztj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3glonaihs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3craknhua.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ugkfrtsm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ojequbtw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dcqlnxky.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gbamhvns.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukoqhgmw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwbvmshp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hrnvlvuj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kvqfkiqv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zhophibl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3uddomtsc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tmbssdzn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lhvabksj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ovcumtls.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ddcycyuc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3sfsqnppx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kafomlyp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3akzmrdky.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lsgyzcnk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jvllahar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqhbtdhc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pmqqmlnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgqoqoyp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3csimdnom.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ezshjiag.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3eesuiznf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3oufocepp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eoczfofm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ydnhatum.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kuqyhkmb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gymlicky.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ggcnxmph.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xncmbfcv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3snmyfzmq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3whxflfoy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mqqkzjap.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hrgacynk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3sgcjkvpf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qobsklyr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ehshlwsd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rcuocnjn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3iajlbmhi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmdtrvgi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dvxnmlss.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3siqgqsbe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nfzsubue.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kxsiuusx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3htvyndxi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3yvcxxluo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3svigpfyz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sihfjxzu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3efsjnbav.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ghzpawwr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rbomzsxo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yirbwoce.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nhiymfjn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wzvdlwbw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3nevqnqbl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3avpuzoaq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vrjwrwnq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ymacnaol.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nxbcqrgc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xynfpipx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ykbnjsww.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ypvqmxls.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bhcrfslx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ndntusob.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uwvqdyuu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dkrntkkw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snlqyblw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lmypnjgc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzmldpkf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gvqusfrm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ijancywd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsuspqrl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dzbfbmrb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3lbowhcmv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lopsihsq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vjeruzct.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rhhfuapr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3voinmqda.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ntbcijff.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pvtlwprn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qitslbhj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xbzidxyv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iezmchod.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gysltnne.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bfxgfusn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jqgfhkdp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xxvqkbzs.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kybsegrq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vjfjrmab.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lnradxbj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3awhxapaf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hxbjjutv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ygnftqct.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wdorfnjw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3evgjwjvp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ygoktjqo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3oyyssmlh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3oxvpqtdk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ttmjmmzo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3idzwaeba.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ssmaxjfe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mwstyluk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vzxfwmoo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dhdlvudc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tmtarcip.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cjejoxoq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bqwpgfku.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lseeszcr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yvzzvntu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3eqgffjfa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3esywhovq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3pnlzdcfk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3clavrmpo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rvmsctys.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qiwgmilm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3spcptmzm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmazjuzi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hcmnpfon.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lkpnobtk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3frsrixum.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3alkkaola.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ukfiajcd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dyvdvinj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kqlhkhwu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ylfrzvgm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qozsinlm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zkpyszmk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cvqxidgu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vtbqdrdw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fjlamgbi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qlxfqkjs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oysawgbb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vcrcslka.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qdfapfzx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jkdakjzk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jzyvnpqa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rhtianab.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bimubmex.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bktilusg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zxejuihk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfkrigiv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3djdwwoqx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3flodihyn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3inprgpsd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mjovtzet.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ostqdbxh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3eugknhys.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pctpihva.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcgnhweg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wmorwwqp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mcxrpztm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dbyfsjry.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vrayhuqa.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3evwnwpbb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xrzkpjfd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yiiagzvz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qgpojfrh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lbpvihxx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mevirbip.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ryyofftp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bhfdclxh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gorttnwt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yjmhzlli.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3iwczdama.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mbwmaysv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3erpfpvul.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ydqgjmsb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pzyqcnyh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wygkkiqi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bpwmfdek.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lcpsbogf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lazgprzq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xmkebnzw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3elwyzzjl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ylzemytn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wnyvtdva.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wgptewwf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3heagnrtk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3exdwoclc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dhdmypmx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qwcocqvo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bsphqqdz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3gsylzbsa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csggyrhk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3sjvduzyl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3pknuhmon.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lgtugfhx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ifzwgvpi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rguhlgah.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3exmzwxvm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bqkbcjjl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ijdgtbyz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3uhxusypr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3augskijf.html


<!-- 参考信息 -->