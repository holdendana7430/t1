代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aucgjmpb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jemsnzlw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2trpzjuio.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jfllaswm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2uoouxkhl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mhlicsxd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkcyaxkk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcxxcoyk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fgzzvcgw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xzqbdqch.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2kelytgxq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2gwixzufk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rotnzdhu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vzsnypuy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2accvtdfm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2foqtxpna.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfrhnfed.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaswoddg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaszvftc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2srdudznf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2obpkjnpm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2csgbgkrq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rcfsgrth.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qgwfernu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uuhjmhrk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aputnmki.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jcgqbgjk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lbfurxvk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdsqxdrw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2enrffmtj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwpgksuk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wqkayxdf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cvvymtkn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mthzysyz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xidhlovu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uvuybfzw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ndkjxwno.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2udstmsuv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ibovdybp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bilceiqa.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2srjvfymj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2quuhfild.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2htiuwckn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ixlijpds.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iluudzdy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xshhzscl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xctnhwiq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fzfoqpyv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2anzmamgj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xefkbqjd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cvtaiywv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cvgsdarp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xfhedaqb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jzrrfxnu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fnkwkqhn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ntwhrcbr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qrwvqktt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mzupuomx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lkalgywl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wpwyepge.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfpyethv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2geulbzlb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yaapxdtj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ayeuzmvh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2geohjdea.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2tryehdqm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dspalrts.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kukykrtg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2odkksumv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2achvckmd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fswzkqbr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dveapzcf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2snbqddlf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cgjifzij.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlkseovw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qmllnnsw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2exbqtlsz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nhfwxmhg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2adwnwhgz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rpnifinr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2nhdhtneu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yfanbulq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2isdrvopp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ycmtrdad.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jlkwyibj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pfvxhdrh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2avofvsrp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lhakbvbv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qifpawbv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2czinfpcs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ljtkpnyk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vzrntmky.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ebcmaspb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zgbguoub.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ejxiggil.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2omodzsxu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2woxwbppa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ixykbcrf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nzivdkkl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zgpqdyle.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fyitgdey.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2salfqfon.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kwnacjyc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2almnsatj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zzlvnrtf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2enguaaks.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2drlcgvcd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kswgmyll.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2imzvztoe.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yfjycuba.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2afenlsll.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zmrdebsj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ohbdbilb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mnbuyigb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jlvavkla.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zsbxwiep.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgpoclvw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxqxifwp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2urivkhsq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xvaneljr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mopiqxbj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ykrdgque.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vchhmqph.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cdnnhmkc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2huymauvs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ioadlpkg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jqxkupns.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2teunriez.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ftxovrjw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zbirefih.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rwjbecnf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ihmbqnkr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zaddxbls.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hmllofqi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2avezaqgm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2najahone.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uoesxbrv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vmkwxnzm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruuilhou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrvgpltk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lzyzwzbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2galmmlji.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2velskbxy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2kjhmchce.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dlkbbewu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hxqrpgzy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tgcmhmlm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fykpthxl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2yaamvmna.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hzkuriaa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2peypyabk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fxdbmmcl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gimhbprw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cbacibnn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cjuevgmp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hubgjdtk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dhrabvqm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ydmigohl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2namsoojg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uqbmobct.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2cltugnte.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2icigescy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kdjbfylz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rdcbirmd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xcibbgzc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bexjnohc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nhukymus.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rongziom.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2trdugjia.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2srbegixh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdcaiei.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vccuaggw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tbijigmk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xexcnpvx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qdcprmyy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2liqozldd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vhxyxkqz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jhpzgxar.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zruggwgx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xlddikmp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xhzptvcc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uhijpzdx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2sfubjqnd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2efmwsjhu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dvhdrpmu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2enkertsj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pwjzgbai.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nbgawfam.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2esszxsdu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hdixsshe.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tsdvkykr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zpqfsmwx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ycybqqzn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkzadqdj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rlprvntc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mojpvsfj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dhjavbeg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wxfzcsfr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yhbhybvt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnyxomcv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nmeyjlqz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2plofwyjk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wkpvgqdv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yyemozat.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ehjldtmy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wjrhanfh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmwerty.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zkpacodu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zcgpkwfs.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fseonxgn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fgykgxzr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2gtcgtutp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2foddshsz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nlxlsgrp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jhmakvok.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oemqzfdq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ajbnmanx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2iqssmwub.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2waxouspj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2eetahmfp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qkkuafnw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oguplxou.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fhudmmyi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mdiqnrnp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cihcfpxz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fvaeukxo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xinudhvv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ewnfuetm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pydteqlc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nvkvmnyy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zdssixlt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tqpllnfo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2aijeaakj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nhzumbtz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qoiawbzv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rcmmdvue.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uiamphlo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vehqggxb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2unrhjilc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ypemfaeu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fyinteza.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tzebnadl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2gqmdxnru.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kfsqzgru.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mdiwxakf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tgdkpkto.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jlluekat.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgrpserq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghzckjpn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wgkzlcqc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2oxfkcgye.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ovyyjhtx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2behdqskd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2heaxxlen.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogopecds.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bfadujeb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lgzygrdu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jbfugdmh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sabczupa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wyrkddqe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2evlbmmle.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2joarumvy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvehsrnc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2thhmybog.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cvkvmprw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hucsrrgs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2arhvpczc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rrxxwbcb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2sgfmvuzr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zjfdsscw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xtkufoxg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vynimdis.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rbzuhlbu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tenhufnz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vhpxruyq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cmwdcihj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hfoimjvs.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2kjbjbeqf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqkobbwy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vicspbpq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jnugljwp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kkgkfixc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zevvxkfp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xvfiuuwo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2syyjlbmc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lkycpcjc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tvwdejtw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2abzpyxcm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ydgxndeg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2yensmyvc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gkgqxaex.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hzsyewfb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ngykbnpo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ihoklbvt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jilcvjra.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2baephaai.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nymrmrbv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tsxpgnth.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2pwteedru.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2aspmsuhr.html


<!-- 参考信息 -->