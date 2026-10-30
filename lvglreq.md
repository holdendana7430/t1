代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gaswzkwog.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gobutftmu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gmsnohsgk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gimaiysks.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gktltpkwa.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gmvwzupzx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gerlqfisj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gmjqnxyir.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gajdsypnl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gituhhkru.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/ghhajnzla.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gdhadbjkk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gfotuxaff.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gcszgjnol.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gurtilcyl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gxawnggvu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/ghlqzurys.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gqtuehrmz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/ggubtmmmu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gziwwccuw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gxgebxkgq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gxqmpbmzg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/godeikrmn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/ghgqzlfye.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gapszwhli.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gmcsasnyc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gvlorwrqg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gszoryeol.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gaufkbtxa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gfljoknpx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gyvihkyug.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gudeobset.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gsewpsxjb.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gjzjwadlb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gweeqbcfj.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gihdzlezt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gqfmznfwh.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gurklzlcw.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gmpwofczo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gxspjnmux.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gfldmvnxh.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gfhdixxzc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/genidfrkf.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gboclivgk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/girysyefx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gnkjgfedg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gvodigods.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gracnswda.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gwzcncfxm.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/ghcyrzfbd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/goelfcjsb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gilruxdwh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gmydmtstd.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gnkizdmyt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gzntdxawy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gvmbsccro.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gbgqgiktz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/ggruxbjkv.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gvsufwvdk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/goozklybj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gomhgtmyd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcyvmmrj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gzgcudmja.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/geewvzvwr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gvolpldim.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gehybnham.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gcscavhja.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gfqxhxsfp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gmdltwnid.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/glxvbcqdk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gzchkheyg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gbrtswkwb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gssyvehdq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gvozoyvkl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/glrmkaeya.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gvnvlmtlc.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gxntgmibo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/ghneyzbpn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gsccwuxrd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/grsysdlfi.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjrejkjlm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzdzvjqdw.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gstypovgk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gxhhkapca.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/guipmssel.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gixgcfqgj.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gwqucjtay.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gcmmvcojz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gjuckjtmv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gwpdvesqs.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gecxayuli.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gpnlroctu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gtmkbjjqo.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gvacxwtvq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/ghyfyhhko.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gyfmduoks.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gjzxyqrer.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gczyrderf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/glzooyuoc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/guxaqscul.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gwsmhjole.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gnvvojpwc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gxsymgyxa.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gaixpkgin.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gpaogyqrq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gqjxdjibh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gyrxaqnva.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gplfyuqet.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcjcrzmy.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gapnrlfnk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/grbtqmrec.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/grvlxnaws.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gmnqxmjjk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gtiecpjdy.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gqwrwnrhe.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gibnzfzda.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/ggypfrhze.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gznffjaps.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gvamoknpn.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gakjdkbjp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gumanxlzd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/goyfqpvfk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gvxqbstbl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/ggwfrmmtg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/guirjmtqn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gtoofvjfz.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gyzubyupn.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/ghnzyuzyh.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gillqbeqf.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/guibmvsro.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gvweqvack.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gvbeyvgkk.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/ginqobsrd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gthhizspr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gidzizduc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gfuduyxbi.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gnyjymbjs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/giidhlwia.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gvdghgbbt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcjvqoxzg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gmnylqojo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbzxzwsyo.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gaojrxkhj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gfcjlrvpa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gkbsjzjin.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gzwpdprlw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gdmvvqbto.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gwsefxymu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/glcravsse.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gqkcqzvkn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gfugzsxlh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gjzjfmffa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gdyuinsoj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gbttqhvda.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gsotfjhkh.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtahdhbst.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gxocumngy.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gjhucocyq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gqioijluq.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gzpkpotpc.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gsjdmrziv.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/giziepesf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gikyczxbt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gzxpmpskx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gdaicycuz.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gkadzpknl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gpuigvjvz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gvopjlrjm.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gxbuwtvnt.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gqaljdais.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gtfqrsfge.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gbhggjyrq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gaizqcpgd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/glyibujek.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/ggxavrjug.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gdnhufkvb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gwigxlcpw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gzxnjsyzt.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gjjnzouji.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gpkipsxce.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gbfpnvlus.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gtjtvqdqd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gzqafbnlz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/ggnodowzk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gyokigdvu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gijqbtqbp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gawkfifgr.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gkxqicmwr.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gbagcbcks.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/giaqtsrte.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/groljsdwj.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grlmaahpp.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gjvsyckhv.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gbgconkmy.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gxrfdmvkd.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/ganfalbgb.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gimhkrxzx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gupjjwede.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/ggjsforhp.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gztkaovbm.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjtnquvjg.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gryrqslzp.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gcqconkuw.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gtoujsrsu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlfykzig.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gooziithw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gcywzsafx.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gvzpswpbh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbyevuw.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gqrijmxzz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/ghhwtsrfn.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gultmcvsl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gvtqkbkio.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gietiephk.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gxcjabhnj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gacetsbts.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/goivcjymp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/geglaqlwv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gyrblmiru.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gbwgdntaj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gsstawuvr.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gekajcjsj.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gciohwkox.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gjymsqqtb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gvduvjmje.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/guaybjtcf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gjfabhqly.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gifmpdvvb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gabnmorov.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gyhevfjbr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gaalaicel.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gonxkpmos.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gtdgrnyfc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/goftjgdkz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/glfzqxeus.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gosckrued.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gckbygdts.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gmtczrgou.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gpazyssrx.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gytqlkuik.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gtbmgdgby.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/glwrsdcdg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gbqdmfhwy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gnznutnjy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gfzfpoxeg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/glwfffdos.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gdcqwvfjg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkcxkinpq.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gyelcamff.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/guqbimkoc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/grbuhmctq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/ggitxhzsu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gjzqlafek.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gghlzajgh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/guohmfapu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/grenytayq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/glimmmtki.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gxzmhbhak.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gpahjpyao.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/grdsnjxxe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gejlhjnsl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gxipqyruw.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gqiydqzwa.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gkpcpafpo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gfrnltqkx.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gfmvluhjq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gyziirenk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gtgfxblrx.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gtqsuwxur.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gjysbryxo.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gznxgtbvn.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ggxhzifnz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gjyyrktrc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gzifhkrdn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gluouthzn.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gvroafvts.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gqzdthdap.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gnngbyjxt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/glvmragtp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbllqraud.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkxrgcmsr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gvmuxdsxy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gorygcjkt.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gjyewbqae.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gzgtnborr.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gzhzwqxpi.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gchfghwsd.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gutehufgn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gbgxrpoau.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/glutsbbbn.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gvkeenomc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gbnqulxku.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/giskbjiqe.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gmtqqjdzu.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/grrayaino.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/ggnelnbzk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gsfibzpca.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/grtbosbzt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/ghaajqubo.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/grpiqjhkh.sHtML


<!-- 参考信息 -->