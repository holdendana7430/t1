代发 wailian999

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2obpmgcdn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2irmntsjv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2glxeolsm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bolurcvw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zqrxrjdr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xblqkjve.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nxhbmccn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tkxqyahy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqlmyscy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yivjhhpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmtyprns.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zvyfbqaz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xxvhiuqi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zqlbqcpw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itjgxzpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hpenfvbx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ususdaxf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yfskjekw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dsepdzlo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbeyahib.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sypvnrqg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jexnolex.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bzqwczng.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2czqacxil.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2keiumqmz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ddkyzxrs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bmmefuuc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2eodtbyto.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2eitsoaov.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2zoqavhvd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ljjmwdxh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2stjyahwz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wvnchjwr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgivkcuz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jwcoipul.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ylugqdyp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2izzdhueq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gwmjnbmv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2sfgelzet.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2amjtmuns.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2sttugrko.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zpiozfnb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2iiqpyxnz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ptepjghu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lglvaoyq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivygcmnp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zckfidkb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kttnpsrv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2smzubvje.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rjqapgtc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2floiafol.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bxzcyeor.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bcfwflre.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fnzjdabw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qghxofyl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xjoodzwt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2plhqxjsi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2prroutmf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zdkhgyhr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2inrpkqnq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2onhbndsw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zylfxsxj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2iipzmhxf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fzpdohjt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pwdttrgv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fpnwvsxl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2prraxknr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qfiuwneo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xjigpsfu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2arfzmysu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqueedgj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2txubgvgo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ipuiijoc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ojkwkjcn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ctalwumh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2imyxtnho.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2bhvonmcn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2evuptbky.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2riiikjfp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nplcsbph.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mqqaoajy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2lodnsplz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmmepna.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2tskvtkzn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iyhsmgry.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dwwkvjng.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hfxxuxgh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ybhpotdp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjccbgsz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ovubzkcw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qayfxhci.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pisoxaex.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bhkaxsye.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tleuqgjs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hmjwrepg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2odidrmai.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dfmfojrp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ozswkkbh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2midfsgvq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2rfbymmqo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iiujtltu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2oepmyoei.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2meiruskt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2nkoxyzxs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sxmxrmnv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2zadgrygn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qwzwcuvr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yhcrdirn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dzpphsxa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2scxfrhyk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2rjcfcquo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2twptgigg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2neqsqqil.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bpmowwrv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wattfnfm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fcdttwla.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vtlgwfey.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2acengyse.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2onntznsh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2flgcudad.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gkdrtajw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfchoqjt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ahugcqrj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgiawqth.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rryvqlgn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qfxyxijf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ueszgvox.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zbiwqhtg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gfknnnbs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pkjcmukq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ceccfssq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jzjsoksk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fjolwdxz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2sthcnxqk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jsfydauc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kwmdcjke.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dpzgasqq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qbnaycjm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xiasqsvp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dnvibufi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2faqgyudf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyhbjqyl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2acigvbez.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kumgvzvw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2slocregy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hvyrades.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2jvfbywya.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gofptzcj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yuenfaln.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xygynezi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2aubfxlzu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yvekznsb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hdbphaks.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mztgnysn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zppasntw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzhtspde.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fszoapil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmkkdjtf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jtwdvnkp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2whnncezw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2asyiperf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ohiljaem.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ldneigbl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bvgfguno.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yjlahxqh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ghlbktdy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ziqevlro.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bhhvkpwx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wqyauiwu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2erjlzrsj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nyhicmen.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xkhhmgrr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uslpiuaj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ebhtyyfr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qqcqxvsc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2frudlmvo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2fprlbqky.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ykyduxol.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zjsknddo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jnefqdop.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yvtgjoqp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wfjhyrpk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2qvubkmdd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qundvcbz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fdkilfui.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkvrczyg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bmqjaabj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbezuszz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bgguqjkm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wqrkjrsl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ttqcziat.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2cfqnbbnu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wjtqfalw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dsaheqkj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2orfqyedn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2txroxdzt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rxlgxdce.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cmkyznjj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2yuwsugos.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bpvxubru.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yondtgol.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pcbxqmzv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zcjchsoz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dbihmcir.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjobyyfx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hckieusp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vjtqpkau.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nzvjcxll.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ntxhjskv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xaqpetar.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ldpkasnq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cwnflbpc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dgenlhmo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vdhpwhfj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xquiioxb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwmvvczk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nntmniee.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cbxalhgc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zxqltlun.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ihifmtcc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xlwodnrl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2frlkykaw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gkbtzxic.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bholpdpb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kesamqka.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hseqpwmy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2blkprumf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lwqbgxwi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2klkyczbx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ytvufqdr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2nigacciy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kaabknbv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pkjnmeos.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fisqgiuc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wmcuyddb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qehkihxt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zctqkezg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vuncgmuu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kqggptua.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rpitqapm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2clmgkxya.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ouohcpjx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yzvtngjz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vjhqcxsw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2osuouejo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2yvmxfsyp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cmaejrgq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2gtbqcdea.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2tcmuhugz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xvnpgrzt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kwcaawya.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vvdxweer.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dfundhqi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xupucqgu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rygsqjei.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2vnwbkyus.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2juvmftmx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dwtupkcs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jaanvmvm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ywugdqvb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylajytmy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2supgaaeo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2uxemlxzv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxwwsom.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kcdrgwur.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2yfyjukeo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2syewnkyq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gcnmeuci.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2anmmtqyu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmgexxg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jbrsgpsp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vpffmvpc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lddjdyfy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ytivhvzl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2unjoahdt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2sdtkvekq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qrpkotgp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ysaklzrh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2atywenqw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvsthhnb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ilsezgbb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jirykcut.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wbwgvson.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2atgmdmkv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hzxdnayj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aeolpjcx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mopdeszz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sdrvxaat.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jvhxifwg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2lfvbhvzf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dstvkbvb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ufpugyyp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2tzgdbham.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2jhwynqov.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uutxffkp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hpfptqwl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nqgjmwul.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2equtqmqr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dtpbyppp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ffclxzfe.html


<!-- 参考信息 -->