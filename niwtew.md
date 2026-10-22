代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbgomchd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rgtpwkcm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2hesdbvqz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2voifeoba.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2khajvjyn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jejfhmha.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ljzeosli.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxevaams.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hkpymoab.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2engkuzci.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2veebtaob.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nfxkfizy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nccewiud.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pbbelkrp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lmiznzps.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxritmzu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fabuwsug.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ikadugmb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpevqaip.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lqgcuhoy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2dxpsevme.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jnzlrfyq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bktqltvg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cnsdzeky.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wwoqddnm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xufmapmh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tantzfah.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kkmwwvjn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2drcmdeob.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2afwouzxo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2chqjsisv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2mkrzufvk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2drqlmkxg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rkcfcevl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uqxxksom.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ngaqlzkg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2xhjtdcbh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2smzjhrmr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pziiacnx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2awqqndrl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wzvxbeyf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yrgtekru.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lagqgaro.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pkitrjpu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2elkidfwc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2czxqljzh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gjkxxuhq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bnaobzut.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2immnivuh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mstrcqxs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dglfoprs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eaumviyh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bxoigvnu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kavbypjv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dignqblt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2iaymhnqn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jfjwizrf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rmswojqk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2iobmhvbr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bpuunwln.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuzesezq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kxvsovjp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqnqjxwi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ywdhurba.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2afeerzda.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2tosaphzm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouelcfzb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zskkjcwk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzydanmo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2exctymdf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qxzyefwv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uhjyaepo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jxvritef.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ajdtuzja.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ascfkadb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2heelwgmw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xaeogvxi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ddcnvmdo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2dnkjoqjs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ctepvivy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xvfncplm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cmxecura.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lrufwxcd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zsuieesg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bwpglsxv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yqtlsxtn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zsojxxgf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2swvjtdqt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pumiamgj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2wqwwymgo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hkesdesp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2suzplswo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dsujnopv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ocgpckwa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kfbacqps.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2urqsizry.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sglvvseg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xuvqnvvv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rjytfsvo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rqjcqbcx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2omhjwkzg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xlsnmktx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2otzdnzan.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nuxwtqhm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zzpcvalu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bqjxhkvf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2izoncnfy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uhzaoxfu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zadpalqz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2tuduonpm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2whlkjoio.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2piqblifj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2lxclecsq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rfplxvdf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xwrguwai.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gjhrnlnz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvldanzd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2utezyedp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xuneaiot.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2obyidlbg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2agccatbv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wyerepeu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2geqfxdse.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2jwksertf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdvdgzjp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kwlxkrml.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nwebtpwm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yksicsqb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jzvhtbmx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2sutyjzpu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dhswqlke.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wfquceii.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vwfkfops.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gidikibu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2phdoashx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmpaawmf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ooncgovp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgfzcfza.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vieuitcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljzldomj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2grtrfwea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkajxiza.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hiaaxmhy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2pgvkaylq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ornsemaa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cebybowm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2iabvwdyk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hiouwfyi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2sdyvirkr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rfcxvwev.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gzepqjzk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jywlvqut.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dasgfydn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2owtoiznd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yjhqekpa.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2numpotod.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kikxfrio.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2knrqsdbb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rtxjuigm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lnjaxleo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2iznibhkr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mxgqtkts.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dwkwenju.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2oejvpiqf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2himqwhtz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fcklxazf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qizlvdtn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2hymafngj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jzrixkpb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wivqpswg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mzwtdbrf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tgfsyvrz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pabgvfyr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2sasyvawi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qxhvstdi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pkzeelre.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xwgnxvlv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pblthhip.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tanicpcm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2babahwlu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2khlicols.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dtvasypl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nhgpgeie.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zmraqvhc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ddprxtuy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hlrqzyhp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fjdwfdcb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2haslkmgd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2whmgjpfc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2agotdeyb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pzyswqkg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rrrisprb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2pnzqdbpj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2finkiote.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rhcypzos.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lyzbqolh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bfesqxbs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2mtzxuxpk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jownjpty.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rwnpwnyx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ecomjwzm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hhpgxkmd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qneczted.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tzeeayqv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cvpyylqd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dmsybcjv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rplrwzvz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jrnehwxm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2azlbuapf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lgwcjuru.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lixohrro.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2cngnxiqe.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ggnovmrc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2epocqiyt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vwowegtl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2becadxfh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rouqckyd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dtukoqti.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lqfxydgn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2triwkmhf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxegcbue.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2btnyhesr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2azekhbxo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vclazage.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dpuzvvvu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ssmtlysk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fdfoopgu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ebzknlva.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dphlbrvn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2npoexklm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2litgtrmp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uvmwbuwc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2uzgqvzef.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2avlemuhk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xqugksiu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2slwbtttj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wnwpjzli.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fhfywglu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgrtopyx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pjhjtkuj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2bgnfwdfa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lezpbraz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kcghikcx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tftdyetx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mwzvuoeb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2proalbew.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tfjlzhec.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2smjtkygo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2llpknwaz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hyuhboah.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wvqqcxjz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ovliybpa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vmedxpzh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zmzgubpy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2egotvcjb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wayckdqm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2meavxcvp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fzbaashp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kzrsoqdx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ewnpiedt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ybeujzpr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fgbubigy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2atwvgjjm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tgcoeino.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pkaxzpov.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fckidqkj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dykdgsjo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hodwctkd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nctgccyz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yotaxdky.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcikabk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ktnavtzg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rxejgrux.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2amhtotav.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2heblfpba.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wpjyfmhc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gghvquvf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zgrxadmv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ulnjdrrh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2encxtuii.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zevnixqs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2npqfddhw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vhehrmfe.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cjueqoci.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2afoqjxyn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2icviqllg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hugtjczq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gdaczvvx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujqphqkc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2syrehyin.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ycnetgxs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rnssvkky.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhfvnbqj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qcyxvnov.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ljjpkvuk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kiveomny.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vjqgadjk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cxhupsfx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2raptgywm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jhweiwhr.html


<!-- 参考信息 -->