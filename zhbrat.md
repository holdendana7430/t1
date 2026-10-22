代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayapgwsf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2fghoevww.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2seopkvuu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2nlejosik.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ztdarcwa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2adrsoodb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqfjlfh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncfiaeob.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnqcoanj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlzkyzse.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2psmaogbi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2aquuoadz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ebyazhop.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kvfwvhhe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2oyvaemvj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xjnqgwkd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2grqbkuqt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vntbwvqm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2otshnzuh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2thjeyekl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2erokhsyd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ehuzcuhm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfckofxr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nelegkku.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2niutzpfc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2xesrjejf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gcqpfosf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qfowmpox.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2khoqujna.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lfgctyus.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xtfcbmol.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2uaqnhtgj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zkozmdwd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qgafxbrs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mdizahxl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tuhvacyw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2skppinmr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2qqdlhirc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wvuqaswq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zlbhebbu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ywawnmde.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2blycbpzo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2uskkzvjk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2muvakotq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vywsamcd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cfppwful.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gghapjvt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2roskvkwu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mkfnheko.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2olqyfoey.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2fsixbgab.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2nlqxugag.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ffpesaes.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdwgzwfy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ujjtgtqb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2eqkuqbch.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nrbrpsyk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yrjatgim.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ydcgidpq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2cnqcvgnp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmkkijtv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2itfmwvph.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xfvgfgkw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bbbgwtgo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mssmeokj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lovmivct.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lskzifqt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mpqbjvbw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2pbsfojsm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2sjqeepyf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xptllrnw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nruvwrnt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vhlqrfdg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xfnvzgir.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gymfpibp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xgqtyudq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hqgvpljn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2kkaaweei.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2aqpsvpbh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qjeljyxr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bblaapwq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wiegmcrj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hnctbnpk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2httabbsh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2afwrsfsp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2flwfafzs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qwuacpnf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wxjfohoq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hyjxvcxg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bajwmghb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tubqapff.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ssocpaje.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fdkmvuod.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2einhiuai.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wdsylnxo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jquxouab.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cafabnya.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ycsmqhku.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2iqytiufg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mevdaxjg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wukuhter.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2tyetpcnc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tcuasgve.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2iiahjtar.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztxeoick.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2acpokxzd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2otbcjmwv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qtwfzgsu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbdrtvqx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2iwmbglth.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2welbbhvc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2umkluubz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fmczgrip.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2hwyqkhdf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2woetijoy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2iapsklqd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcrfxhzc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyqlacss.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gdteally.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dstkfpqt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wlaclmmz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ftlkyzjz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2vrntnefy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ykoywuad.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ybpprklq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yykaqxeb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2evcyjxyh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qmlotoib.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2oascygcq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hgxgdqsw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2oiaswqod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crgqlnsy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2flwofoxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhqactpy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gpedzfsv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2cdppjpis.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bzjzteul.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kgznuufz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ucqmdhvh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gnruiudo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pbvrsvwz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2myzazfrv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ponodvum.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2usbkbqzj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2oygnszdj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nciqnmne.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hyhjosob.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mnlagccx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tbuhsvfw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dupjfjij.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oxhhcgfv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhiqeayj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yjkrrgqk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvytzxg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2epubttrg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2yxxkcpsc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zyumxesa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hnvmbmqv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2scafuoct.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hxnrpyob.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2morzuppe.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qywefvkf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rsmjoasi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rexnupqs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2byjvohab.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hqinbsxv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mzurnlhk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xpzrglvd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fbhoxvnb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bqttqibj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2uzwdryoa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2avsfffds.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qyqnrzpj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lgfkrotv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2wmcyyhai.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jhshuonf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hkzyurnn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lrewkeuu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qxhhafzf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hiylfysr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2abdwugxb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kozxsaqn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rgwpuqia.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ujkilpll.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2sgukpbzf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2guedmjzh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2uqmhswhm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2uwahpcmu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fmseyiga.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dspubcwy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cyxiuyrz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ychrivkt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zxnmcjre.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2abdzttmy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ldjmlypw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wvrnsxsp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gxfaokpz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2axcntadu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwtvgvqp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rjcancvi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tffucixe.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xnzpibbs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ygywdkxi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2shtsijdz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wqbujpxq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bigukakt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tdasnfhc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tdrcbpvr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwsdivko.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wvwtvhnx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jzwvqsyu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cvigppzd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2srjlxgxc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qdnmrsij.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ybbqdplz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2smsyaowt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mamlvzhp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fztpjsqo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nxzctdim.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2akkkbxku.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2oxuzvfai.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2emohrcks.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2shxkamjj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lmmaclnk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xipoewts.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kzagqwkm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2romyohgc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wxgmtaxx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ywgnjswd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bfvivlvo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hvuonxzr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vniilcse.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vbkcplqf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mncnzqjm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rbqlamdj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aybghsaf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbtjjcx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ewahihla.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qzniezru.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgqqsnr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oefiaqar.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qzuupqmm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ffgyscmt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dfokjpqu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mhrtvvij.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2migwgmvg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fiujross.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xibwtyfz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ytgnoyum.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dkbyycik.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xemdhdeu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nkiettds.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gtxbvzab.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mkhtvmpe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dghxvlri.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vygyxwun.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2agldabit.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2maiblwin.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jsulhopf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pcxeplwq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fwsqqsmm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2enmnsufd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tqjyfuvz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oerjjhef.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oyxioyut.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vicfktco.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mdlpxqlc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nkijlmfr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2tpsmaufk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cgdslrvg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmgjiofd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vpzrycfx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2siqymapc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rqldqusn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mnsoyfyq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nbhzwkmj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2emrnlgci.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ztervvqv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2aozlbech.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2swkvzklp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2haorxwnj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tpsjqcqp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qllmbxyo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fsliypep.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mreamgfr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tdltocun.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zcatrujs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mstlrskd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fvkuaqll.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gbhtjilo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kzykibpb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ioerftpg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jciixjir.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hrmyhuic.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wuucrqfu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2axoybvaw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ucnvpedf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbfdfoyc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2odizfirs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2fnlmnxae.html


<!-- 参考信息 -->