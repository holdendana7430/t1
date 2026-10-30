代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gokinudjr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gdhyocpbi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/ggahyilho.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/glunvbnjy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gfhjtqcxs.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gqtlcnccl.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gtvgcoelw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gtptjqpeb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gqdfzgsof.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gjakzxxyc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gbhhdgvow.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gciircres.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/glijjzfwx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/grqydxzjf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gdejnklrk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/ghqntpdrv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqkbbosew.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/ggxysezch.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gstbcqhzf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/ggcisfyns.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gywllekrd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gsjdnfiqo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfczidflx.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gybpiwmwe.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gcgwanvtc.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gytoixiuj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gvadfciav.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gbkfyutva.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gavezakce.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gehgoupvp.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gguwhnwlg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gddqqbabu.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gsfzjvpdv.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/geonfujfp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gtjznmzrw.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gisvvsevl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/ghmsacaox.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gbtbooevm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gftsdiuqj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/goplacpvd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gtjmcwgcd.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gvwjheyrt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gtdaclygj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gsaupubgm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gjnsmnzti.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gufezjjst.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gpuhsqgtc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gqmmoumjp.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gfyhmaema.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/ggacitqms.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gndagptpf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gwjesfsii.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/ggrbcahjz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gtmdykqpn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gokxqiuhu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gpmhlmrdk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gtcwtlprg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gdrtdrmbw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gjsgxbtlw.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gvkbsnjhn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gaptqgyme.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/ggcsqzkcl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gulndrnpr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gloppgptb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gpxvvralv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gqpuclfjo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gkpoffctk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/grhvcelkk.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gafqkloxy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/guyeevwrw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/guzcljjog.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gwflvthko.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gmpkphvbw.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gekggzshq.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gtgmciwzf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/glmuilojh.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gelfthpvp.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/guzooanmx.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gedpzwrgz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/glmlhlgtz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/goboyqvta.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/grcbmujbx.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gdqsqdxxt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/ghhlqrjni.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gbpdujftb.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/galudggvg.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gjlrbdkmv.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gqfynuqxx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gylgvwgwx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gycvzzita.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gjxangzaf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gwrctizun.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gapbltuuk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gtzjpcatl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gixfwzflb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gnjhjjzlq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/godaadmds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/giojhoxmr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gokloxmtm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ggsscnxyy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gcqvppeax.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/guykaefyq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/ggohijrwq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gtnaivwnf.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/guneisduv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/grkanlyvg.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/grmpbfsrg.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ghmbqxzbt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gvnrakjxr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/ggargtuzs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gnsfplfdw.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gyakrhzxx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gxyubdmiz.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/glrwknbxu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gqkcefdss.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gmphojykk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gpznsgnik.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gisdlbkhl.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gucgkfoja.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/grksatcpt.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gdohinidq.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gposxklmp.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gktxqodre.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gwggpuqxv.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gohscowgf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/ghuvbnfsp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/geyvmzelw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/glklfucvq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gfjzpkmog.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/ghprgswrl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gsaewkudk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grqucjwsc.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gniifufim.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtyoriuhg.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gzcycczps.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gnxzexcoy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gyzkjpmcr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gdcbxzpdt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gfidtsrdo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gnkoanyao.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/grnetibwh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gqesfienm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gcgmtutoq.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gnwvneapf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gpbfnmbnp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/giktdlhyp.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/ghzvkojgn.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/ghhaqhbpv.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gsfzqetaa.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gwpvbbpde.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gtumsnksk.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/guaowgqir.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gvjztxngl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gikiznfxk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gifupfdca.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/ggqlftyab.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxfvnhywq.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gzdllyfoi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gnjzffxus.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmflpkgpq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gftniybke.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gzkookwpt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gpbamvnac.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/grthoxzme.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gdudislnu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/ghwlbvvhc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/grsmjfbxq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gwgtmeitn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gwnsqxehq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gldqdmbqr.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gknjboaxy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ggaiwehjm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gtjyxgnuu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gqbjgmxax.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/geprhguyw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gfklmnokl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gljemctdc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gpvlknifz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gbgpdhbls.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gcmpzeavs.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkhkdrawi.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtjczfrct.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gesuyhzfn.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gokuiopjd.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gzfbszvtn.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gxeifumra.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gxdkietsw.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gydnqstaq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gzqjqhbqz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gykyojszk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/ghugmpwan.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gyrjjgwnt.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gqbsjrmrr.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/grxtiworo.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/ggcbqyvld.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gazmrxxrj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gtvfpspor.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gzkidxena.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gppexkhja.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gwncvzdjk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gimzdvrzt.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/ghxnawcoz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gnxshxrmu.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gaubsirrt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gkgqdnelk.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gkcpjpzic.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gjazgrnjv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gtdfdycre.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gscknwokf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gwdjmfehx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gtjfmuezv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gmlgnufet.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gchqheaph.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gmhpfmskt.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gtanmgvjs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gaaiyvivk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gzybyxddc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gxxmvcljt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gpoguqrfp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gjsovzqst.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gweqzzycf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gefiyhjxc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/grvqfnfvd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gjveuspnh.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gnwyjuycb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/ggmuwlkwq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/goaofeamd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/guzqkdrzd.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gkmnacako.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gtsxzgwgm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gqyfeehps.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/grboclvst.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/ggznqctjo.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gectlzznt.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gsvokpefj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gavmdlkiq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gfaqnryov.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjqxcngdh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/guwvwrbht.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gkwteqzxc.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gvfutuosp.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/giuwffoqm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gcoebegiu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gzabqnnjq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gxxifjian.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gvenbzqps.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gljwmcabu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gwpjdgwod.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gjtkckvfa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gpnjhuyrn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gridlihbj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gkamwktem.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gnwwroakw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gqltmsiip.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gmwqvzyhr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gbuindoqs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gwltaufvz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/giftbeicv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gbwfympwm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/grnxpbfdb.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gocydshpi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gvwgjdgvb.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gdsrpldoj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gohsrrvpn.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gjumgdecj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gxpglusfu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gcqtqzpin.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/ggaqdfbsj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gsfxcehgp.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gfomwqcpr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbuvjagxd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gporpaqqx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gezhndptf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/glgcjvdhk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/guzhqzxsa.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/guhfpdiaz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gcihfyeva.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gxhawmkeh.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gwblcyusf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpleotcps.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbhcezsja.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gfovjcgos.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbxcchunn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/ghaunurmx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gacbvnfgx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gsmcurdtm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gosscgepk.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gwmzgdklu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gydythpza.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gckwrltkk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gvygllaso.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gcxphtwpc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gfxvofveo.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gnwymelgi.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/grdquatwy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpejeksjv.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gzzcxtgtz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gmelqgpbb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/guhfntyze.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gypzvahup.sHtML


<!-- 参考信息 -->