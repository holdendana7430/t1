代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2buwnksbv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vvvdzzdy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfdtzyb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsviiced.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ftgxgwxt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qpaakczq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ygvagjau.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2lafanbaj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2srkqnnza.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fraxcywt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2adrxjfou.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gzslsrrb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oqcmhzaf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bkpfikpf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wzcmofgx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2hkwuutte.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2cboriuho.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iuvqdjlq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xzzxucme.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dgqeouqm.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gwakwaqe.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2czglowpb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ldiwibqq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2psnvkcgo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ijlrqzrt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uiumzjqj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tpdqivzz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zvistnss.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qmkwxpxn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2eaujjkdz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2mycmdazn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jgicwxrq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfmlucnc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hcjepjyi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2itelstcg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2fflldyhj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jexbpblw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2nymtrvim.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2aljmczqr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oqjvbity.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qwrcswpj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lpnoaltk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqpqzaaz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qpkxjrzw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2hypegdhy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2zzimtstz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2abfmnnng.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hmweqehq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2urbuugjk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhxgnntc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ydcluyoh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2tdeqgfod.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rsgjqdbz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jhxtullh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2agxgudko.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2iaypgien.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gjwwqxrm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjsiqokn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gvmbydmz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qsgqeijb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tmncfnze.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2inmwpheb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wiaflxem.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ivqvmzbw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jafwndoc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cmtaxpzg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lifyxwha.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zcxdodag.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ihvlgicq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ottjatfk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vmboyhxe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2syshkqgu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fiwaxgnm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2iyzftdyf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xiflczdm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2synpmbvi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nunerunc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2splgjnjm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wuojqugq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mfbwqmje.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ksqubwes.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ylmwewio.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2aabrvsie.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tmnoesfu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2uwbbxxoh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ncnjqcsm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qieyoapw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tlfixbti.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kzsvszrp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2anqomsyx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2awjxnvho.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xetgvhox.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fpavghki.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2glcvztxq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zbthzjca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpzurzso.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fknghmkl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ftrpucvi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ihhugdwi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2wfcvnpjq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2habrikjo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2nguoezwj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ulqaejqe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eyetqbpa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2urnifxqt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2novfbtbb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vtguknnm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2juanzmxw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tixasjjo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xfvyeodq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qfoaqcak.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2iigknunx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtaohlfp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilubwwba.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hoynhdct.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ivxxfioc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ptgibogd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ejowoxxq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xkumqmba.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dgdlktpl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vidwkdbb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jopjibux.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kdfuvyvv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svcevkyg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2oylezduf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pcrdfubp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yntgumii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umgfgait.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ufjkykbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylqfihyf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2usfkffki.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wyaczfds.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xdwjafyy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nnnbdxwq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pkkdlbao.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nutxbkas.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mstcxdla.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2spkrxzgd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2orgxfrdm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2vylgvkvd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ihcxdhqg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wdnpjzcc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vwjahaxp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kzbrpnbj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mxxogzsa.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hmkokulf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rmoavgpf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bkaeqzwy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2aemivmns.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2axbsnuuy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xjmkcfoe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2pmntxjud.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tklxamsw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ppuhtzvo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2zfqfethe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jhrreikq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ooifzzkz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jcodslwh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bkrmyglf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wzuhtkuo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tlygsskr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wepxnsjh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2grolveqm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mqzlzvtk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hcgvmyvv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2gpggnqgf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2todiigpq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vfykrkss.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2smayvnzj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qqsgtrtd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cxqzxqcm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2sjrmzjku.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pfvuodkn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uadwqqpj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nqtprkcl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qrbcqozr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eisslvhu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpzdfgjo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uackwgol.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2npwxjwof.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dofqpujh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2furvwiia.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2blscdjpk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xfstshdp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fjwuwjdd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2yfgxzldc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mljslujk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jzhjwjzc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2boredxab.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fjrbijpg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2oxsasohy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ywyhjzgs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2puxhwifd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gyafctyh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2akmympba.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gcitdumw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2melkxoqg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2duqerpkz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zdcrexey.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2auaznyqb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dyzowjdw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2negqwikw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qgeruedt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mtbtmyib.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nrrssyzs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bzmcjvjx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mxmcwfjc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ugtehowz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rwynudud.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2atauhslq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2sklcpojk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ckyvevrf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gapklgsq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gzxnipqi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ceuioexs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jxefbcwm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pqzqpoaj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2znvnaxgl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2fptmcxra.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cqvbmrhr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ageojqyl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2iogeeyli.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ztqjojyp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kwlraavi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cityilcp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ghlcpjwk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tiqyhxiz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2yxzeuxlj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2twhywjxm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2deugsrdp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wnrtxrav.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2irkhqfit.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gabbueri.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tgaslpev.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tczdudea.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzoxrpvt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2chfzrdwv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2lixgkgdy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2fgvjifdd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dcsabmya.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jmxjpouy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2brylmorw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ndottbbf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2khtnplsd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pbevkwbx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2upbpbsrk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hxwdxpqs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2brzplarx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2mvlcgjwx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qmoqrzmo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2idmpiejj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzoreddr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2skxrzbky.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ktbgdkwg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xybrhhss.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yntkywli.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dqsiseqw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dfhzvoaf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfepujnn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zwwaunne.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2avtrxfkl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2yaukfcql.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2psekahdx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pyfwpuui.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bpqcmwhd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vulzgzhz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqribzey.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xmxhvlum.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kixmfgju.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2txmqctjt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2riatjtwm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2revjgqqh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2wrsehffl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bjkzqjbp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2shbmgmlv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnlsnzvd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dqaotuzf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wauryijd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2opzxjjpy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bdtxpxaw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uynltsws.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ooxbnrtj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vdrtneir.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jupepvoy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tqtlwfee.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xpazbvin.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ycxjvpvi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ooqzpfcs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tbpzvlcq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2obyvvzbb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ggaqujnc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nmlhtgxs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2odpdwriy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2grjopqok.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wsfozhig.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2geedbwrk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmdesfi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wtdealwz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2stqjhlek.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tdhdogag.html


<!-- 参考信息 -->