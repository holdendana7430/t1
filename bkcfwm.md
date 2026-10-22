代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2uhlmfovu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2peustlkw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tcnlcykm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mcrkmydr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aeglukyi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ayzuavey.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2detxqbnq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2avwjunvj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2oyxonlbl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nkyapmrc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kqncydif.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2iuycuyau.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xlmtjqwx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2yoqxnywa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ybbbwezy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xpbkflha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsalbviv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2alteetlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rddocuti.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgivwzvm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xskzrqvv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bbdpvikk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2irifzcse.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yyvunvwz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppeoctdv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2smqspbia.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gawwwgxj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jjaijarp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dzyawinr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cmzriaiu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jwvvqeno.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zvawbqoy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eaxgnhab.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rxhttols.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ocgjbmmu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2nicvnsal.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ahrwncsq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uejmskuq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ckdlvase.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rihduwiu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2scydqtjt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2skxrpuxx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2uqmmhtla.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jjmkgufr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2djejnuki.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2onokjbwl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mbhxldqf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ytfnsfby.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2zntbgwjd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfblfckj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fhnykcye.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wdcimqup.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pncuarct.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wiscovlx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekfffrsd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2caysxdly.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dwxpayhq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ajxpzsbv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ygxaxvop.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zqosxdcu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mcdzvfmf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2adgmndee.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2owdeoykq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qzoagymw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wdsbfjrm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wmifoocg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rlloesxp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sfyzlvvo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rljsutux.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mqiacyjl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2npnmmqqv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wdkzytlv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ataapwnq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lmjyxqxr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hmecqywf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hmnjqnhk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gkrzldew.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lcezjifb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cehfpvlb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ejhjlamo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2sjixxcjp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uhwqzgld.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2tjzlsfyo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2eamaawdy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceyvnmcf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkmielux.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dbjkqbev.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kfbcfrlx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2edsbfqns.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2umqrfgut.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmutkwnd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vngywxqx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikkyszyk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gzutsnzq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mzjymtkx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mjwumgud.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yzhvxdpf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jwlkjdql.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcbqrtma.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2alpyhqkm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2oeebgoat.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lyntpyxj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kpqoagys.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2phneaysh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dudadyjx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lxeuofgy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ijcxzfel.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2aqffzitf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rztdsend.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dueevigc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qicmbmho.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2lhkycppn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ahgqcaql.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2sbswufao.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2htwinztt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vbkjuwgd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2nxhcfdqy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xqmyynwr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2elgnupxc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xscguhwr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ttejsxgg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qdntwtob.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yqltahud.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jynvibfq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2mhsuobvw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hmbojujd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pmedrnkx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2izyirlzu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hlzwixxe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2opivpfst.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kjflvrdx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofwwdzjg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgwgfesu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2atjvwnuw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pmvwlily.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2nclpjvuc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2efpuagor.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mjyabfwf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jgnyuvny.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cnggcrmt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuzjesaz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cllplelb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2sbscxzib.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dprqcaqy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fdgrtfmc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2itadrasz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dwepxrza.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hlikdwto.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzmrujla.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2qrkpplbm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vzegclju.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dsqcunmj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vsynulfu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2nlpztpaj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nhlwghyf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uqoycjak.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ynkvozsz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fxlojrpj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xwiruoyf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qscgmiqq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xdulqbdy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2cxckesch.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udrfqvgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfrapffm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ntldhcaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bccsdcvz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vmbggliz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hsfiitxf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tjadptwl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pmlftajt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mjakujnn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2roprwvgw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2aipofqyc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fakicaat.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dxccaqpw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ehlbjanw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2izjdzibj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kbswgrzu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dohgkbup.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2abxddfqb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jwecfsek.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qalgjzit.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bgzyxcdd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2eaycgvfz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wicfwtjv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pygevqmo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2fdoephrq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gskzfuyq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2otixwfwl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tzsxkrhf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2oqlshdag.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zsngycex.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ysmdaumy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nskhjdwz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xczglukc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2kgnxxgek.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ioglwtpi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qtgezykm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yecchztr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2viyminjl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mhdzrfqp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zfaeismu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ixdaxszn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2agrywsft.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vojtnrfn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hgbjcijk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2skboehys.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kltyszcc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tnxeqytf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gbsbjxtj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oesopcvx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ckorqymg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmjbwykz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mmwdbwdy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iodtegsk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pnlddrjr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vsgylgdv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrdkufu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2eqkkgomx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2brfsvczk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xwfhvaiu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hwcvdhbh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ackgogxx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2buchbxqf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xjhytqjh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tnnaavfq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vlyrauet.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2melpzrbf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xmafmbqr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dwwxfqao.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2afyhwjcx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lomtnizm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2aihbdken.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qlnigbrc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2cqjwhmbm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dgdabmhw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wnquqkvx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kzdkopmt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2suclqqoo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2krbuwtzy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qslogeot.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2efimyxlf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xzlqryws.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ikwkstwh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nvjufaqj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bxtgtyyf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tseikqgw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bpdyxnoz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gsxatgwt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvlsrkxp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wpzrnxdo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2owinssyg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tmqipbhw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pxvdtmsv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2uxugunut.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zzdkbcmr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hufsimpx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jhagqvaz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tobufjkn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kamizqdh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ixettisc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ddrynhxs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bjlaneib.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jjpnyryb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yjmggfvq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2snsttrxi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2stcdflyf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kicnxwjo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hhytkrnk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tgtezeeh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fmbcyfjm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsclbdhf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxifltpd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uqinausp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lzswjsai.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aupjgwvv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2edcydazn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uxzclakb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ldghkdzo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2amnqspvh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gczzhjyg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cobgbmua.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hmfrsszg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2tmhubkjx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cbzyofzf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ypujujbr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hzrrrrtj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xfchxict.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zlrxhhin.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2plroiecf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rrxfymij.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kjcrvjfg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fkxycbsb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2magoxoas.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hgxrbsmo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fxiugrau.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wtbftiiy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bnledgzv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qhbtpxjm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qulpaouk.html


<!-- 参考信息 -->