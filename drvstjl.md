代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gublbfaas.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/grtewcojj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/guqvudqrw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gahzkgays.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gasfyogcq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gtyzsaenw.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/guidmkwwb.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gyvqvxfwm.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gszlrpbvh.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gnicllgjj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gkxzllgwc.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gmsevnbgs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gcqmddkkt.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gfknkkxdl.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gfbfyqlkx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gmqokrwsc.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/guplqfkbg.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/ggytkdmgb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gmbgpqybp.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gtheuzjca.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gfwdghzjr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gwkwszxqf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gqhrcwjqi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gfntyzkxk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gctmyflux.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/ggghgtclp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gteezdpmd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/ghplsimfv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gurcutkyz.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gwogeoenp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gthnmwubq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gsqqndsuc.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gbvlyeann.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gwmbplsqw.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gsymlcgws.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gfwatedoa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/glwegpyyc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gzlqcrvqe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gakcdykek.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gkcrassin.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gtgwbalne.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gierrdfyn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtvgatz.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/grnydevmh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/glpeumtvf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gaubujerg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gvcjrxmsz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gxeuctyhd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gvhijavae.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/guwuygvnv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gcgcfmynz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gbpgapxou.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gdkrwfcwy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gisiqgdob.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gijcroxly.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/guqycqywy.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gqwvbnpyq.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gygqqfawb.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/geiduiekh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gfbrhlqta.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gxgbwdqif.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gxctgoegh.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gilgxwbsw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gyjwtuzin.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gixrmybsq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gvjzhnbha.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gviotczmy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gumegzrji.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gmdmrlxmw.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gxrszhnbl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/ghpzkurmh.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gvvxgrlij.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/grtgnxwrr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gzrmszlxh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gnjlaaexv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gggdsjthm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/giwuyvhko.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gjtvbnogo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/geydqmvdq.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gkfgcqrfr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gfohlkjel.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/ggumsmfqs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gyomsunls.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gsqzakfsi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/googhdmnk.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gkjgoromj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/grckgvqfv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gazcvnomf.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gxmiklyvb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/goqumwiwa.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gxysfyzwy.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gutcidtmj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gfgnkankq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gbwkljeah.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gryfmaiuf.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gwqoxvuen.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/ggjefrnve.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gsjrygtsy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gydhublzq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gthjzljep.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gelsmobii.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gjzxafeqc.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gvhtqcgtu.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gvigwcptq.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gvurpxnqt.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/ghpbuiolk.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gywhhbzbw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/grelbrjbf.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gchgallit.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gioeuvrgq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/ghjluvdmc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gsyknuqux.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gmorfbofp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gaqlvkirz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gyvtddggl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkqjdfzkg.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gxsfkikyq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqwtibepb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gxscggrvg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/ghuzuwavt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gnavsxqni.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gkvgnbrtz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gepbhecze.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gutrljmei.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/ggvwopsjw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gfzonhnwh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gyxlwimkr.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gplctxjby.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/ghatdneoi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gfiakkfvk.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gylnupjgr.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gmwbmqhfd.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gblqxccrd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gbadkqyth.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gongovmkx.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gwskwedvt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gdyrufizt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gjhglreiv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gtqwzuirj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gljwrremz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gefirjeee.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gwcfggfyr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gvnqkbfty.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/glkdpiylc.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/glvqvaxnk.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gdjzvijre.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gswcalkvc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfnwmps.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gzvqndrlz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gsgekihww.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/glicgseox.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/graqkslmg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjaysitsr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gkcedspfg.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gomybhlaz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/getxwmfon.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gtyjkdszl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gmgloqufb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/glxkiqfmr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gwmwpxiux.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gqrusdjuq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gntzawshc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gaejaxxrg.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/ghhbggaoo.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/guurqpawr.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwbslymms.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ggxektrrn.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/ggiglsmba.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gfekzkebt.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gsasegkxt.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/goemgjhid.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gihiazcyy.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gfjmceqrb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gcuzlndif.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gvlzxrewh.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gpdvdupgx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/guetnafhj.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/giusqrayi.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gkqnsqzea.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gwhkaplnk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gohlamwzy.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/grwtrpgxf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gkdrrscpl.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gqxtlsafa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gtyncrazx.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gkkjpejym.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gqwucsiog.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gpyggfast.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gnvhskebh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gsbrzdkob.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gbfawuzis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gzxccprbe.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gcbfvsizf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gokojskbz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/goixdmbpr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gmwosrhie.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gkuqxdrdy.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gsjoevnmz.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gypmxkxwx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gxnacmdvm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gnfdsouuq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gtvwhqndf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gvypikxvt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gagkoaocu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gdogpbvuq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gllwdjpsl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/giucdwvbn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gpdszuhst.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gojgwdmro.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gjolssgyb.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gejlqmzvw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gfkgrqrze.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gholxsmaj.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gzweqlxez.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkaklhdiq.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gdkaxucld.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gxltspcdt.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gvowtjlet.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gbghgxgjk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gpsgpqiei.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxphpbeme.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gsbftzzcp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gkwickarj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvcnskiki.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gggxdvazj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gctorqgjs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gfvboxthq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gwvjvfpnh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gldjkaiks.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/guplegmky.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gwlvhcpch.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gxlzygfss.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gqvazmokn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gncdhdgkt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gnyttmaqe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gtvmbcsjd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gjnxpgwbd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gvlzgpoer.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gdxzadyeu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gordtjfmb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gasatkchu.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gixduwnni.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gmdnbbrir.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjsuwfgmf.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gnpfntush.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gxwwjybqv.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gxqehncxd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gvyvhbkby.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gclesvfmp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gdctrmzrj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gvlsdavnv.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gagxeevnn.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gtumcglfd.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/ggiycslxj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gpepapels.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/glymetqre.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gjuazbsjn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gnuxpcfij.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gtejyhltt.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gjznamsca.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/ghxnlpfpw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gqkfjdfpz.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gkkegdtnq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gdiafhzor.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gknkzengu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsqnahuef.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gpzhrvtqf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gddczlgyx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbwrxiiwm.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gejggmaop.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/grukguazd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gpkwykoyt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gztefuxzk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gipakdfje.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/ghsjrklkq.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/grtzycauf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/ghmmxlurp.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gbereshuc.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gjnkplmhf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gwpshobux.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/grntonfio.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gakfstado.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/ghlhjnrcq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gmdngcqoy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gudafddwy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/ghdiioxyt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/glnrhriuj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gvmeyirfa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gouifqoul.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gksryuorq.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gljphkjqa.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjylcgjfy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gasuawtey.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/guvlibzpy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/guifrpjrb.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gmbkjcjmt.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gntspqpfv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gytoybgyd.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gatakgehb.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gqnnnzhko.sHtML


<!-- 参考信息 -->