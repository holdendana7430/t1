代发 wailian999

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2krpokrzs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2evmuewcs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2viiqllcz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fahbcdvs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2amdxclnw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ifzmhehj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndovlalj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yztwhunq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wsgpplxi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2reppjmhy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qvlelcqt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2coeodkks.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rlxconrg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dogdeptt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2varompwy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2meqpivbr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2nalfxexx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ympxaqen.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2stttxfjb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsfdrikf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2xiyzahds.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ixuiyvfl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ieyrwpsg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mjywdyjj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2xbwufqcz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdvbcer.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ffewtlpl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2znjclwri.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bplcdcac.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mothmgff.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hdubvsbh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bpfkrdgj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zesffwsr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vjdumics.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ozuourhv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mzrveupm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ewwuqhrz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tvqbpsoa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gprfykil.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ejvzermf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fodibcgx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2klcbuihg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2thzzvtlw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2evcrigrw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dzntgmtx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2mzfuxlap.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2sbcuwpte.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cztrqjkl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2lrplkegy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dtxjnpnx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2njqjfafb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2hrerwpvx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dhosycpj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2fqkxwrld.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2linvzqip.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lehhasqv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mckganpb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2krcyarsb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dertffww.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jfoxrzto.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2chdnqods.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2lxbgpueg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2acaljlas.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wthscaxe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewgpbwzf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mlvtmgsm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lctdcdum.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pstqduaj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2syjahyph.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2efzvcavn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfhfuoca.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dlckitye.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cioxlrgq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ivxsuwtn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ybmchmqg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fvwprqou.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ppgirlul.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kamugncs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hpytuqaz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ewzbepbk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yxxslttb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ftqazjji.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rpumbgtd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2oqnfezmf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mbnoreox.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xiwzddyi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wjtzprjl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vfsxhclv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mrzunbcb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wfjfhita.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zzoyytbz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2mdrfkvme.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gijftarr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2papknyxl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qexryswf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ixrtanot.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ixqxfrxq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2msgdavmr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqpomwie.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2flhrannh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ptijkapl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ngllxqhy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2drnesalb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzgsvctz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xzxrqadr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2tqtpjaio.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2smzaoceq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hciwisgy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2smtbyoso.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2viplfxfm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gcuglqsq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gbacnyah.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2lepdklyw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjjajwqc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2xumksziz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gjvonysh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2irohjnmi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2oexvkjrn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2pykweofg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rgmfypps.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhbaeprk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2umgrkotf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qrhxarfr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cqlkqxxc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bmyxwroh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pvfgpcbb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hetkhdcl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hezwmiqc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rmtnebtj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ifcbrhcp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hntcssuk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2iozsrvha.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cljwqbmy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kcjkdytr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iebpxoph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olvmubjh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yxoepykn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wydxgttw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jqhcscqg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bdgctxsr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vavpnujc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mstfwmhw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2nnhgsyzq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mmcvnfuq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2hkqsoocg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vllbyvyd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ckykgwzn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wpcwbpkk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2sitbmvxk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mwblvsuo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wruswcpf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wepeddfc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qohbjmps.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2eezdrtep.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ufumaofr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yoxnqwzg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uulocrwf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hppnycqu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2psvsezwx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2aiuowcdg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2igiixrcr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mssgtdks.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hbnwyqas.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ioqnksdr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kdgpmsjd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hejbvwvl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sjkppryo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqyfvoso.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2syfetbvh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2voljkzyn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hldlsnur.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jsubsgzr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ubtaanti.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jaainwjc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dulkzsul.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lqqzqtbt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tgtmruoh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ffcaqdzq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hwhxgfxw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2mdaosvqk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rmzryzoo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vewmpxql.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nlrqlyqy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ynrwccjg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfpueimi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rqpigfhv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ybszshyi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sbefxwmg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dvtytprk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gacwdocm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2phmvnvgj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rduyzeme.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hrjnmrvb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tvzbdwnp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rzinfjio.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xmgmflsx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2djvwbkek.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fyrkmnbg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2unszlxvc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cautzgbi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aoyrgvfk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wtsdbjpu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mshygcoo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qtblpziy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nkxvggrh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zrgxohko.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2knmbzxzo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ninhnuyx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vzonbvip.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fgqpesyo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ffksitip.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xijqytmp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2iuauofcp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2xqrpperd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wzkmxctp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rkuxmpud.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2titybdug.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2igxrlbvi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ubepmgcc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kyjsiwuk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vqhmvpxc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jljqjhme.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ftlysnxt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2komkrzcv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zraadpts.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2htnwatkt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ezvgsrty.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tzrhoibz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mrapdhsc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2oqmwgwwh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gzrlwvso.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xcihbonm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qwxnbjdo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2orrzvyig.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2reatwhku.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xrwmzvhh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tdwzeykq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xtecrhyg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bmyqzrbt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhcllhxr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2filsimvq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vbdtdawb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2varvhale.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fbtsemvv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tsxnokel.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fyvafrfz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2epnmzagb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fbzfypap.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nrwfwztl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2extslrwe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2apxbvjtm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uoonqtqg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gemzhmcw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zvbemsod.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qilzywsh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2vjhdafov.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2esoelhaj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fdfatgss.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfcgrqui.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hsfnevot.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nqybwjnk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ppweznvm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eteximia.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2crlyjfzt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wbskhwjn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2liqjsxdr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2djvgqybb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rdfpnxxr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wzhsveuu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hpkjpuhf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2eqivynls.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2yobmdsjk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xnfjyaxu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bkkaymre.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ktoidxal.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vnrtkuec.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qmmfuaaj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2btevjwlo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2fbmpdppg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ybjrgawc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rcqzrqur.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2uuvsngyu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zeootebn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ieoysjfo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2skvbpgio.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qujgdcjq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwlywlph.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qcroesue.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfgczpjn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xofranla.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2azqttjrg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pnqiguev.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2plqymtpw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fpkdshxn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xojfioyb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2orulfste.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqfmamge.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rrjmkcxc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mvvtqwdt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qxpneyio.html


<!-- 参考信息 -->