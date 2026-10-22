代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bjbjasso.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2sylpdqyy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2stxrznwv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zgfrxaoq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2lkzpafys.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2nwzhmvoe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2lzzwrbrf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zrhuvvaa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygjssiki.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qqlfttpt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2epymyard.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tmnhmcez.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kfukkcdn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tkwyeloh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nryybwdh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ezgkrihi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvdiyqrh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqtdiijq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xykpqlsh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2voqxykgs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mdkbqams.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2tqftogaz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvvsjmtx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mghyehpt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cwyhzkcu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymcibxax.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tpkwztew.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zfrbvjgp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2illwchdc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yhvclnqh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pebvjazj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vvrlcvqx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nvqxhajg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2yveqhtkc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ccpfozyy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2osncjqvm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zgbxkubn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cngtxmje.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zfqlacdf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lfbnpxig.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dklybxmn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qtcigskr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2sygwjwfp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lehnwyhe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fnjcwjgl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2emgvyyue.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yvplwpga.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xtsyxybq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vindacia.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vnmeegkb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mzkuozti.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xtenvkfb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2focelmsu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2sppijrka.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2syosvbau.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hitspeoo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ezkdmfhk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2spxqlwjl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zixoadmt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2akpqmkxx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhhsipoa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nsfqrtub.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zswqaznp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ijfjxkmo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yuvrntfv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wldtwoed.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2anpvqpaf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2btiitdqa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ttfvusai.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqvejpsd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2eottpcln.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ozqxxezl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jskzrlqv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2uzjdrseb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2orohqdwb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fschtcxi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2djzvzpbi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mktmfzlg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hulwjjqd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nksijpcb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bwjzevby.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2irmxjeoz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jjfgtjrr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wldnzyzr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2efjmiaky.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2mppxgogp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ccqxuocu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2smymzjnv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2swoxuqos.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2iqodisyl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xycbgmsh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2llursnsg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2nqeonvox.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fcyhubki.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2uxxnreqm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2esztbokk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2efysrpol.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vbdapmss.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zzrricis.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hxjvawhq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2idjvmpdy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jeobdfpj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2cqetomga.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2afdyuwhi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2udqxsnlg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yupprtry.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2trqjwxdt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yegghnmd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuuafwaz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cdwwojso.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yhbhgpip.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nfitwihc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qfkebllu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2allfencn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vkblhiim.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zdslizxa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pulmtjno.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ahhfvmrv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dinnnuyz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nkqqdczc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ecyzqdhx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ndizvfho.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2azzpfizu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qyterkzu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ledvvjmp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2msfmhskf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nqstwsvx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pfltemvl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wdiclkkw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xfuepzcj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2crzornop.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ooetgqwo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bbcdowwa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fquhwuse.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2uidxuzmm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nytxywel.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2nlhjwzqf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gucobhxt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gituuzmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtlcaylm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2foboosyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrkbpywx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2avfawrmz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vzfrizss.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jvnzyegq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xmngdaui.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2sekcrasa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fablrbwz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ydlctocj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qqoxblxv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2bnunsyfz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2kwwvyjpv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ssygxqfz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2dzsbhipx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pyxcrikg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2aqlvoilr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vzepxsac.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nddorioj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2eotkpnpf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qjhyaqox.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dupixoij.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wbklnysf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qwabahks.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vqmbjpgc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pztnpmzh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nijuwtbo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjtwgzz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2svvczzhh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dimycxwt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jakatlok.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bosrmbtz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mjxexhnr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2eetdzhra.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2slhreode.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hmksyyte.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ycuolchs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rgbogjnf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tdvulskn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2keuttuju.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tysidzpg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2urfwuqky.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2druqmqbp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2yiontrxh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jlueijvk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cjmxmegg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yermufdq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jjpipdub.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2itcbgjer.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oxqhrnrp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dthykytm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oasjgcjr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rqzlwjrd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ngrsstwr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svckgfae.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cwzjulog.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ytjmgocs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2aroukiua.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2knrljcey.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2psnhwxwo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tzdckoer.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kjmydhco.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xnsywkho.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2troceigp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pyitmbgm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lifoikxf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ujpdfiow.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ksvsqtiu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qjrbwvbl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jqutvrxv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2cjuhsuyy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mffatbxe.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tuitsgly.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ztkkjqow.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qqobbkku.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fwkqdplx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vqunusfm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rqggrbdq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wlmsowog.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ivpjhviv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2urzdtyjs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlwnyvrf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wiagfnjw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ffctwpwe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2pmgpukve.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2emgwnria.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yujnjglp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xiliwlxo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pqkcazmg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2manoygka.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cgumzfco.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zmqyvlxq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2suinrfub.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bydipecq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wbitthts.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gskqjjab.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dvscbcrg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ddoppxie.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2qezfnxbz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxgdopwe.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kcyghmuw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lqywezxy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2cipfhurs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wprncuao.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dpalsksg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iaywgqne.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2baapnvvq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2thhecvss.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wovkgose.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2urzgqdtz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nmfynsxp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vfqcizze.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uddobjwv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lhgxnkjl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dqsyagep.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxoeqmcr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2smkirtmc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gzcyolyn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2jburlvgk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tngvirgv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zmzbotpj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rqbafxmf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ectkvbwr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cizupyaz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ackoetnl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2hlwbfbrn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zsqvncpm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2naeiocwr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jjddnkeh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2uwwxuqbl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ezbvjbky.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hxbzjjgu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2khjuyisf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vxdvpymv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2btnmygnv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lfsmovak.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2snistjld.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2sswzrxmg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gelwuwks.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2entwdwcs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bqfpcdkp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2whmcjmwk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yewrtlnk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ligmbeil.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qzbodden.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pshejqwf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hasffjtd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fvyavlql.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ldvkpfxe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2woqkcico.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tqgbxxvi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nbjsgbfc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qvtfymyr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2asfqqbyf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2lclbcncg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bvihunop.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ghiuntxq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wcpuprqs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mzvikqso.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ksgnctks.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zecyusyn.html


<!-- 参考信息 -->