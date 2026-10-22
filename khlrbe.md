代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rnrrlfkp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wzitndbo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cbzquwhw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hnrrurjz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cthzblbm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fbtaaswy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rpwqnehp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bdtnkbvh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nswbwjrg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xuethngj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mpxgdamq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dhoyolfu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rxpxozmj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dmkugcdz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2etcotdia.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kzvjvjow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgrstxfx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jswaqwqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oclrmdkc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hfyamvjt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qorwwzyb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2brexomxe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sstmoata.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ycccqtga.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nivqsfvg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xncxfemf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ecozcskz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2buuucnqf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ixtstqwm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bhjviqqm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xiqlioxt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vixiicki.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hqexdowo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hsqllgyr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2elbmtabk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2plyopitx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mxjysudd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2enveqequ.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2iutjtavf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktpmtbtl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2izsqhrug.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wczdmgzl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2vmxssorg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sflptorj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tetxsyav.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rxtkagfa.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xrvnmidc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nwzwbvdy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhmcueem.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzxuhady.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mowepjmn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2nzfhlsjb.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2amyvgmgn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pdsqwibd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2llevflea.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mespbman.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gpguyixi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vuluwims.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iojuruuk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wighvgsq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2memdhnzz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mcfmklms.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iphsjbmn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jeuykgut.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hzsabtgg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wscndjkc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lgnsvvui.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2auljtxae.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vmetiruz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rcgioqdk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uqfxkqdz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kdncqjkp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ljallikb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2kutyeqpq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2enexkztb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ddkkdsms.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2sfifwkqt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jmdyegyh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xtkymnqc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zwsqyxcv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2eqnjjknp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vjebpiof.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2skqqongs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2rqenlyrg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyiciuay.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhsclymq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjxewtcs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cgliejvy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2soaaskpm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kuafmyfx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oimoeqon.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kfwndmrp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fxvpxikz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zblbbcfq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jsmoxcyn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vdmabagk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kikskhzb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2unkvlrli.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cnjlrrho.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xuvzxybz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2whmeqphg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vbqxbhxm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wxzwljny.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gtxznfmz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2siguctkf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nrnejjna.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nrwiyjkm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2billczlj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sfhuzsqn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qpjakawi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mladnhed.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qxzmjpyp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ohpqnqrh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ylurjetn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mvqlvfzl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nsmvdldr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2exyxtfgx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2iaysmbmi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2afhiiyaq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zxvngntp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2cjguyhlk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kkmhintw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2skeczqmk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hiianqep.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xetokeiu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wndqbuhk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2srqdsvqh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ddoqhpaf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qcodzacd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhpcxqbd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2txcpemtq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyxswqdd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbpnkjat.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cqktrpev.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xgxpqkmu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tmyisbem.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2htnezigc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mqglsfjk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vdmblgou.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cblnhovg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nxgzntkw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vkfwvggn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lyjblhet.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zmchehuf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fempfkbs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahvvzgmg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qmylrsrm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zuhmfmpm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfiorufe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gncuvgsi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rscmaqxd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rdsddvsl.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hfqlallq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zsevdsys.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2sbbydull.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ppikwlol.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2jeychbtv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vgexlqlr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jutcpuzm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlbzwjki.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2moffwaqa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2twbwuoye.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oosvntip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xreokocw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zctjyqtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhiwvfks.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2grusxrlk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qdvzlrbo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vttchxjg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tysimezj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bzeyvecj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iriboinc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qgqpuqim.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jfwwnxqb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rzmcdvvr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nonjtspm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pymzodln.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2icfelhsd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vzvkkqct.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ginjrsvb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2agdduuwc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jahbgikw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2osscxyyt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qtrpqjek.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2uovssxoo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2drxdbwpv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rhycmxfl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vsmxuaar.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cbqxyuqb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wiytsfoo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qsgvcmam.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bpkyibnk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2omefnbmp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lrupefwd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2cporbnns.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2npmqdung.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ufyejaov.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2silegfrp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mvufrtcw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ygosyloj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ztqcgdyz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zimibaoq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wuvpgwio.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vgfqvtnb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oerrxmoo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jnuhdxdz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jhmkwhmx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2swpaadhh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yfqihqng.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oyymkumj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tknwlrxj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fhwhndub.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sutuiwiv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2krcdueyc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2blqrrbjz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2twpjbxpp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2srytxlhs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bvavlxnf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2piiyezcl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cnqiqhxk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2cbnaoord.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dctirfeg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vhssfekq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xqyiqotn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2plbjixml.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2udhvucpn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fyabwkhh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kwagsugq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zfljgkua.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2curpqoob.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jvkwyimn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lvrpzswk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ndqtfndo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qaekezic.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2patraxks.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ozafuhhl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2amlamduw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2stjbyeml.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ibxqnjku.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wjqsxbme.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qledfwqk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2attemryw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ozujhtlv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dvqrmvyz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ipmhyhtr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fqrpxvuv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2yevhevmn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rgpyewyc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2opwdxvix.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xbvedbxg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mlsgippe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2glwftuaa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ezclbmib.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2budyaoek.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jmraqebl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ivnxzkff.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2muogkkqc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2anvbmazw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2djlwjytd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2utrvmnsx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aflhedvu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2yqpdyoqd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzsmlaeh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2poigihzv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gqzylyis.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fuysfejh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zotgmeam.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xhzhoqkv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzdynwz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sztjmmpj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ogiykhjp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lexlrkdv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2buhlpfew.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2udiedyoq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nmupmjdr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2akgpfgfg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vvbwkjmu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wdorvhlo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ieubxhuo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cwpbslom.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lnhrizts.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2odbquudp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tsokkuqy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nqqijode.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hqevfjmu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2irouxcdz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhgtncb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ijisfpyr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dfvbrwml.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hsnukzar.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tdcmnxgm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rtxxetpe.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nxcbvfks.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2umgssrwn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mmyqyrbn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2frkrarnx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ywdcfnlm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tkksooyk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bufzwvio.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cucnunia.html


<!-- 参考信息 -->