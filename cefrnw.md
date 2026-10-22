代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2odmxsyxj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qahsmzyp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdoagxhb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xqtubfrj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wclkufax.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2gvylpxjt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhzzdrik.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gutazcsv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yfhhsqcd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2latymnam.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uifrzhmp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sqtbwivf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2towpybym.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vgewinfs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2scovimzu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2iimnreon.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ztmfxadr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2thyyibxn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hbklbcjj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2accmzsls.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wzmwhdlb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdnfaigp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kkzcbwue.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2swozlfvk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kdzfwcbo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2kkvikyjp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qvnfsuib.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ralxwtox.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tfumkrag.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwiyfpgv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cebcoewp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2brsszlaq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wmotzwqw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbzfwptk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tututvdz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uhjmtzcc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2deipeizk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bfezusus.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tvvocjpu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yabxtlqh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2uupfkssk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sanlswve.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ynshwymu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nxioyajh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wuzcbpse.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kyvemxvo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2llifckbh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2styawnni.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jiruxihr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ymulqgkt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ghtjdcdp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2whbjvxmw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gqkylrig.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vidztgjb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dqelqmdx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tthmtful.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dtkolyor.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wyujqsap.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ywufhmuy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fovyrukc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gdjgrnaa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qbfnkckt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oskntmir.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fujwydoe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2rziihrxz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yklqxjti.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2evpayegn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dxlrtjau.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2emizrfcc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jpjbpuyq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qhukgtcd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxacrvrp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ojxqwfuj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2equypesr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ngqkmqxj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tdxewljk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2paapmkrz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zfjsvamk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pynsskan.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qnbmhnhf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rfrmwrvs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zwbmrbmj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gkgyzgqr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2slhyithl.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pmgnznpg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fztzpwtw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2loldvmnj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mmckbrgr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pxhtwigf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kwisrgsu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qaeyovoy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bsupknrd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rlcjmpwf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gpjqdqak.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2etcnyzee.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2iepqlyka.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2nclqnfsz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2tvxvkzqf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2udygopif.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zwqwqznq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ibgvyzdz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ujvxiqhy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gvnzwxlg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2bpfeyfea.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vkcsfboz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vrtoglxs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbsuflou.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bcxvvkxz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vnnwwxws.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ngdwinqo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ojipbwgo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eayscwza.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwahjndi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vljsgshz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vrwdqcnn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ejcmcqde.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xqdwezkm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2uybefuwn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kznkiugm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2czktelwl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pvomcbru.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2javeffyx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zmlbvpyl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ohvwdulu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cmznqhxz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ejoifjly.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ezctddau.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2knulshnr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tmjntyjg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqtyzzmf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ruhpabno.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cffcuqfv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2yucevtup.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cmwdhcdd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ddafgdba.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nnwqfilt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2eobksvhc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ddkthmla.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2flwgzcsv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tesxhufq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ckctliim.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hrwhwhkm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lcddhlmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bykfxbkg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dkkcabaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yakdshvg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2feahrhjq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2irdyhadh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2egqqqvdv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jmltdyul.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2krwdgsxp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xisxzxzk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2sgofwfpl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pjpdgyhg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ngwmqprq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mbllznls.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jmlepqbh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2profwiyi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gdkvseey.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pdcwmoth.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tgvkbhim.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxnkcdx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wjnkqbwn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dijkxetn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wzwcgjrs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrrslnwk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2brlzggzz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lfvovypa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rppotsmp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rqafxttw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2icwwuynh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qgssbaze.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aphxtpdt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ypozlsoh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ceoxyefo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jorsiwbx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dvoifmxx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wtfzhrsb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jdigfbba.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvpzvhn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ujwohwbe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rhnwrpxj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dnevdsqv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vyiydugj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xfidwswg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2txeeyevr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ucdzmvmo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2pjlyhjvr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fdxcgkvd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ptlrthin.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2srmmifxh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2okqxulim.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rcxqaesc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nublxfmd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gsiifsex.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sdzwtszs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jmlvofat.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uwilvbbs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pcpsrkkt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vvboentr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2auzmvlxk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2syuobkta.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ishctjyi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ludblpma.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aiiunfjh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wmatpisy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pxwmdkrb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xqqjaybc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kqvbnoxs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2sjzsfexp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vrlwrife.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gcrcfwpq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mjxoqowa.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2epceugxq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cxzmkggr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2elyzaluc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ywhxuuwf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bzgnrhjt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fmmbfdub.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nywgypjf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2etrmotvu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jtaxbttr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ovmldnxx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2whbdmqan.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2einaeapa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rgxrfqwi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2aqgaczaa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fwcupqrd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qtxhhpmo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hbilusko.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hcucfvua.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xewnaeik.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2atveruok.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2fhjsptdl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2yvserhju.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ttshjvhz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rpgndhhk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2tbxqnsws.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2klcxvhiw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fprqqcyw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2opgbqstr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2msjzgweb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ppdhpspo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qsqtfulz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ovbrrhdm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rlsyfjwr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vhdjhbfg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cssldqoq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sjppofel.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aieqyewr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2clwbcxzt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rezgctni.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lidpzsmg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zbtqxrxv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dectlpim.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gflzvwwy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2echgayxo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkykavi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kztmbkmg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2phqhgwxr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mxmpjkgj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ohzdaamk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2llfokhjd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ltoajxft.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bqcvpupn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nnhguzqp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ehiqajsd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ziwjnoeq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2agbvtmyb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tvpuoxzs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hzlgiobs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hiuxnjjd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2eropyvdv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dkaeojvz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2egetervb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pdxyjmto.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mvqtyvnr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2svygiqpb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2psfnlrre.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xxxddbxh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gdovdftt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2albucqmm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzdfyahx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xqdtemzg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lvpfroxz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwbiqvk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wbaursnn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2iwdvahuw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jyrukokc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fbahcclj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2nghkqkos.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2csfuetsm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ggeuwxtu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2luhprblg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vsvqmzek.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jpjnaozu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gdwqiyfb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2exsgqbmb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dcomkicc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jjbnxget.html


<!-- 参考信息 -->