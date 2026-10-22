代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2caemdvxs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xxjmjhzm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qkoxgnbo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2grabbijf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hlrqxhld.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tasegmcb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jzmavdlb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifjhaiaf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kghtiqyz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wrqqwtzf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcvdxjlg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yslcmacs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hnjieoks.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ohupopjz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bkkjoasd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2woyvcvgx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrgfmngl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmpgvpdb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwklfqdm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qsuljezs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2pqbxdgfr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2eycitwzn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ivvhpzde.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ibjtxctw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qqqvuliq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhrfnqen.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jmtmuddj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2vkxhauid.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2sepaoszu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fxnhiktn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2swgvssyn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2phzithjn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xbndirul.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2bdufbvoh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ymlzmjsj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nlmeiyyv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rulekjne.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pogjvzmu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ayufismx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bjoxxvzw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vgjhogqr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gmctddoo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zzfvshmx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vdazrfyg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vsrfiggg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jwwcxnwy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uxydguwh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mcngdzft.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2igxauhmh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pcorfcbo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ooxsgfqv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kerdiwhi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bsqyzvlu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zfeexuwk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pynfikgo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2implixzp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2flnafmdq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2haeozkva.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wygimtcn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2usukoeww.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ijfcynjr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iyjuubdr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zcoxpjmb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xsbclorv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hvrkdgnm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2tukcutvh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjchmooh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gjnwoeyr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2swbbpkdg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wjcbcruc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vxpxfajq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zjgfragg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qegtyawj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ynxujhvv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ginzhbsq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jbljbmip.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2eeegajib.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ahwugagz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2btncpyqh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mktyqwub.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mmthkcce.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fxqnlcer.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ewdseuus.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kwthhaab.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qafxcfyr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pujbhfkn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2kpltawdd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cespqybi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mryhpzat.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vdxrqjsd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ksobxygw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kapemphi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2qvqgsvku.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pemvbztt.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dppkfpeb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2krrxypos.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ayymwtll.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2btfijaqs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xqqhknow.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2quwjttia.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2otrxbwmx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bmugfyyx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zqgeokde.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wjbiobqi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qevvsraw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ncelguqv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2hqjojovm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nnibstbk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2awtpyuzj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2inxqfoga.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wsttpvuz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2supplyue.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2sxeqaxhy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oglyhiis.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aaapedbq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2moxeqzfs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsjvihmy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2chzfqhuh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2epowxsuy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fsyxulcd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2klubvkfc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2khdvvjxe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ezovtlde.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fktqdbpp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzncmlpa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcpsvvib.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2anpvywku.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mlebbrdx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xopsyvtx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fzplzopm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fxkpkwrx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nvixumac.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2meoxbihk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gjlemrld.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fwixgqsr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egtymlvu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hwvdtfgo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qrcrcqfh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2blqtlycg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2seboqxuc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2tmciuams.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffimncyc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eozrgclw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vwebfpdt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hqciecze.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dowperse.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cklchfzx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2tlvgudtc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pumgkxva.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zjceouxc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hpihswvl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hhejdadv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ghgceirs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zpxfxghi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ysnodbug.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ltzcypfa.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2sgkjprto.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2azdqdvky.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rmbarosz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jcepmruf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2esmlzuzd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cpqsfayc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2mgrvejui.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gfrpocdn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ddmkkgtb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vhhoqzwv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jubglbpe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dyqueqhs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kfwxayvx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pmfbcozz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2sbubiadl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zfbkzxfz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2bioctrnq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ybufodvv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rkvcxxap.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2plygopab.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dzspziic.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nvztfwpp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2fcixcqrq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uajkdiqq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gtoefkbn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hvglvwhq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pswvaugq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2afuxrear.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pmuobeaj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oswvokgx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2veytbaom.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jbeqlhdb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sgqxhwcd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2agmvjvrw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ayadmhfl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2moqjoemo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yloteqzd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqwoihag.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jgonfwky.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vflxfkua.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fpaebebh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2isxnpdxl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qkievvuy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wuxyhxcf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dkbfndun.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uzxnssdj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kapahfdj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fntflgxk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ozckiszt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2brjlflhq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfxaswls.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2breabjty.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2oczipztk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ountrvkj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2phyprffc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jwiqdbzq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2svxcfwdy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rdwhfjpq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nqheoixh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hivuyfgy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rukkhynr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ifietxgd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xpkbhenz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rcncndgx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2emkmhqsx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iaibdzbk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zurslpsv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wkrlxgnx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rodaaksx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qfxozhdq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nmaykzow.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ennxukpz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2uiokhbkc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2yebtncpd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dfshmygy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2wdpygfpg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cfkbreci.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ranyhamf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lgwqiyuu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ucjxklpc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mcomtrjb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hvtayjmr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zeumlzfb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bkffctny.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2radttqmy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2desrqlob.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jhzaqonm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kqazwsfe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mcbkoysw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2grmnhitu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uaudbemp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fckvsbci.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvcoopir.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2clublrxa.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zfssqjpk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2njkkqcco.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2lktqddgk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2epduanat.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2imjcwwpz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rmiuuysf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cejejvys.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qjsndfwt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hivypzwf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2cxzxeydh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gasxktew.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yztdhddl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghmmbemd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dulmgvzd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xkdbyiud.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zfnzkiek.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vkvkabbq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kmzxvpbg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2btiumkti.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jisqoqjq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zcikugnu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2icnekgpf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vxhklkod.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vudksfbe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2regunxfl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cixsnstu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2okeziafd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nohnxkgw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ahpkidjj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yiaxxojw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qdhnefub.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wdwzwxio.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tmvkzbov.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2koquhqin.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jpytpbpg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2bkautgfh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hhhxmthj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjyjknnq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ifppsejn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cicllecf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qokvvnir.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mqleeqzx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2umosibna.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2aqmazgri.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hhillepx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tmygjzzb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gmdbselb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xelsvisy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pxotyqjt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jbypkfvd.html


<!-- 参考信息 -->