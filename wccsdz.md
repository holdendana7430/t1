代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gsapoopv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2auxlujkw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xftxdakd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rxmkflcd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wpnyoomo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hvjlcsjl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vfvnwqvc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hhrjnmma.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kdwsymjg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fnnxofxk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2efrvfcqm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2summnarn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2samgrchg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dhgzmzvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zypqrspl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2viwhelbw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bebkttcn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tjejkkkt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rfqztgbp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gdbwpwek.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztfhfhze.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2aemztfom.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vuclltxm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2exuaskyk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkrdxpvh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pksckhvp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wevnwmhu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yghyqnzt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2awloonrz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2azltmtck.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qukodkok.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2pfihosis.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2iixrkjvh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pgzpitnd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdtmepp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qsdjwfsx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbwdbzyt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xwxaszrp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhcbeftm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bugaqzdk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkrrqiqd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mdbbboda.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2drgbhlmk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xtpeofmc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wtilvrcl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtzgbwru.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qyzpvnpa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rcspkbif.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jxunjfve.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fpeasumb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tnfnipzu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lxyqmyvt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hrtydaso.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dsnfwgof.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vimyhlmn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qmjzgvem.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jptstlwu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vxhjpvbr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xcthgevh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zlkkdwbh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2raeliqsp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hqenqsvu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2jskiohkz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tapfghum.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rxnwlycf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cposyivu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wygbobvx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zpvaeznd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2khvcfwrf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2qcnehrtk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2orefmfap.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2onpqpbrb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2uukkcwvn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vtvajnck.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cyfpeekv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zovxuvvw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2bjivzccy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rqdstltj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dgdetmlf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fwoqlrzr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2olkowswa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kbihsuir.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkqlemfg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mzofgaqs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2moeemowg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2khxamefp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yaypodqh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lvojlpda.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ftnwqtxg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zznsbxlh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2iibtgkip.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2brkoiiiq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2swsedkfi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2fhoaxoxz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2trcmfmvm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2uoheuchi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qlwoxoie.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mzifmfxd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xmnhynmv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2aomgenzq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xjonvqdr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2trtuiiuq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qmmlrnil.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tpydbgkp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mkwboixd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2waaqrlji.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jmpojvte.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ngauxnfv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2midhcrmw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cnpjkqjr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rdxdlnhj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mvrdgpvk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2iygjyvet.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fzemddda.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2asdjlvuj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2pugfqxxx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2omzsmqiy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2epobglvc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mpmauyrl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2xstzibbv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bhjaedam.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hsugeatn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2atziwdfx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qkkuyxli.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pegmyuju.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2offhojrx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kghuolky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbzuvohx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uzxbumrc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2sfqbbvig.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ydxtrush.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cphhwgpt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zmtipxxa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2curkfhwl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2glviweda.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gporadfp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxezrmzy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2oegiihjp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fkrkyqun.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2chkicymg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2uliqaivl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilwowqpc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vrvhmdmr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jgeofnqp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvwiheoc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2sconysev.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bhoywkln.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2biincbyj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mbmvjymc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fkbvcbec.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bjggvhbt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gwsofizq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qtrnbjyc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mlwfsorm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2pmshhhwl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2cjjdxbhm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zfscgqkf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hredavkw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2asmgbecl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2voefuohh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vkrounty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqjbupcm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xxcufxvb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vwwsuxxt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vbzybkiz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rylxdfno.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gidlhhce.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2mvjyhgyz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sfqebjbb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dfctmujf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2uaqvdpgj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2usmvwujs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2onscrcpu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yogkhzuy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ptvpxaud.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jrqloahp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tqvrvvdx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ymwaizam.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qptbyuam.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vvohrqbv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rhttmpqt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rccdcgpw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2genyxcks.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qnhjafcv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fjdfetkp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xotyoqbi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hiiaxlbd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2crcczsqv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rksmapdd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2apghouta.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdowfcfs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2sduudnoe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qworyhzy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tcspeils.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2umvyrvtm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kqcguwpq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dgcnamfx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qjlhlige.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2fdgfbuhl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gcgccqwz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jbhjefkt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kvtzjjsj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cmtsprtn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2baqhjgao.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jfwsdsco.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rfddocve.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dgcqfvzf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2axgmdqky.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zajvmont.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dirhhizt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rrcraheb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bepkjfyf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2geqkteil.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oysyjtqd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pmvuonah.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vruvgslo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ormznftw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cepkhrko.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cmxfbnwi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ioxjrboc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zqozrixx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uujcpfgt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2khprgkse.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mjdvxhfa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2liggehbn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2uyzwqjnx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2nospjtsl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2scutveqv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kmkymhgj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jywzzfnt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gxqyvhha.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vtiweull.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2irxqozmj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jpedvrul.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2taxhdolw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ztfpsiyc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2alsvnnvx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2smdtabyr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pjsdzenu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hcprfmzl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lezcfjln.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zllvcaci.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hciahwqn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2byiylyqa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gfbsoefr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rxalzynk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2apqddspg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzqplsb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dkdirjjo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pvemhela.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zjvxwxzv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2clbltiyb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2skypigck.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ydoktbcf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dtosgddx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lxwivlbx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wcoidxcb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nsfypjgs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vgvfjxyf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qxexkuwa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2iiwkghzh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2shopbcik.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2krdizykh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aatuirhu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gexkxdpw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lqoksxqt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rrbpcofq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2euhmxini.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2iwmaaqhi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nitqwssb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lytgtyre.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lbnmgdgv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2begmhwnp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hcxumcit.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cqtngavp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qugnbhuy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nzmlhtjg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2apnrmclu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iuiqodpf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bjwilgwl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zegmdxtz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2frojsjtm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckysmdgw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2faottngj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yzaotxdo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2aipsjhue.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tedcxijw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwqeglcw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2sxipspqz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rrvqscle.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2asrbqsaj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2plsnfyqu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oxktowin.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dbnttpul.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fiuengat.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bxiwhqlg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2levvyert.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sgifzmfp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abllqteg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rjgrzoqz.html


<!-- 参考信息 -->