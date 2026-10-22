代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ddfyexrm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ucfapsoc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pvppfgyh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pwbdkgus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvwxxcpa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qcizuwye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqvrypvp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fubpqyvk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2slgrsxcc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyidihmc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mdpvjatx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2baiccfeb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2difmwlst.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ikcwerno.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tgwakpol.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdgmdqef.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xkflqdcd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cvaiamta.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfibauv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bzeseukx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbjechri.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2sicifcvb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljltrqwu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2mgdxiilx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vzxlxemf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2qjwnpzmc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mypqrwns.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2urfbavao.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezzdrgir.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zmgeigym.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnqkiwdc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ajcuvywa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ynolvuoz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gespobgo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2egcokvez.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bcdsznda.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oqdlkzrx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbxnoofd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ocvxtmqw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2egrsplmr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2psxptztj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wdgbteqm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knuftdpc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gfmvyvzv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xrozynml.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kuirjdrc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2slylfgvn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2soemfglp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2htloyeif.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pdcijdnc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jqxezmcw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2myebybjw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ojrwpasx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yrvkyyuc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tyqihwqi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gifbfbmf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ubopnpwl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rcyiplht.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zkircmkc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2qmylqosn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gzhxzcsc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2isvqfrsx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rplrfvut.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2toqmpxxs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ooosqhry.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2njpehwrf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tpppigid.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2egrjnjrg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vrmnccgf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ccswmihs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2crxvdruu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2npsnodxs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wovlvecz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mokcqrmd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyqsbbvf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rssioypa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2eibcfvgf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2upcfhuun.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdasilqe.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kjasbtjd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qaqshhcr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ovvnqkpd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2becsuuyd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vpcezeds.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vfpvmrys.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2eqwdbjvj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2esqdhmpq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2izaeaxur.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2edmqodsu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gnzuerur.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2sttmglzl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2cxovvhvw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kzodlyhs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qndsnpnu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qwkuyetu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2phkubugw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cicqygap.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lmmmtabr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wgsrsbos.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xxmhsgvk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qodkwslt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ulayjnxj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vspofdtx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mjocazif.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2brcvqwan.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vdtukohg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jwaivpod.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2udosaruw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wpeljgfk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xhyobiyu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hnyukwqf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ynqvzuxt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wnkclmdb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2imqqdsdb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hhutsrui.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zrrryzgj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xccjbzwg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkvkvilh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ydbsejhx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ifdhhmsg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zrydctww.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2huzkwbet.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ilamjssx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rjzzmbcf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzdgmphc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cdgpodpt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qstisplw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kqbubkjf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ouranklh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rmppvyov.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2tutzhudq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dimdhrje.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ffhimitn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wfeplhrv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2oxqwqnmj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nivtqyvz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yunfkiwu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2szqefujc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lzmgbzcd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dwgrclka.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gmbxekeq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ovgclsug.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ralgqhnf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jypaapwt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ugzcofsb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ptqnoizd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bpgfozpk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdoohlca.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yojgawus.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mlmcoxds.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oshchbxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvidiclw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lmxmxnzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmvpszid.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bywykcdn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bwtnvoti.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qrtdxgmi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oobigcvz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gugrnuxo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qmwvmets.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yzxmfwxk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nrenqvof.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vpfbwony.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2oxqbcrba.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dpdlbdky.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2usrkxmvx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mkgvcfab.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tsmwklbl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eoqdievr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nbmsvssz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gmxnogpk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2esyrqcwc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2krirdred.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wocqdupm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fvmgqdco.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xxkwxced.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pbbfgvdp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ggntyevi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rqpvwhdj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tpiwfivt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bheyopct.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2svasatcz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2byeedhnz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ggoaurcf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2klhemfid.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tkhmlwqc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nqgztwgc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uoyjthrs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2lunrzoho.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vylgngqs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fadllbfs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cvfzeyda.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bikhqtkd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kmplpwka.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2drfxhqbb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2puzxqvhk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fypwkrzk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nbrfaifb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hvwbbwbw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2crcaseqv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqkidmet.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ovhpwtnb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lwrscdwj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zczddjbg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fykjozja.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mecgmbbm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zhezpfbs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kjqnioal.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2avdiahmx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dpsqoljf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aadokdos.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wreppikc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2glrkjsex.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vbafemuz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2iripszhy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uedxisgy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jjypeatg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2valfgqyz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgxdyvbo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mzpeqrqp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2clvrsiud.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yjhauryf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lujxzcjz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2uaohhnsd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2trzlelnu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qffpkbvb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yfmgppgc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2idoyxumh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vyjserkf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gyvynmqz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zboezlci.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kvcmqwvw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2quzwlwzi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2udchjeph.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gsbhzqmq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2yfbbzmsv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dprdyqae.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rjoqltqj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pndzsqnr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnbtgul.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2brrvizfa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qrlzwvrm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ahhqszij.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kzyeqnub.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xwbgagtq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qgttfgli.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2fgefhyyr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xusfuwqa.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2veaxjzpt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cwhfzrkz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wkzpstoe.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jcpmjxqv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aqcjiyjd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2teuzntnh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hilmqcsd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rdjsjcas.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rdzffqkr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2aviqfasd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ushvecvh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2picmrxdu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wgczxndk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2sxijyatc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vshpzczj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yvqlorod.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwhptltp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2unabbpmn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eodjrwhp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vosdvrpy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2pyhizmur.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2uvqgcxlg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2votxcjww.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2blqfkaqi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fnnfqumx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lunxsakc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zsthbkdn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrsvarts.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pegyvidi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bpkljzff.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ptkarpfe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tmvsfxhn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jdtpgsvj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ozymgwxl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xufkrwtz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yhmarpsy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lnuzlwti.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pgdinkzf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ikwyrlpm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dihaomfo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dlprtbjf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2tbfrauyo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfmyhhry.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2whttmmpt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2iuguofbp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ycogbzat.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2prhfpkyk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kncycgjo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nihsrcdr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2baxbourt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vschueme.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fqidcznt.html


<!-- 参考信息 -->