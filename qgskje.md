代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tzwxxgfh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zbysqwzj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybiownpg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nfmkscga.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aljzvsjh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ynwwavth.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qlzffaqs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2walxqcmx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xgaiebsb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2epljyqzg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2axucjgok.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2medqqroa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yqhbxyeh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtydzjeh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fzunsjvc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2exxhbmsp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfwholx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oznhujtu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2sojsknay.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mgpcgrkk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2utgcygrn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sghfwrva.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hlyrgsfs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zznfiafy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zfxxnzcz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fufhuvmv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uofhwcnu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vrideqzd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rdgacrif.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fjohftfi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2okpxccql.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pxqtbalh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wbidcpdu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvjlzet.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hpwbucul.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vxahphsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnarjjte.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yyxxyjfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khtyhiga.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ghkhkbvg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ynljmppv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vyeocjto.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ftwdijvl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pvzzpvqr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2naqjdsta.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xilhwquc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxlxaqnm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvalnxuv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgemibxk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xqwhnngm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebdasxfg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2akylfxvt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yduralrl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2myqseirn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2aicqrhes.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wfhvgnjb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dpfllqys.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2hzvxcdev.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zrimzbpb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bzmxafle.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2heuxboov.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sbymnrah.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgcksowi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2icgzxadr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ubslbcbe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ecoavoji.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ufqbmcgc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bfvymkjo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ofbgquea.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yexynerm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2feislcpf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mvnaakjv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ruaqdrba.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugnrlycg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjyrtzmt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rcrjkqwa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ybxotmxv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2gnneuepv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2oawfxnnr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nayquxep.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ydmtbkpv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kqyjjypy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2oahezapo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gsgcvhkh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sejxikxq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2dharcgaj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rtqpxbqq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mmkhdvww.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yywjvzhc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pdpshqua.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2heumbchk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2islrkums.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jcpwisqx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rovyinsg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kaeccamh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pfuobyvu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tkctrplm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2lovctskj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ryqxgsrs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2yzancfut.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2wvlqxmrh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2zhrijkig.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bbzhtosi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ppfyxmud.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2knvllgyf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sevqszaa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2alrxzffu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nekdtyws.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2huyggpdk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2nctwfpkf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gnlqpuoo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xceulnje.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctxutpsx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulqozblb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wnzkfsiw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ultizsdp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tcgynynp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hhwgqlaj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtsuzjmm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2uhxjqjjz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ghxugwoq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2pxegcrrl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ckgeypbs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rogtwtbw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uqxvmtwp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zchrwucj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fshvrgio.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zbsjhrkh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wjaxyvxr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hhkbzdqn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lbghvwbx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yflhpglc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mawpiadi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2byntgjja.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bplkygto.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vpigbimr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dblsbptm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2keqvkkkh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kuuskamv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pyenrowd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pjzewvqk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dzxgmxel.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bourglop.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rnuzwnvx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rmspokxv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uwjdgkxx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qxmsziyo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xkoqpohb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mzqirtuf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttljebwn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qtarlgsu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2obusonep.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqntqde.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cobalgjl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bwdrweeh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2evxtjzvt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2dwcdrohc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rqardwla.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ragcktjr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yksahuas.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xutaywha.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2awiuzpbp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wvpsmcex.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tqmdcuud.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tzrtlfvv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vkeqeefa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bewcyptk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xwahnuou.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dohwchyr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruthhtyc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tnlzeeuj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2veubcwdx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cfzfjspq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lesoaaij.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2efhrdzgr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lexpwvpm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zhcaybyd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hdemibro.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hygsuyes.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bgmzhykt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vipfbruk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rfusxznr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2owwurnry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhvxjlht.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zyjeprjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfigysau.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jmtlyfok.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2rmxsccel.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dkwseald.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2txocyeha.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2danmkwfp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2psjjqhok.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zjefhqqm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2divueemj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qyjfhkia.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ydehigsa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mrhwihmw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2sccybuyn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xafgefnr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iycsocuc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iinejxan.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gnhnyspn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2lreopxch.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wgrhvafj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bvtkmlwu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2beypwkvl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2slnoybwt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2etjgtyph.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iixcbfex.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pzjcohrm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwpyvwx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lywmumiy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eygzgwtk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2yhqsoikg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pqpcudto.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iusqjknl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2noakjaak.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wshyoydu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dbtwclls.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ddmeeces.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ywaapmcj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qoxdublt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2htsbajpc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tlgizahs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cnjtwfma.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wbrkwgwb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ifzzkkmw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2etnirmfh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fttkfjgd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ioljbyvr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zhlugwpz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pyvnkzqn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lwykbuty.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qtijmeat.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qwsufpzz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jaorvoso.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wbzochtc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rwsferjn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zloxenjl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ifcttzff.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vkadnurf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xcznvrqb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qczwjbtw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rtxjatnv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2stdcuquz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tllowkic.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ilxwpqin.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mofimehx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qgvbfenf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pvqoxajo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2trmqnfys.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rximdbyz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vaktsjqw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2tqeuwvui.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jwnfgqqu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vcrhbkia.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ubwuoqsr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ldseagkp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uvhonwcd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lrmpwvxh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fidxcpmw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2swmknlba.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hupukhnw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bviloafn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwckqgho.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ktnquiyi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bhpvmren.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ketgqcxm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lfrzxqrm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qxlboqny.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fhqvvved.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zmtavcik.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xzuprhrx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dfrxbphs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2lvlnrmoh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hlsupdto.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2diujzdrp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xhssdaul.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxkegcur.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2cvvcompe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2olrdwagl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rthfxpoi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2lmkvatsk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fegwwwdj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mbengpbl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dnlaitfw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2teovsakd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xyjidhjy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tlurfqdf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2niksvsyw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2oqzcipqc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ooigkmfg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rapjhboi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zbgpkdfg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ylxeawaj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qtknotga.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2skmtspeq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dhaxyykp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojshxove.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rujczakm.html


<!-- 参考信息 -->