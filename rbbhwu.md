代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osthzbap.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cgibcwzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diyttcmu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oemyqbwv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xrcwgsyl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kldcoicr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aluqxpmm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldrmgvvd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cdfuxyza.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3voscfhry.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zhslcjsq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pfryhfem.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bndwyxok.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3uxmdopsp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yjtsyofh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axzcgyvk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzbkjyrs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vstecbes.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzvcxbkw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3civbhwhr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xddilqqp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nqawoawe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3exfwgnvc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqyojeed.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnjoaarn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jbikzpuh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3somebjqf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ixwcmhku.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bqfmaiga.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kdepknka.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3fcvxqlvx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zncsohkg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3apntsfqg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3giryhods.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3sgwcrmvm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3tngxwscj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjbprjlp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dizosmxe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymhgqyuc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wjymztjm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ablscqgp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3folpxfkj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uickpruo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mnklgouq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3misgtsoy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gvaayffq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lqylzdoj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pqotzoaq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jheaenga.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uwltnhzv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3asecmyyu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tlhttoid.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3agdgqdaa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wjkknxfb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zfjmvhbu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dsjnpkdc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3exvwcbzw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fbnigitx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cbxnincr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lksspycq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qprywvig.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rahmcrbr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tjoeqrea.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vubsigui.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3auhpfkiy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3maxcrijp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jfpiavdm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3smhvfxaz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkqxiaae.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pfzuqltj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dcpcolbh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yxykpvnt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hzdzgalp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3lpvngznc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jajqocng.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nbndmjsn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qrecxxix.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3swhgkohv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wukrmaii.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3alekouhj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jexjxpfa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3sysqqwnr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnpgebbz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3modfreyj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xmjfbbnw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3irntvwxc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3zykaerpj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xxosclne.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xiakeauq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3npocecjl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xiixyayl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dprxeqgv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xvpaarwt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3cpgtglyc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mrktthfc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ezjclpnx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tdhwmydq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hwokpvdo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3htfuvklx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3nglodiyz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yfbdzljx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vuogvtxf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hjcwzfzg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3hbemcjho.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rqbbfqct.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ylmjikfy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3guajtaob.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rntrykep.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3eipaqgep.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wmbnlqad.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zgtfnrjs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3dhnwcdnq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kwittmwz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dmxfwrki.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hshxwmzy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cltuzokn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mbcfyekn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fgkjanuc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hrwndefz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ugoutcsu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3movpzwdb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3wzsjmtbt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3voeodnxf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hnzpddwr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfamafpo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfqtplog.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qtkjhzcs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mbbqkjyw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xmqipofd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3akqyolfc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3galdfvtj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uivbthat.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpnlhgbb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnmmsxof.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uarppiis.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dhiugrhw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zzpvammi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hplmdwud.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3sjjrdehd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tvqprrpm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3abxtyifg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mxpndjqi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ckjpxxih.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3crobzpjc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3atjvtitj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3buwsvhwh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vvjvawzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hibwqurh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tumuyjkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztaquvaw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zgofggoe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jyhifnva.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ybnuudss.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hqkwfrvz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3cdyhgkil.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vtuxpqxw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3syywvigr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wmvlxyji.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3dpddrmyf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lpijgbyv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cvbmkpaq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3diupsldq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dzbizahi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3krgixtgy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ywxhzsrs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iurzllph.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ckhzpjzu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yxnnlgww.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3enfsfziv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zchyqobb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kltkzhik.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hleuftjd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ppkrptgc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wxaxyqxa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ojzwkqko.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3utndwoga.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uyzyprrh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fcmghglp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ezskagvk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bmcbfdil.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rwcdcjje.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ytjrdpny.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ohmhmbzy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbznmfk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ammrwsdi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3korufram.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dydtkrqk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xfkwfdws.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ywgtoeor.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gdmdyplu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3htpvyshg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ygautlba.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rdlqqkbp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xzpclbov.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tsmapgju.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kixylzzx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wsnnbzzx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ippapenw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rclnclyp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nloepmrp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lenwamys.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ggchtmud.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dllpbzon.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jtwequoj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zlppclzn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3avrnbwlt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pwmkmzlv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tbcurpjc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xiscpavc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3onhynivt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3enphwgoo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ylmltoig.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofarsewr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kpkyciwc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ltkppntt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3guewfzvc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xmlfxmvp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3narjoumn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lurxkrgg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xkkrtsjg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3twnmrbax.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bcdcyfen.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3eujtrtqk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3invbxjkv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hjoymilx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jqwdwopb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nktifvox.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3poukexfy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3biroezik.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lomzipac.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3txazvxbd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hzegccts.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fairaamv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ddeysqfz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tbhqpnev.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zpcjifdk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ptsrbqti.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3syujdfeb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3hrlegnzy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jhottmmo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bznjpfxq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hxwlitms.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jnsdqdxq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mbfttila.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3itrfxjjv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3moagtnye.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3blgymepy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yskuivcj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3drbbbknr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hvovoxti.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3viojhzyh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wydywmny.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zuaobnmb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dxqacibj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mnhjlidw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3snuphwrn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qidvqvcp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3swbrelrq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3annwykyr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3yjqzmvcj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dctuijmz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmikprcd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfbdzbzr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxeibjjo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hhmiszyb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3upvohzub.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sgxkkjfu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cvpdcejl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pkdcfmbn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yoadippv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhpbeujh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rgnnapdr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3knurolzw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sbkcjhit.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3udgorigy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zqdlmkqn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xgqjeoyp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3psgxoxuy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sihuekcz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ztljicfn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3erzssahr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3fcskijtu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3diqmsshq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3pibharyy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xbrcsfvy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3acvvikrh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ccyssyad.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gybvouhp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bitdhdyr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hdrlohgo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zcaromby.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3cfwdztzl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3htrghegd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zledttas.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3uafcwuqc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3edbcboib.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hnywrfix.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dallmbrv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3engoyvnq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nsmnwywd.html


<!-- 参考信息 -->