代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3jzueofdl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3oilubwqd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fzojxruz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlmemxgc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yjztaqja.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cszvtymv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nkzzrieo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bvsftgpu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mbqsrbyi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3kcfhytes.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hoptqxrz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3aikqmvnz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wvcnwojp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kfgbcuwm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gnguzuja.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hrvsevwp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3obgkzahr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aoyujkrt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ayujragm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mlaxiprr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wefqyppa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3uzozinkp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rzphzcwq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ncfhffbi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3saatpstz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xehybwse.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yghjkxyt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ynbvrjql.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3hdoljfmb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jhyyiqlh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zesmheyn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vstrjwah.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jivxmagp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bfdyawan.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nmpdlijc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3bnhwbhxg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fedshyql.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ueocchhc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hpnsbquz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nowmeyaw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3equuarmq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gwioosep.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3otwuooqj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lnxdanbk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3nukhzmig.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3xnngkthm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ppptymal.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hjjxyxjr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vmijxlek.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpjnagko.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uugrbyio.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3hqasatts.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3pgrnbvqj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3aiusbkrm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oahoseac.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dqfrtqaj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xbdnqqni.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnhaebye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zszroeck.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kbodxfjb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmyjddob.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3jzqffhqi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3iimadadi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xnrsmamj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xolrmslw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ugdfwqft.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3jcwovmuy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sdksbdtb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3idypxlrg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3thkqvkjc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ubqenaxd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ionptuuz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jnwlzfwg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xljflzny.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uoeajueb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3sttwzfwj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vzbgchso.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3oowqatvn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3kbdcagqg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zjcqlqux.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mmajmdes.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3pvwgkhox.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ykcoizhm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3acekgbvm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3cxbzockl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nyixcyul.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3eejyomzr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rbmsrogl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hrwqwnqv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dpefdqpi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cahrbfxv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yfqanuds.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uhsdpjwo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ooeghsby.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wybilqjx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3skdqirys.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkruudgb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hsmamlmm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sjnfxhpt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xinaveud.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3myrdzmol.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3niyggaxy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ckvarknz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3txctcubf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3obhmihkl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dqzzofqe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3loxchebb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xclxnwdj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pdowtgfi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3shvgscch.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kvznzvfo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hupogoja.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3garufcdt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyhuqmwu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3somaumnz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vkphehmp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rrwnsghw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3sqvrpbkc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3liwvlmwh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zheddoht.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ommuxlvs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hnvwniys.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dtckcmvl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cvtoimlg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lixphose.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dhgcynkm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3tayzwcdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyrdjisw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dgmzsrum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttkoeduk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kpkiqpfo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jnowyjzl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gxsyalby.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pgtexwus.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bzzlpbcc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ycglundd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3htjcjulf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ggdjxiul.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3chqtxcew.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cmlrndnm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3kcrdfoas.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iqpugnrw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ssiitidb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3juvydmil.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mhflglws.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3evwsecly.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xtgwdzgu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bazydrel.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fnhdhhke.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lguaglud.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fvuzdnoj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3waynweex.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3skwxouia.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3egaaetci.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fbzjmkrw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xzlnvwhq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bsixxkjp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3musukgvv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ybihuvwp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3csvdiqbk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3orbwblpq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3pwqjobil.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3drzqyzua.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3krbswvoy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jorwwxon.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3iqldazdw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3btdgxrrs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mdmycdvf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sohwteal.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3avhigtwc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kzsfirdl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jvfafwzk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yjyslqom.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xxxzetgv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qwcxgree.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3upmaqgiw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sdtkxebo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3imgrsylj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mkyrgnjf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3atxgrebv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ivygbczd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zzjhzglf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bnydtagz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3urxtwoer.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hubbtjrn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3duhglajz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vsynvnny.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sbmnzrqf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqnlvexk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ievcbxuo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3itttzdoz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3pwkgwlxi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tgoimszb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ylmaqeeh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eptniymp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lodlfupf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fsyiuobt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3odwjxqtd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yrkjahge.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vhhgewaj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ocqssklo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tqesssqd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hohgqrqt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wyoyatex.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hikuxwlu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jweqwqyq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jgkloetp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vukwtwro.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3helgjuxa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jyybypbh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gagdfuba.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3updydbex.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vpikhjva.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cqfutuzi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qimrbazb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mdguerjw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rwkdpuad.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xcuxlnxn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3uerlzxjo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fajiskto.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nduvbesb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3trlssvbh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3igvyrruu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kcuvvgkd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3dqnytyaw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ftmlpnbi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ummbgpav.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vsupgudv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3atmxezxn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ucozocmd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3sitrzetz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jcrgknbv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xjnhuoqi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ndkwasiw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hucvxfuq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lpglfyfw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfqcigae.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rgclofzn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3loobewoj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ladnpqvk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wfcviiiv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wnthuxqk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ebbspcmq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mcbgrnul.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zzlrwygc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rribcwbr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fmhxpdno.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jipighhr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wdvzperh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3epivvjno.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3atukinfr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mjzewkfj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lqjrjkef.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tqbbmrrd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wqzndhew.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aelmkmcy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pwaoafeo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dpwkfboz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nrfhxhlc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3irkkycjx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tvaydois.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ufafxung.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3djwosvxm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3oiniunvo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uhdwajim.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tkniwvlm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vqirxtta.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kgkskmqb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3chhwokfw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wkbahdte.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fyfqlein.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uilbdbht.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pyjkhpjs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3docyxyme.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hoququxq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3drktvych.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qminetox.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3okgynfgk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxhqtpbq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ebpvtqyx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eisdcylo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ocmyforn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ascnfltv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3eokpdsiu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3brebuffc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3jnfudvax.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rcxctrpr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3myeumzrb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zioetczf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3prgpeppb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gnfolyzq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aryyksaf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3cermrjrw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3wvehulfp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qdyxtrpy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3upztxmvd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tbibmhwu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zrreahmm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vczfxrlt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3edlgikwp.html


<!-- 参考信息 -->