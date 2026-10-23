代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qnnioype.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zhvempmy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bbgttscc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cmrsljkq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mszvmjbh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qtxfsnng.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wzlgdhql.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dpiecvca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttbefdrn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hzvlmjzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzqqvhkr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3egfronhp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xxjuwklx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ddatzkhd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwncfkfe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rceddpzw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aadwktdn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3azohokvo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xvdqxwyk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jjxmhzqy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wygoetwt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dixlnvtj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kbklvnzl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jegvhbjl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vevrnozt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yaxtbmzx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qfecwhfi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3slvhvfdb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ovytgpzf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vlsmgxto.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3zmzmtumz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bjchlpnj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhcrhhjh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dqtktohw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xnxcxrag.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3jirbyqhc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kjnzthkb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ncygiiqe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wujtbyst.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3iscpvkah.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgphciqd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfrrzwqm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nsuzgagl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3jwgvizqw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nammxdgj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgccrdwu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3plgvpccw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kcdixllr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3murmcqwo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3oijwkaku.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ajqqvgjb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3blbhtcqg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cjpfxvcp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uylasclf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cnefrijt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qyeemwqc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vcckdwqd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jcgssjuu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ofhxxoni.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lipwfslh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lanotwtu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lpzptpfd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3avztdaxz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ljfyopld.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ginzzjgc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3yleapxhb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgmmjeu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3asrhgwpk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3slxkymyt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uoaiszgv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zvccirnq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ecbvrjii.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xmeibazx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3cgcabnxd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lxxkwmwu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ksdcmygd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxpvhyvi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3denovwjf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vabgafzf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3txjzqldu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3msnzdywt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vfnvbeaa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bdhaogkz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3blaszqmo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nocamjos.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tinzgdeb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3amlrdzrj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cbkxscey.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3powdvywa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mqqcfwdw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqsddvs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gvvtkkma.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3klyeaswr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rapxjpjy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3lpbhuscr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vnaoxgdi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3numylweg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hilyvujz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ooctnkgo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xqvgbuja.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eeeaszid.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3nfffbrgk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ddvmoask.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tzjprhll.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3irovopvs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hmnitdfd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3iolbgvxx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3arxmfogf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aqbtxgmf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lwlptifr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hdymsglh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mommauvu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lfmtpgit.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vkzlnmtw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wxaiflje.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xnirbyav.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3npopxmam.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uooefhym.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qpslveoi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3kmlhiifj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xrzwhknc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxpxankv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mdqrzohb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dhhygolx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrzvadib.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ksiqlozf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pcwrinex.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bmnvqsqa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3hcravqdd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fpoyndvo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nwmoxqvo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jqpuxluz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tdmusuiz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jagxahwz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fitrrseq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tbtzvkaq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fzrzecnp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qjcijtpg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dsanqowj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vjgkgddv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vochohax.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qqaacmrg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3agthkmmc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pxmrhggk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kqdymarl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3hgozdswx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3nhstqqjr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3iiqoynjl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vjneohti.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kfadfcsg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zgjiwhsa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xtkbupsl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ckotybho.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3damihrgr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqcuytoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utdyskav.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xgceezln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybnqpcjz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ibyepkum.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xllgkqli.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bqxlnalc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wgbcjblt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3evjkffhc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3eugulqqf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3rmjifprr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3voruxsqs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3cegehbda.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qsfntwag.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kkmfarve.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3nelnwgoz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3snzukztg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ccwlvtjf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sxnijboo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zwlmzkpb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3kpgxyaxd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3copzrubc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fefakyxa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3onxgynsm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3arrxxdqz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lnwwhqzf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ildqlrlp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nztfctof.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nricuhcv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yaspxzsa.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kffygvmv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qpgszlna.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uogeswlz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mbotvxye.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yznwoday.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gshlyzrj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mongtucc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3hkhcoybk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vlekecre.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ldkigmvz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qcpjoaid.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3crknmhap.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xvcuhlap.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kwbtjail.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3isityqmm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3emhhyxpv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pdoeikox.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3apmjnocp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eyepjelb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wpyhamhq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gfufqhoi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfllvalr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hdgmfmet.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jsedzodm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vycsdptl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbhvtsn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wlvubqgz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xtxhoapk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zvdhggtg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3woxhdotq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jjdcfsuf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hiqstikt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nuvsqgeg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3imssrxfy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3godlrbfp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hlnwqlyd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cpfgnqoi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wnmiyosf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hbukbttx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3haojuhgp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tuppjrij.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ttjzjruo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3nthpqrar.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nfelddxb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3buaaunpj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wzutqfau.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ipnfaupg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ykygrlrj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kqwxxdpo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ccceagbi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3lzvctbju.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3eubgcagj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qvptbkkn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kmcgfgcf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gzqmoygv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jbtseajg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3koguywfs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ausmhlwk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3llgdwmwl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qxhbinkz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3rslttnru.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lnubkmhu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dociekhm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wtwolbdw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xmjamzqc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3bcbimdtx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3easkvgyx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xqnhdhzr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cbawhehe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kxmvupwb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3liolauzw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3svnydqgg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ckqbyrgq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hnupzdep.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ysysgxuj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gihwtbdw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tkunuhgy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dzjvzpha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3sxgjsgsj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fhmzvruz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3srnnxccp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3puwpwqjm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3dajrmbxr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hckrlniz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3zwgevysv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmflgvue.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ugzharna.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3qtbufjth.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3agptzbyf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hmtxpocl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rjrzroxv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mcmmsfwe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lyjtnsxo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iwlvwogo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tyxgruok.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vubfavqa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mtdicbod.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3voapnjuk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tgfhazcp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wkwrevwl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3sxojncwc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jkbiswxu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3buduaeab.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zhblofez.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ajonwqas.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nqokjque.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nobxkdbb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zzezrrun.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uccpgmqo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3oisjdvah.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dbquqtmk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vyglurfh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yrbfffjg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmwgzel.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3clbjxied.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3iitdkufj.html


<!-- 参考信息 -->