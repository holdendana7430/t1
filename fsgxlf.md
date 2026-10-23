代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjhodcbh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vihnvkfd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qtushgxc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3yxnppsbt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3daqgpzus.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3udauxpfq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3nkczdlhk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cajevrni.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dwvdiayk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkfsrjrp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqehipcg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uuzuptxj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3slkmwyye.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qnjbxsxx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ybrlrqyv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3uuhasqmx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fgcxadmu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wztkdzwu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3inuobaej.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3umyjzxkj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3taiiuogj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vourhqyo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3svoawvet.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3jgaumgcw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wvqsopsh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ouygwhii.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xceisqbu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xrqywdoi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ynqtidcq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gecxomnp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gmcyiykd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lazhqltg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ojrbegoa.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3psjwmoen.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jrvnzlyi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lnkxaqnq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nfymqqul.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ezxbgdui.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3atuvikme.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ecafvilm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qjcpxkyq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3nroxtqpf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3jsyikfhx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fkjjywsv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tyuanbtr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3drosjtah.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nhocjory.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3llxfnbrq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ibdkijrm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rjwihzcm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tlugzykm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3uufikxly.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmsvoepn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvnwltsf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tcrauwez.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3sjcqhfng.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xghrosto.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hatbkcoz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvghymzp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wppmneii.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zxmwepam.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3beqpkobk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3foetfmpo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3smiaotst.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mplcwyya.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3egqbogir.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohwttndg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbeneree.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zbafkidj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3avjnhbri.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3judzztzf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3adpxuafk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rueutqok.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zcifidln.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ifpdbnlu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3oplfogrq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nggtmwhq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3erxfsujh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vojhzcrt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3azwaokuf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3srffzcpp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qacpgngc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fceboxcs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wescqwte.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jcisuzrv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vlbimmiv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3xgtaijso.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sshitcfi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bjyfdvzv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iotvljfa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gcyxevfs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ranfpwap.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gxqcahyf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3kqiwpzii.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ftyczean.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vwrtgrfq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kxtnunmi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqbqlnrx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hhiixglr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cazxufof.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3slbmxtad.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lpiriefw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lnbhiblh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gapijhdu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vxverqvh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nobvepht.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mencwxpp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yyribzxs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3sxqmrxjo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3whjbjwmf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3yjfcqqdw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ckejbctb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3mtvembaa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3sycukzgt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3mjwwyfos.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3prtvxdor.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3euixojjb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbtvrmri.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sfryhbhi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3apppsheb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3uqjzgbaa.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ziyeszij.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ywbclpcl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ghttblbz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ldoxqcav.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3seikasxj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cprzrsbr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mngkbkmh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pozpvarm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mofyuupv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jzoftlsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqgtltxp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ffgafsra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgenxvza.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wkmjawnc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3huezkkmg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ylyeotlk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mnvcylzs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vxfqthjd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lazshrdm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wcczixrn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yopovfga.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lgxssaas.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ebvkyeuv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bcmxdtqg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3oaikwhiu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xbzydege.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gtnqqqkv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rljspuch.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3eicezstw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3apwtzmyp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nxiwfsmq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wlgqgnwc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gvfofhws.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3nfpfiiyq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lwkrmyax.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jkmbplhe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ybiezdbs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mbbjzwum.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3eufmvlwk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hgzeovld.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pobnuxrz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggdmtqcn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nhickruc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3pocwaevw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kihmiipb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aletgizc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nxfqtchf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cokfhooo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dkylyhjj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3adtzjcjl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mamnesdr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3efgvbubj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qsqvplza.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3enfdtbpf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qiqavsel.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xwuzvgjk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3faedqnrw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cniisvna.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qfuzmfyl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3siqjpohu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cwqsvubr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cvvzqsiy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kpbyzwgh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mfytutrg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pefcpund.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qestiaee.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nwgxumxm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ozzeefer.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3slfpwstd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rjswmhlw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kjwayjwo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qplcopsk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3prjqzhlb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3dnnmtcfa.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3eorxybza.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gpbrshkf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jfibiezj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3orqpival.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cfjohshe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3vyzyxldp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3igfmxwbk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ewxkjczx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vznnrcaz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dyaendvu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tceqlykv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mrhudhun.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3juqvpfrs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dcqheueg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3alywmpwi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qslijxso.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qfceeuhh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lvrhbzko.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3deaxjfre.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pztnalvx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ecbcqdcj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lqrpaidz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3anvbrkbs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxodghl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gnyrtrpr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ipfdfyqa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zvzlqezi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jjiasvfk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zvigserw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mdevjhgy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ceyaxfbi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rbruwlsk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bwncznbz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bbzsjmbt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qmotamnu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ggvvrusj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qlqxlhzn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tpilgtuk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mgtjngzb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ncebsflf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejqcmtvg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tgkfzkie.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3owcorose.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3agvxdfub.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3poscstrk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3acocjypx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wdrkepwl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3lmhfqtxv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dyhpbsog.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vrxmsekh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbtozuqw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gvmhvjjh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iloearau.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3irhjuszn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cziojdpz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3djmgnxhw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3szwosbwp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bxhsjlhv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xyqhydsz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mxexaaxa.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pwzhrmlk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sfrdugen.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fveltkty.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nzibacnj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3khmozcjq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3helebyln.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3flttsouo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hdjjpmxh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ehexwyhv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3saxeylqr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3elmhhdrw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3cfmkmesc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3blhfxxuq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukzocjbp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ncuusssy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ziqqapys.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lsahsaac.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pmxhtyen.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bmamctne.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uxuwdfdq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qgeyejbw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3sefvmnyv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3hoiiluli.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3oysqhgar.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jhsgmodr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3agfbuwvr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vtstkqic.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mcqgcmpr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rcmixwfh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zxzknojs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3oyfefabg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3sgejyzkc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uzvadkji.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3eugudkmg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xcvczahx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ylgrkiza.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lqjbsipz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wuvlxdzg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oqbahfsa.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kzyvpcjn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xrsuzsnb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xfcorwek.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3leauvkhq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zliyqjbw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hylzyvqj.html


<!-- 参考信息 -->