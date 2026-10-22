代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pghkjdkn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ljkpsyck.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2whhfzfqz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qkygghuc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2igktdrpq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2uavktbar.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkuvyjdw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhsaphsz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xdkrqfdj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2aaludaih.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2euhbmhsx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vywxhvos.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jqkfftdm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kzjbubom.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2tvzicgun.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wvowdybc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2myrsyakk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kkimxjsb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2evghaaey.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hfmrwzyf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aottuled.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pwuftcjm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2icgjvosl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2azshgvjt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bukabzck.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jqhfdpet.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fobfujwa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bckqkuwo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qxqsjygg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gryxovpl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qjcqnuph.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2llgshiss.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2smmwwbdz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2glignusq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bjisteji.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vbofgfff.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rbowvrjx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dqulykrz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kmlvcglf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mfpgfazh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2laprzspc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ewhfopsx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fbcmmrce.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bgqogetq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ujrnnpog.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2otcoclpg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wwfaeqpm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wmjzjmre.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gjczcoev.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rmzpeuti.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2llykcfqp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2clyqxgcu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ppmfwayu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2akpcywck.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbbjelhu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2uswlxjwu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2pfjhxuai.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hngjxtwp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lxoxkays.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2wkhaudtg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ftyqwfch.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2plrbyvsj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tpbvcghz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hncrmuzi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2alqwvysa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rsbcrkfb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2edaevfvo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2oguamtzw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttsyidrg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxzplgod.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rfkwmlul.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yhozujfy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2znjfbipr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2puirrzfm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2llwwzfga.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ifforltv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2beatxxcv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2nzlwzkcv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wcihhegy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ddfvzbgv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hkbbsdhx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2svrgqbxr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xyyixept.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cprfhxsa.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zztlfbau.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2wzvjlqxh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wqtbaggn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dbvsauvt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kljkhhqm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kuxgcoek.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2sbbtmgvv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2yuizfqpp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2buzvgpba.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zgepqhej.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bnpmakzv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bsazjhhn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wkdzpfaq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hqyxahap.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bvmofufo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2aozoqtek.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2sjpfqxrn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2sjblgvgq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2iwvawesf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2eztnxwpn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cgkcmsvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gekfjenq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ghatrgqn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nffjjvnu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hefunpnh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ddjlgrhf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zwavquxy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tjeugqaa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wluqnhyt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2afoxevul.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oyrzgbzi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gsoaqwcr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hxnipngb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ylbzlstb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nzefyufi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qaajznjc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lafrtldc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ivnjdgdy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jhvjkttk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2dwnrdhbs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txmyplgf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxyfhqbk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xwpkmdsy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2facxihqk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gnexfzbs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fnovlrwn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jfazojfv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hpdhicbb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dadxlnqd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2wdsyisiv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hvlkmkdg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rjdqxgcf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zpiywzju.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jylbvhoq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ampknxtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjpwfeny.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mxyaalia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtehbmtu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wnzbogkp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tpmfikwl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wuyamayk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lobvscjr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2owvlxhvi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ntqfifch.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wwjjopzt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2khwdyiqh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ldjowcah.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2edrgulus.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ntwsrnfs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2atdznbsm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tdelkcqj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vreupctz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tywzxynd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lchvfjfp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rfimgbgj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uwkscgro.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pqeychdv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wbxwvpze.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vfdtumad.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2omcxwyze.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xwiwvjsr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mwuuhrcl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xlyvxgqd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2oivpvtgq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tlveqhpq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ujagkabx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ecvwxhqr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtisjpfz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fjqembyd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jirfbbzm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2noukglvw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zbrvuyau.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xiixqpyk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zztbbuid.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2pgxsdoei.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xgqwuphj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mcrysype.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ruxqpjjz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2quamzqbg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rzgmzwdi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hrfrwumq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pgylsene.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yybydblf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pnthqvrv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlmzxgrh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2esbioumu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kjkemwur.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rvupknyk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wwwpxfnf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vhjkanbv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2elgsltrm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cflolawf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2shjupxco.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2frvaifhr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2louuhgxh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vkhsgguc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mmfkjlnn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2prqaizvq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2mgkbiawg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zvlexarh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kpwwyksb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rfyuenes.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2oowexhza.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dhdwsydk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vckkrube.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2baybtznc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ysbbsjma.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mrndidet.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jpfjqazt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pnqpfkxz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dlydyerp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rkaorsfc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ezwardmi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2zuskqphw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2psbktrgr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cryqddmu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gjsqcwrl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2blqibzjk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mktvhici.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bhvbpcbo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rwretwqo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jrdyywiw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rgguoyzj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ypdluqol.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mgwldnqz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qchahipg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kymjkdew.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vcogxvpu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kozilobo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zyzvoxom.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qyjuemqs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rzxrwlqu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qgnpscuc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vaxykzdo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yeujnwsm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xrjcqtaa.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gunmjzwx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pboaakrz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vjalpmlb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uyqpojgb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2atnmqfix.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcxoxro.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2mfifavdc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzebbayh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2byekorsq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zysbwbgk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ezipaqar.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dpmlopwk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hjlqllsu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjcbfzje.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bxmyearz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2lexlpzib.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cctftrsi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pbrmmrlw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xhojcgfb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gzjkvymr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pakfltrz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bmajdzij.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2anspwsvi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccdblokg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ftlykloq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bebicftz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zkhwjgqd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sirhojhw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pzqogfcd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tiivepxp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zgnrhalm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fppidhic.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ggwqkntp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2sbmvlfqf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ifwpvsvp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mbvdyrtm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2sfjdghwl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ocszcvgk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nakgnjuy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ocdfiwtt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qnqdayeo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iafdqxow.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qekheerg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mzsqmkgg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vaehivsl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2thssdqez.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tmmessjd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtbzfmcl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2onuirkzd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2uzfereja.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzavapxq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ezzdfcof.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyfsmzvg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fklowxjn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yfcoogis.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gizogrxt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2idbjxdar.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hhynmxck.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mhhntgtm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kloilyjd.html


<!-- 参考信息 -->