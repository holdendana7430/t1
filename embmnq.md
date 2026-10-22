代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wgnxkspi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ymumhwia.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dvutkqzg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygdoigtb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2elgmlobn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cclvtfdb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yxvncklf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2udczmnsz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkzylwhe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2awxjarmb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqpczcej.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2teqwxzrg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2skcaavfz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mhwmkmll.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jhkavkdo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpuycywc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmyndzuk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycuvxsar.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ghxkiilo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2btaxyijy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mekustsz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xiowgfgz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ypfkxlkz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xluzuwpc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ihemlrwg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpfhkcdy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pzwybqgo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2dmpcdikv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vdljqnng.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ljdvmtyh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2panjrbsx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2shmrpmbs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hnutaexb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hybnpbqq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cpucmlae.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kcepgteb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kqbfcvrz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oezmzdtm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cszyfvit.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nrflvesg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wenqnsjb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kknsdybw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qavnocep.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ikwodgiq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bdkqlkwf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zafxutfd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mklyzway.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rggzidnc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jkilhrqf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2alwmmbiu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lepviqsn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfupogub.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zwrnlder.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lqpdnbtc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hnesaqek.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wckaspcy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uzjkpcww.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2srzwrowy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ugndozxh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2bxlspozc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2muyvkvez.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndwcypzw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tkftcpvx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xahrejmw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zvbfenvk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2sumyaepj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ohscdkrh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dzfrcbxk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwvtwcsi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykikpwji.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ukjpmxmp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2howzjfji.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nlcugudb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2iromiyjw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yjziupxj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2pkvsdxhs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2smdbhifu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mfkadizh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2slnjytdo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gxqjkkzx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iqpnygtd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2isldtcan.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lgpcydyy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2illzekjw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2btqeaevt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vdkbqxnq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2bztmcvzl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vsqnpoje.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2oswnjwqu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ecwbkwrq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2iniqbbmj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lludecyn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vrspoors.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fxoeqkus.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jermocpo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2abfkdijh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2uqaasxiu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kikeurxg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sjojbmju.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kdtedlyx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hkyxtbld.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2kqmfshmx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2aiqncgzy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xcrbghxd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ebxiguwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bmkuybdt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2sblclkaw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksgyavfd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rftksixg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vazuyagr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rhpflwri.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2apcjtsgq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jgbcqtze.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2tkgwekpv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ujqgsfti.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mjmuosnp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gzjciifx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivnxapvb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hztrjsbs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tygwrjhc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zkdrokjg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rbajkuwi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zmgjnply.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2agqzyqnw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wbqggofx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ldabazvw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2iekrndry.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tqciizqq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2uhtypiey.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rraunsbv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mgaoaloz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zfinhcvm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qwcdebys.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2bbbzkxaf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2edjvudlz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bwmtfiqj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hnixlbrd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lmqavtyt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2riahnlbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aslhfiqm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jwchequg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxtcrlld.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jdlmfneg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zwuzvxoc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kwlufumm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vozbwsib.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2iqgluahq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fzpipdce.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uumoaect.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2cxjsdfqb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lxnpdxtw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rgvetppq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2sqwbhvtg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2kopfzgld.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvqglyqz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnfvapve.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kvrsgyir.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mnoxngqr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2znqksush.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hlwnsvue.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uzalceeh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2czqrterq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2abgsckxh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jvocquht.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rsjphsnm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2juxqtseh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jktioriu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qhsvatah.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nfiiapis.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2oksovmup.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pjecjrma.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2skidkzit.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2edugjwti.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2axjxqwxp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aatnzsxj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2hvmsjksc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nwuyuhid.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mwmqupqd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2biizkhjm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tcaqhlnx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zqngbtdf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sgwlkhyl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gbrrchrd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2nurbwtkq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ibezodao.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gbuimhvb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bthpuptq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jryqeizg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbwapulc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ptbryveq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wymeqguv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xzvbcula.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vswwssgi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bpzwbneq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jqjzvlry.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2scedvrns.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fbnsnnac.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gexzfouj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uhygfxdh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ybbobwoi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ppeerpck.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vtslrxfq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2nwughtsy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fwypjqze.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zbgnggjg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fubhaslp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2swnfbkzs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zszlzyvh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ducltwuy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wgkkeqgz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2twdfujwh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qojpbxdy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gwuxpmnz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zhhqjkss.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lrzohgnc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ctakwayg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzradzpc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2sgvbcifp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2biqjhvej.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2uqqanqvl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrsampfm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2upzaechj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2nklhphnh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2leuvbmwd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tmnmopwp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zschgkwh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pmwhizpj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2knhpaxcs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zndjgmsw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2fzioeovi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2yavrgbjy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ssyqcsrl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jqygfhzj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cyyayeno.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hadsbtem.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mikgpwha.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2uzzlzwmo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ubksppxi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iioetldn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bizpzsnd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mrnseeqr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lcxfwxed.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wtemfena.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iswshzwz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iwkwfhco.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wusfqeur.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zgyxtols.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bcxbddzz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vatjfemy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2unbowhkr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jfsiqtse.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zkxnixjy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wsbptlth.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2iddsgwft.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzmkpcpm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2theulrra.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rlhkyueq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pcfjomaw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zmmeucev.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2uzgmwmat.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vssthidv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mregmwxs.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qvyizyze.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bqzhiahk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2hircblka.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bofmbngq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qltpcxmq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iltcwbvg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nsncjqrm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2auiickcb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2czepdmpw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vcwsgkpa.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2feourhvp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tnhjfwmw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hepfeyxg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2davvquxe.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mysddpfn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ezopjmvf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ftdvvrvx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2grzezllt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wkuxkbrg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2naqawwrm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2btghzeyd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ffbppwzn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ghugxnsw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kvdftzbo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bpcbnpen.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hututjbu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nglynjdp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2oixrsbqh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gnsckged.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tilsjbqv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdldmuey.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jqgrkmoj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ucqgkqmp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2owtsqzph.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mznfrgvv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xysqtjxl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hvqmrwwv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2gdrewrqu.html


<!-- 参考信息 -->