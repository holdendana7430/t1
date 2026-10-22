代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yiyiirim.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sdjsuvhv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nnnoroug.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2guredupf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2buiukvsf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gnzovnwp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ucovlhjr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kfenyvau.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2flflvpkj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gbthyghu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hmutrhlq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xvmtaieu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pukfuoir.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wudtzwhk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ktnpfemi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fmnudzeo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nvqnkdzh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mubqmdgi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ysyyhspg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tyvywqgv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2goxanojn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2abckcldg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2btxuegmz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cvpggocj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjmxyvbu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xcantyei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mijzsoca.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2taspttav.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fghkbgbq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzvarskv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hjrraopt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpxodzin.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rskpjtsf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dnoyjgxx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2chnluvhp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wetetpsw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2oalcaool.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wknorabn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssaptygz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uzbmjqfz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mokgwidp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ytvstoqh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2eubqeysb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ddfenmdh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2tgkzwimf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mjxdmtjw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2daftgyvb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2fmgztjhz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jqoatmcd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mfwczwol.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjnyraqk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gnxmeats.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ypsugggv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rajnixvl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rxrayaqv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pywildxs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2abstlurx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jtksduve.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2beavjzoa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2dcmrwsus.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nmnpjtjs.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dicgkacz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2llejmtzz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mmipjblm.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ulkiypkj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yjomnkhp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pvcjleoq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2teitkovo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ptksqrja.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2aogfhxme.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fdmohyox.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2elhbpmsn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rmjkuupg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xstyrduj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fdvycuzk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xvddpebz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cswqpjgj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rqwispnp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bnyklgio.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hjgnvkcp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2psxrhtli.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gbdyslvl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rwpdbuex.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tjxyvqus.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2clhkgdyt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gwoozswg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2kdhrlgie.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gdhvdlkw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qzrjcdqs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jlyuodqg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2reirojhe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ijqnpsnv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2semfraeq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2raamddmr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jslbdqsy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bfekrdsd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kjybduzw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2amcebfca.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmysrxsv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kgswrvaq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hwloykwq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbinofvl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kkhsnpdj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vqpyibbv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2evidhhbt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ctpfqwbf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bxpmrimh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2esuignjg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2duuzvewf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2othakduo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wnkzjkab.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rhcufjvc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2atsmlgsh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vlsahpfr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tkkvnjff.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mlyaoxpm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2alumrskr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gvoeymfe.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2osvnklec.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fxlzcxsm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vznqtgeo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ruxdpycv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ioyvahhz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yeerwbvy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jnfvifjh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nbtjspvq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2unzknxwo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tkpjywcu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hnvjrxkx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bpggvpov.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2oqznewpc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pdymsjhn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2arzkvuxz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2heetxlnh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2khejagwc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2runxzqrd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ezddmdgd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wrhflhyl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kqgtssgp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuzowdwu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dsvvfvok.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2llvopcdy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wjebjmmf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2lrvoentn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wiuefait.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xqwwapym.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vszcihww.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tjdcwyhj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2relnjhpl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzpjgbya.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jrltfcso.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ixqtkjtm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ulszvbpv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dnwhqzmq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qrmrsxdp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dgautgyg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wyhgrufb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rmjzncvf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oyuoxgnv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2znzonffw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tkviumpw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mbiggcdz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tdvstzmi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hxeuusgx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hsefelqq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fwqihgoz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tvlpfkoz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oomrpuzm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wwcgzmll.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lmzsjugo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qkoagboh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdhndkoc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rtvedrsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqwdhoaq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mpwejwzd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2udrllbpe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2blaoksbr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2siuomfwj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cafvulrt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2atmztqax.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hlwownmf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qkzdrsmt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2mllnprcd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2odncmqst.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tebetyod.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lhnsgjzc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ggrkvqjx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nsprwldy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ujyzcrak.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2szdumxcx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2khwpbmoc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ucgdmslg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gbxjgfeh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xgaqxqoy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qjmaijhw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ultdygjw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gitgonay.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dyroojub.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2akxootxb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rwyfrcyj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hilxvprq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ziyisjbh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hltqmfbc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vnrgemkx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bjaisazw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fibzjonl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rcxayhyx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ucyedrqi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fcjweons.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2cvhxkoto.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2elwkbcvy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ryrwxyly.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2otutqxjl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oimcfptk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hfnfugoz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2upamlbjf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uwyyaquf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2whzyfzal.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hlanhovk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bfhtuenf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gnuacauj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ywoaqesn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ozltirjh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xrqentgt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mdaxncjl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2acuvuode.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rsukckqr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nisejzaf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dbhefavc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2shmufsau.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dfwyudze.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ostjocjo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2acjzzpsa.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ytexromy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xtiicxdb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jkhvfdfd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rqcxmfdn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xcptdrpj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fcwfcxwg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ynagxztc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2comhzhdn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2cbloiihh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fobuxdyb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2gvzyhtvb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tdasvxxx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2frrikfuy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2htlzqmfs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uqthswqb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emqlnvuy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sijkvxus.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2uwvqarwg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ixwebnfy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jkzxexmt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2busfqxbg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2feankiyz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ikoextjs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kdatosjk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mcarhxff.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ytmwpdlv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rwkavkng.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dfpehjlz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2aowvjouw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2khjyitpw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2izypvsui.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zaxpupzu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2egnmlshn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ugluuqdn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bgwzuejk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2knrmjanf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vebcgots.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbmmxyxn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uuddkbdi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hbmkopck.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ywxtbngd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2otfqoyws.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2srbnqgsc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ikwycurs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xrkolynr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2njlhpzxu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwowbpwl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xwdyonkc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ixffporb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2cbnmdpfq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jcbclxyq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bhqkgltf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zhhporvm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eqhqdvgx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wtquwaej.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wlegzqet.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2fivfggaq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dfqfhacv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2thafinyi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dbfvjxnk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2liihnvfz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2apzchmeh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ygizqnrv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vuyxoihj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pgxikiie.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tqfuhdbd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xnfogqrv.html


<!-- 参考信息 -->