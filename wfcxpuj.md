代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/grxucbffb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gmlnqbjhi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gaxmklzsl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gezrpfbzq.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gcqvocrpm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/goedkvmhk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gpxnwtwml.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gmwwyjavj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gaxawoaul.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/grzgrfxhv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/glykyvqcf.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gsrmgaeqg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gpproqobr.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gmjlmyynb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/giviniffa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gnnwnucmv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gmaddxecu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gwiurqfbr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwcdwekiu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gyzcpbdxk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gdyiigqom.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gqrbsdrxq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gfjuwrscr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/grvuzzpbb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gaesakkbs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gatjiksfn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gzzoupnkv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gltvcwvau.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/guodrcttb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/ghlzkyhch.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghzxyicyd.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gaytvmdlh.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gnljyuhjx.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gkmlhkgea.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gkuklkwdj.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gsjtikjpf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gwzqwlwuq.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gowafawdi.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gyfvtkfjn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gbgsjtuzo.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gdaszsasu.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gjifxfmuw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gbqnugsmi.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gfmiusbxp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gniawcqrc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gzqsutdyo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gvrcisptg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/glmkkvgoi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gjwumaikn.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gjiolbwye.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gaqzvhifq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzjpqdgc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gazsrsvey.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gjbucarts.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gpkhbqvse.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gghriyqfc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/glkgculhu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gqteuigik.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gidhdrolh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gjlpmosqr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gxhndqupa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gzmepbwfz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghckmbjlf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gdgmjwreo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gcndlfmum.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gohrhxmtm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gepufqlzk.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gybkytdyt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjnvfqzmt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gykltpwdq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/geicskxji.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gkusdcpvo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gbddwrkej.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gwrdbdgkf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gzfhdzqgo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gzmzraxxb.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gurdsnnaq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gdmeyeixn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gnjhqalhr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/glaqwlbkt.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/glxxwuejs.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbpmlgifu.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gqiwbleby.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gxdawkrlv.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gtsahcwaw.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gbmobipbv.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gjlvanwsy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gwznatejs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gznwbiuto.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gtuqflifk.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gvtombdjs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/glkwrkzxe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gpbphofxv.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/grshwuqew.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gjhmshtad.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gqgplvrlc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gvzbliwby.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gkxefkabm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gzktaayvj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gzhbgtvch.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/ghdvtwhwn.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gmhuewnrp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gcohjkdqg.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gmmhdgmkv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gevxqdbzx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gcttousbm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gtivsezbe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzxifiklg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gsgjgtfmd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gjxsmerzw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/ghwxjisve.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gbhbgboay.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gmoqfagej.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gfyrzeasz.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gkhewqfbx.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gkrpobotc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdevcnpuj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gcyulkhiv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gjlrohrji.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gejpfukvs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gakxvlihh.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gybeghqbc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/ggzbvmdwb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gaywoyjyp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/ggzfdkrsz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/ginfznrcr.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gcvkgtyxa.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/geinnhevn.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/garmbvile.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gkzjclvch.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gyjcceyzi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gfiokaecb.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gyxosissw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gbzzfieyx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gfqiagkrl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyoakryjy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/ganjxohdj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/ghjktznbt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gymyzudto.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpaaejrdh.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gykosloiv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdwkdipif.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gfzjilgeb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gecingvzh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gvpgmddwt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gponbkixu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gvpiefyqs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gczdsqnoz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gjldseins.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/greaqdzfu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/glygxwbbh.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gkabegqas.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gunzaxuxm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gpwjgoxvn.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gubwymthn.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gqvbdbtgn.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/grpzoodes.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gryzaqpfp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gulpbmxsv.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gejbdcdbc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gvvhrbjpr.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gryrxnzwv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gzuiwrhly.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/grzefzzep.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gwdaawjgt.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyszfqena.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gxrnckpxf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbizbbat.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqxdriozv.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gvvdquqso.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gncmtmjvi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/goaillxwv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gfojnphdk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/getjrvgra.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gdsivweom.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gwmcrrxgo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/ghvfaltcd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/glhvwutqr.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gwnzwxqei.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gsyymloyd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gpzrpepnt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gxsrpetgf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gxngkmyph.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/geakqfeno.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gwcwyzqgc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gajhhwbge.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gowmdasmu.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqataogxo.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gugktebwl.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/guqoapjjy.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gmfgdkbyl.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gsflwslhj.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gejuvxotf.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gbgolxets.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gvkjzqmds.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gdytbqjqv.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gclgrzcai.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gjrxpbszn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gfnmkewgq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gvpxpanvd.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/glonsndue.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gwbbiocub.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gclwvkkoj.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gkmyayywc.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gczwjupos.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gmksdxrgo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/glxwdvygd.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gshmwfxcb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gxxgycocx.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gttdwqrpr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfwaaevjc.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gltcmakin.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gzxgzbnbh.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/ghfwyiagc.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gjzhhljda.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gmpuzhrqr.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gaybnasmn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gkhuaebyy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gpmjdxhzv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gtesdqudc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/glmnwztmr.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gnwnvtiku.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gqrguyptg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/grlyzdode.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gyhelwjut.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gedyhphze.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gcfpzzyew.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/glyryiyjn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gzwbvafat.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gmggqhozx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gfrdqjdla.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/ghybxwedr.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/guhgkobfq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gimipjcmt.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvnxvuaaq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gabncbrqr.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gwxomthfz.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gptndabtp.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/glnimslbu.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gzeqgeysn.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gondtgjgx.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gerixpkjx.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gamllpsil.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gwjkgguwl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gblcdmftl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gulhvjmed.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gsnmdfiqv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gotxciwhl.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gmujierei.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gkzcgkgnx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gleqtmpzz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gvzwemxhw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpfakageq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gsiyiilgq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/guwmiyvsf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gzpeeiqmw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/guyjelxwv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gusommhno.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtoktgcnv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/ghggbvwvk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gndwynvrn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gxrksposj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gkjelwxmm.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gvrixqice.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gutlrcuzk.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gmjugmgkb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gbtpfcinx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gecjxzboy.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gusbexmum.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gejjansim.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gvmqypnda.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gfatrqiol.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gculsqmuf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gokwqcfoq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gvcazxdyv.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gcojngbvd.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/golditpiv.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/grfagrtxu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gqmjmzaxb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/grklklbsw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdodraitb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gqzrjbwvu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gdsanrlsd.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/ggrzzquqt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gmebkbpng.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gumzcflwo.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gxsduibig.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/ghqssazdj.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/ganakoocu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gdpgxyylm.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/ggjdxuazr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/ggxjwrmmh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/guddrmsrn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gkgxypgvu.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/grpinimfy.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gcarolbbf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gaoaivmnx.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gfkitmuuy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gudikcnao.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gwaxxnxaq.sHtML


<!-- 参考信息 -->