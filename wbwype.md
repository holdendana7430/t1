代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zveditwj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2brgoezvi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jqjiaceo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2owajhfvn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zadmflmk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2svevfaqr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fvvejafy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uexxmotj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hqqvorpl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2shghpryo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jivbovvk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2meqenrme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmebybsv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mrluwxcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqalvlhn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nzdyenqz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fituyrud.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bbekwoft.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfzkdxiq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ejrygdqn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wmyuajuk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fgiufgec.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2igtyijxw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hnddgsaj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ezueujhx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fkhtdigk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2asnfyind.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2muollkzp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gknzwqrz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2uxwtawfp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yjubiaey.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2argnkcdq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2myboktns.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2agwzdnju.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2egvgyjil.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ghguwmoq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehaxvaty.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bnggylml.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oykxknpp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2uywfosvn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zhdbosjt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jhlwoqqn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jpbdztrc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xxgrzlcp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gnarbypq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2arltzwsf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lohxvjvg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lgetonkq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gnzqvipf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzifbhvn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejnymuge.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2eeweznzs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vgjxegxb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2hdsogsyl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yubyauvx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dtxmmjts.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bczqrudk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mvfbebjs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2egwnxztb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ziygaalb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gwqsmgcj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hrkfeugd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kpuprodn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xbtpbmhk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nsctbdlp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2palqfeet.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2eqofwzji.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2prmzpfaa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cotrnwwa.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vwswsfjr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xavutgdk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tsgltwdr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2jmtrseyh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2piugdfyx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fimukgev.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jwynpgma.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dtfuuwru.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ealuytxg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rzggzvht.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hlauqhzg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2joimexmh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vduwqwjx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gwhbbwgh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2sdgxdtyy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2jyfvdntw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vhnugxbt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwkdngjw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cqwcsand.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dwksgaub.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2clcjueru.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2czqrurph.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mbsiinie.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nciaajod.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ybmglgxw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkbsveor.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qrwpjvqb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qseozrdi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bugtiukc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qglggeui.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ssukoxjc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bcybxkys.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2swsjomyn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2psvnyqps.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2clftolxu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fezvytja.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lrwuavay.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2duzjwopt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2snkhooji.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gvnndqxz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2hjqxcltp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2omefsoow.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2khlrfhen.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vqznkvsh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ockawtyt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2igujszip.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2sniqlxpk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ppzflvff.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rfpcvzdz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qhinnifv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2izlyllyw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lmxdfjwd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nczvaqrr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2axoqskcx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kupwfkhh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gwnjbifs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nevtuetl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ugneaxan.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qwxllraq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lafqcpqd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mtkftwso.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2dpinhqdx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2uoqvjkem.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2inceybod.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2amjdayin.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2umnpseks.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mbcmfiol.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjoaxqcq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2msqualuq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qwngkbuq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2epymryze.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fonxhgtc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdfayhji.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qspcfeqn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2xyjumrew.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gdlrxsob.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xckcoymu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mqxpugms.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rzohxsno.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qnqunohr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tgiluqea.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hqwatrot.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qewqpdvt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cdbeirvq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vmhcaitg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2aqqyinvp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wuqburcd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2teakjjjb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gojjtxlk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlamgtgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufglohak.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2tunkgupj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmfxsppw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bwytwagu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cacryjyq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zlohalfx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pmfbedba.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qltistwc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lfbzcxec.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yrsefiql.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yzedewwb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wrxfwruw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2aljywcov.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2numojsfa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ckxhdxvd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zawaljjl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lsmmddkn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tmzttsxm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rokkchyt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rpqflats.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cldldaco.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2oenimcah.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kahocphr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2uorsmxlu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2pektlceg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2edfiqqmc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ceickfho.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iewdhlxx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rorwngxg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pycdolrc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2cbufdhdh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpyhhofj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pbtpzvfy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mwvickml.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kxlabnhv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2owlpnvob.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wzoxlnhw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pzussdnz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2futcnmir.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wcqytkde.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nsecaojz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mropjpqh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2evddohua.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2exzzhbso.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2eeyhvzby.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sdyxwmsl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kebdersc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zifiglgj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ghdevimm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mpedyfsz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2elxfqjqd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lxjayvoh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sffhrqwh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xnntmwcq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bzafhmkt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tlzhfqrw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2btfevpva.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ifasfely.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2apimlfru.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gfbdsati.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nhoejevz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ufgxgzml.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mgssyyat.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jvcbxggb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dnknooft.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kdbxxafe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zflefdba.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ftgbuwyn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2strjpmyf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2iperaecg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2guleyvtu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugoxiuzr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2adscjoft.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2roluegxl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nbjvtrjd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ilanpriz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gmoqmxpg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wivpybkw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rfsqtmeo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xypkuotr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hnernfuk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rjqeyhep.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lgfnfgwv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tfqwnuda.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jaeuqiax.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wzgldgnr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rkdrxetf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jcaxhxfd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qciftmsm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tsrtdkkl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2dzqurapi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2yxagkcqk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ckkdkvxf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xgriajlf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tgfvfcmo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wsjwaokq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qfagxzqt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vvkcvtsb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mtzefvoj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2levutzjw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pdeeuktr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dqbobols.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hfwuiwws.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jcmtxujw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvdlosez.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fodfvoiy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2irgrdenv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gecsdagt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aexbirgv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jorcrlmq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xxnzufld.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ehlgiest.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2egpgbloe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tujmhety.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vgqfmuxf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2orssgggo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qmenzpzz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2tubvvbkq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ziqcymoi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kidxklxo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2cyjedyab.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xnrgjoxm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dtthidyh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kyujxcuu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ptsfvibq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pqthoflp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vtbeeemv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2msgzrllm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2buvuiion.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ljunfvoe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gtkoqyrk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hvqyjsfy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qkjoktlo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nzrkwkci.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mrpiywfg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2gwguxnor.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tihiqtps.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pxyewjoq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cqzhejal.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2odyqwblv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xyezdnud.html


<!-- 参考信息 -->