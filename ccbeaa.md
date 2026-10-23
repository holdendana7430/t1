代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fjeilwcv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gwobqudm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ruvkmhig.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3krvmskaq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3orxlcubs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ihrcoqad.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mttijwaz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aplwodup.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nelwgrim.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3unnsnrdo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3badmgobs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jlzdnzel.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ceicwnsa.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3knzmitnj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bqmcvnnn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yorltpud.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lpdrhrvg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hgvrfwzt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gpzkrzqz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qfjwbehu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cawkrgyr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fiohpyjo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3giplaoff.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zzbwunvd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lxugoefi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3grjnulle.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hhkfptwf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qsrhzfst.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wmfpjfbv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ysxhylhv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hqtwgptf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3alfcpzmk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fjbhzhfy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rafgteht.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncmuestb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dfyfavtt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3dhbeuthp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dyzctbhm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eewmzwbv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bxmhaelc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qwomzeyn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzafndjb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3sefsaegp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3afpxrtek.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3clkgowfh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3jtlmcwvp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufhzlqvl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3uqvrtjuq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zazxibmc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hjjqkmwg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3meurhweh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rwkzjdae.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rblwgdsu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zmdhvqkl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3prhqleil.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bqprbnlq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qixgcsai.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bpalhpgt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ckjlgctt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pfcvwoep.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xcebkcfw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pnxiuspq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kjjsxfbh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fankctcy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uacivltr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jeakolil.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fhrqvyzf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mwnrhfum.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zcolfnfi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uullddwa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uitlutdi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cipaomgx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3faabgmzm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xmgdplqu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ounspiwl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3hgwgwrsp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kcyhypsr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyxlouee.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3uijvvfhm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zujztyvj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3niymiptf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jxnicdbe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vqvvaeqp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qtwjnome.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3peqyswza.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sseqcnhk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lysiwtlh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pspznvnz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3daxovkaf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mdkjagqn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3lgfuzrzi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hvlbazgl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3atdnignl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kuhhnbdt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zcguqayo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pigwmbgp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3asmujygt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3swxgndra.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ncufuoek.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wmklutyr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nkzmrnat.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qwmwqjws.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3atmptrhb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3offrtsob.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3daipqlih.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eiyjkiqa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rkxbscdv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnnhsmlk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hgcpjdqa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mxtidvmi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swmusgrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhkalwzh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wvsgraat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jranivme.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3elhhpnfl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cokfucct.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rgzbukry.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gfxzhauu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3sitmzbxe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hczsdmrz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3uawkussb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ggmxjszg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fhlnlqbj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3watvrapy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hscaqyjw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zbiydnog.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nijumiju.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fgbfgpqe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3sparuexl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3itmvwgpv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3bryoxtzm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3moxchfpw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3yqzedwqb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vpxczmed.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wewindzp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vtggkpzv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xfxmftvo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fhkcjqsu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqvmyja.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mprzckws.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uajnvyyu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ikgddohp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcnlsavh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmoeezbq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3okcwoklb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3uzpnzkyv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vunkwsht.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zllzprzm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jnyxunxf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vwsymeus.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3pniwlvth.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cpkmlngd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3srxjlapp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eygrmvzq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3phygocwr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vmxngezz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sbbednag.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cnkccrgj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yrovgdzo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3otulkwmz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3abdcecel.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inwsrztk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rrhdikky.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nmfkkbel.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cyhyoorl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wltlihln.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3uzbureib.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3itywcxai.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qlschcgf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3osvjkxeg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xccrzffh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yoozobev.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xcwwdlae.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3shuxojay.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3skufeoqc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3fbyvetsc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hqzaaxcr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3eoazkbyz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jqqvscwr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sfivyige.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ndjvfttl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3oouvubta.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3aqhxajfc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3butwgmua.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3njgvpfit.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ewepzkwj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fcoixtde.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jvsizpuu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3auepmvca.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wicfmvtn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wxsfmnwx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jjtrtojh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3basebfnq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vmkbhhkt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jlsoirhu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yvmkewaj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ngjqkgbh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3btfdiucr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3umopyton.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wonmgpnf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3doebmrdg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wvqbtvzf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3iywoivmz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ybmgqyrm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tntftmxa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3cdsiynrw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qazdyzlv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3izzibmyd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jaaegsec.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3defjrsoh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bphuikuj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3apfcebfg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jaoqwhby.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ocghffva.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dmplytow.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gkjopexl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qwbijycs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vsmeotom.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jnqxnixc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbazemiy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ahbsvuub.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fdfsftse.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3hwmaxgzp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3brzxxzpf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3guxwbkzr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgpmlndg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3burmqkpk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3coarghpz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ppleuqkb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sahevael.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rdtiyupb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vbvsgmwf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ticwwdpl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3drctxzqf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3amzhwvlz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jeaymdho.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3npkcjhmw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sidzprrt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3shdqmoxj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fmyqzumc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gapbxfsj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fuxyvpch.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jvvjhimn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hoptkuen.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ntxfzjnf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3vstuxrab.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3keysejdx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3immfmsem.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3wviahjgt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3eonwlwvg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkleiyel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acwfvhai.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ukougeul.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kfdpmgui.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3aomolvpo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lszzylao.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3oghwbowm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3duaeeosv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3anvecctv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mcejkuoo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gxpajnro.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3scboiukf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ynpcwjbn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hrmckuvu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdhtdpf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3tfkvxuht.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ownshppx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tjwqhzgc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zbtlnhug.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hhpytfho.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3cprpnvws.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mmhtpzcb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3cyuzbecy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jffvwkff.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tovkffzd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxkyhftp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3brhmoyem.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3bykbqhup.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3mydtrfui.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3amusvmaw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mqvjgcbh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ogimszfo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3subqgzmd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gqhfiooi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3lumawuqp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xfeaeeum.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jtxucngg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ojcpvcav.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eizuigaw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vkuubyef.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zutvvvhe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kjkryglk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3oxwqucux.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ojblfncr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gytqvwxb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mpjmouvy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3nlcfubag.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3socdwwjq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3twlxpsoo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hsokgymu.html


<!-- 参考信息 -->