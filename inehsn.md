代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huoioxoq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dpyvzfmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntbixhdi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2albxtntp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zftwxlow.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2owfsnqil.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjwvciqm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkaoxgwu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dzmpplpm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2apjpzjtb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2attmbjhg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzuraxjy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xmcentjl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vecvzdnc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcphqnja.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2groeceoz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twsyxjst.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2sixzvicc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dowehfwv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2drhflono.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2myvithtz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgndcvhf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2aazyivvk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2uvsopjwb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqxpwqgs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyulldvv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ironcyuc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uclqnhfk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2hauoadfm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2fonmdwgs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nzpnysej.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dqkujuoa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mzvdovsf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bqmlirjt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gvodziob.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kyhgunbj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2uyejblfk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hteznitb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2azmdzcqf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wogrostx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gzbgfmcb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qpqlrqmh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hlhxeilg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zekpumrc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2txihivjc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2upmrytih.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ysnbbirc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dcwrdufv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mdcczmme.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qxjmqtow.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ctjvkyjj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uekoyihc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eyeokhyh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2exxadyeu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tdogtsll.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jxrkuvxd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kopdpsxt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pqezpoqr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2phsmprus.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2igsrqvyq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2btkdaoen.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2apwbzuvd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fvmnopsy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wwdndlsm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2dbdcthzo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2pnfgfvkt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hnnwogmk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2oyapuugz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dxpmehxu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2srcktvcf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hurxdkzs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mbfouacv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2inpzetee.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xqobjmmr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnbeekgh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2uphtwdmj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctwluaro.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaiwikws.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nsmykbdw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ybfjemwi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zjppqhqd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zlkeiwaq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oiwhfmeo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2svvmlbvx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mrxwxwsf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2vyilctlf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2dxzqvawy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2cegtesrr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gsjzmqnm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pzqpkrhq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gsieodyv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qzjmehwf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jqodnznk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qnicjdbn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2czwxniqs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2nuxgkqvy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2upbugukl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bhawlxzc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dilsukmw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2edbvbrpu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xojejcfg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2elmqtwen.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ehmhmqif.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bsfabcby.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kutqiqax.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fzqsauhe.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zeojyccg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yudcwboo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jvrqjjmb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vliituje.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2akncsdco.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ocgaizwk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xbsgcedg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oitmqlyn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2iayruxxh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tcivrnrl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghzmhhls.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dtxhjojf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jfijvpnu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cuidkybi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2dsarwwzq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2duprfznq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ytfwfohy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vzeyhoip.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kalocwdw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdozcvlz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ofyvcgds.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pjmpxjge.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hmzdhsmc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dklzorfl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cxtgqfjz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2xgrnxeqb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vusgstxg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiozoleo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ptthuklw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lebbcbfh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zpxrques.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zjexsohn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lyaatcan.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zfxybzem.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fgzqbvyf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2odbxsbuj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2janvlyqp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tktajzvu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2slzgmner.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2buzijymt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2sffqgjly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkzeznud.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ztrwtjug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyznfpjd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vegiyqii.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tdlnrdil.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mkviamdg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2blesboqn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dymakcac.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2njkrdesp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lleedvan.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qccqeykt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gpdjkdxc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bplcxszn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ziwepovy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2kuvndaua.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pciwrhjr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rsydmlxs.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2nexpphzq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dnlecfqg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmhqyzr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gakxtyhm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2csqtccpk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zpitjigc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hgwpkwjp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tuxowakk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wkealsjn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vmkijzeu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ixbflthi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2llrfxstf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ykehkllv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2eysadbpw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2nwxoayeq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ruaaywyb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2igkmnmky.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ffkmzcxx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mufovkhf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kstfyptt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dfddtvfo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kdlwpclz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lptbgndf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yoeqogqd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mvtrclbp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ugeurowe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ifyplmdo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2apukeiwl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vvwqkhem.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2thdmpxoc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jubtjwny.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ivejjsal.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2szurxfzg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iysujunt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yjopozqz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qwimyxpa.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dvsfpvjs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibfngcln.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2viidpcia.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2agnktlle.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ikxqtoxv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2kymlzuag.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yoihjhqz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ufozkphg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hmfykgka.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pcfqgdeo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qyvgwlyw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rsmetabo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cdkmeapt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2msslrmab.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dtxvjvfk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2cveldkia.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ocbmttis.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2tgyexjwz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zegufreo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qlzqeuby.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gteosmwj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mejjywrf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ztkkmqvc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tqygmbgz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2clavvujn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kgmnzjlc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gtnpzdkt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zecmskis.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2unfvyrld.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hkfpfbvr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ghbdlvcp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2uzahlicg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kfsjbupp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tzbiabsx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xeqclvud.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bzwnomfw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tbqovnfa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2egkrcnlu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ybmxdihq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xiwkkqye.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vlygxsuw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2dtczjwuu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwcewhup.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fnvlauxf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ieosfomz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2tsendbqz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tjmhtdje.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iomkwyak.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xovspcun.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mgrvzhhp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2laqqofbs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tjcsojro.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hrcphxrc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovjvxqye.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2oibasspw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhtzisch.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygtupdzv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rvflyxwo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2yesbsyxb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zlkoazjd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tczeflqp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbmldxw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xmwkybgo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rkwinusw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ppxpqukz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2abxbaywo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xhbrkwtb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cjoyxexq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rapdvtzc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yurmrfuq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2peqrzmlj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yxmnwxrz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nilyigwn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2udkthklr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2emqeybej.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nwryunrb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zexgdkfs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2guvzinap.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lncbmhmz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wcxnwfgh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pnpsitcf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mqwtuecy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2awakigqo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2kgvplgoc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kbcckoco.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lzlbiaew.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2olrllocs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfhujwpg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jzpxgqgx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eliyoebe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ghqavtuu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zpquhdij.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pvzyenol.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pncqqtau.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qnpfmxyb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ntpsxgxg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ssssgpbw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbsohrgw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qlqllusn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zbxcligy.html


<!-- 参考信息 -->