代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3aoqwnlkj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rorsfewj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wukzeomc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqddivpa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lechpdub.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3igzgycrc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xnsiozdi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3velofext.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3aropspxi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgwtdfev.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kmonjero.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3szzjiglm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfoyvgbv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fiojysml.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfgblzet.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ccwkzsxn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jgfgdxvj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dktljupe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxjeykok.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3agxrurmi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gehyyljt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehytbqvk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rjcffgiz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3bxlohxan.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3sgvtdcwx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcrfseeb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eyiqhcnq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mjokiwis.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xlcdajhx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3txmrmmaz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gbkocfvg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3avmyoefn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dribfpvz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3twfddihl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fuzcknbn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3srzoydye.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3auzpwvwf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3iswcpofn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xthnheut.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fpuxnskc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hdeumczm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ycgoonjy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ckimfool.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3larqqhke.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xpabqtjj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kqbdhffs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3igmxepnu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gmmtxrhq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hoquodhn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3tuyqgqax.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3vmwkpmpv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nghbeqdf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hfqcddhk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hepsgivh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3isurhfyb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3eukhtczu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3psuporrj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3myyvkdfh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ahffmtli.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wdjlmabw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3arnyuxpp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3bxhuuwms.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3colpjxdu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3zwrmicgm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cvsihwex.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cxqwiirv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3brxzdgiu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fsxmghub.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3oajzankq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbhgpomn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvifibxo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nqdosqiy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kgmxdqcj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wfnkfavd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3awgdevuu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dqgrdfwo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yqjjiute.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dqbuiufv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qjbbdgla.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hnicyiul.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mqjmhutc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rqcqbehc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3dqiheztc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bkxgxjgv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3imhphfyr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lstytmiv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3areohwvf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3acfcrwjm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3skmtmwgd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kqyksgww.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3jezeycdd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3srhqrkxv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3tvenwvii.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3btpnbydd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bxiyalvc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ejpeednn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hcljineu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ittnjqdc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbeypwgc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yaneecsk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ipcvyulg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nfejosnv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3fatzhkvc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnvqtajp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qspyfeph.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3jtupdfkd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3tgdzaude.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3tkrdsdqd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3afftlgyy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3kwtczxeh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3scnlhull.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xfvjfhwb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bddqzfbi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnqmpsmi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3heunwils.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tzawlhid.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rzzlfczq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3psfdqcqm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rglrlfjy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ihvxwkbb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ivmpgjus.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3recgtgah.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rxnbjnhe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3okahratq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cvuciitb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3puaapbnn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ehnqkbpe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ugbixqon.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3grjyowuy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qqdojnuj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hjurfxya.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zvxfklmh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zmsboagt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3nkwhhabs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gwfuynvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjdhkyhi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bbvqvosc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlqrrwpx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sschxeci.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rwodgngs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kgjjlthw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xkknaxrl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lblefljg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3tydngrok.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qzyilzrk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3avmuhdmy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3rouyqotc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3kdhvpcgt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qlwsiytr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ndqpqpcx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nqwkttvg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eufvjbmj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qanrnohy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gwfstuyc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ppxpwusu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gnspltfq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wnnogtxl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3efxzqagx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xfastvfd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vryywljq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qecpwjgi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yvthnorv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwrqynn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3voionmzc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ssqbehns.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3slqflyeu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwomqtj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kcuitxbf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yebzqqvg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cavyfcxl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wxyxqtfz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rlpzjmna.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gosqukly.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3eqdgjync.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3aoxgwqlm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3btpubqna.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gkznopni.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nddrcpne.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3okatnkbq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3enrujrfm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mrbvlhrr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hauakkov.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jtmpfzwz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zncxsgzi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tuciauij.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqifgmxr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gumocjhw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tvvjtwee.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tehsphoa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zrlgchfr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3otvpojre.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3olnjfhtc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3afkvzbsk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kwwetrwh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mligckup.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3weeytiqz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oautknbp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jlvqqlrz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cwtdferq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3dphhtcvs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bkaasauk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ezcceffh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3alhrpdds.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kkztmwbz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3iyxxuqpx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3emibjyla.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nglkvkvq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3etrqscym.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ubjkhdnt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vyrqfpiq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wwjsjibh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fqyxmvgu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3smvsxbms.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ahjozqpw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3coshrqom.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ondlfctv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wgrwivsr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qyxrdtkf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gfweuwxc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3afietyhi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wiuwimmm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qmkapqtn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nzmrnxqb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vhlytycb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kjpollux.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gggywiok.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tdniurfm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qaywxvnr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3opjzmjbf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jygeyugv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lutujygf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xerrjhbw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qidhfmgp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3twhtmqij.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mmcdtcsf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ktjzjwxj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ldenxipn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rsumdvwp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xqddkfpc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bkocghen.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3aqwukvho.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kzuxvtzs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bkmixprx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wvhhkybg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vtchdgho.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rybhpiok.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3lmxmucii.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mddqhmml.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3amujmlko.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oetzqeta.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zjzjxmwf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gfepampt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3eeledmwa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3aljyfuqa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wxgoxyyi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xsaliiyx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qlpvbczo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zaqxejaz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfbxsmhh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ycnfisuu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fclaszco.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xnnlbbmm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cmzzeswj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3edgvdacb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jscciamw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uyddffbd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vfgzewcv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3acntjkwp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dbugpldd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jcdpkziu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3niehebrk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nkbcoyxt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3oygzxsed.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yrgrubcx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jafbnymr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fvzdvwqg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ykxfdebi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxkmrkl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wuoimhfs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3onzdttuf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ccwcfnkq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ujyjilwq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jzsjbnit.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zhuxlxke.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3metnjdab.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wwwehith.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tdwncwlm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oewjstys.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qrbcjhbn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3oskyodqd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3dmtcvmlk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xibypdqt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qghfziix.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3nynvezwm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3itexsrwj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nyxoozfy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wbohbfws.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mrhlwrhc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xselxqzg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gyysigce.html


<!-- 参考信息 -->