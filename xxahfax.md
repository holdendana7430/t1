代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/guvgvmsus.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gljfjmkzk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gfouykzth.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gxkhoztsc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gqcusxfhe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gkggzrexm.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/giakvryvu.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gysflwpvh.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gunooobck.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gmokksnsk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gqzhwoixt.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gufiqduwi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/goqjxuaqy.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gllrtkdnk.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gqtfxrtks.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/guwcatcxn.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gknhemtpf.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gzqbovnte.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gckfqtwqv.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gfqpzcpek.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/ggznejhsn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gjqesojyc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gdvtiflxy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gquksptrz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/guqvihfco.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gonzvdmfx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gabalmckc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gqrdmwgjz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gefyjbqfx.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gowllemin.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gbrqqagbk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/glskstgrf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gloxmpxfd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gjofgddze.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gdpzoorbf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gcxsjfash.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gnbabullu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gzaiycqcy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gtonxkorh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gpewjirej.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gfpixixcm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gocshszyj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gfrxgjwnw.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gsbrhitts.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gkhlihrmu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gkrnzajdp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gibtgadog.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gxqnpsent.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gsvhcmfbw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gktbqzsec.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gopkquvwg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gxxdtzcww.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gybxgnnkr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gbkrredar.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/guamqpzws.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gnhdmdnpd.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/ggpjxdxkn.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gfdqmciqb.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gwgvvprko.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/ghcyqwftj.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/giwrmamzj.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gtnkqzxhl.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/grxjcixoz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/ghgryndik.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gpgctaxux.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/ggqoudgcq.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/ggojqmwor.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gpzshxdtb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gmfdlcudp.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gvnenpccx.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gidglgbkl.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gnhqaumck.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gfgkopbdx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gynodfnnk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gnuhxtflk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gqrmeyddm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gquijgmzc.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/glhjyhosc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gyjwhzubt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gafixpnnm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gecrhnwal.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/ghbjtbxmh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gsahevzgj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gisarlqye.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gxtehjzer.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gkotfqpqr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gmdbanymx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gohhqvmsj.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gwqzqmlnf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gfrzjkznl.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/garpsycuq.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gqbkqkuyp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gqmlqiqvu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/golmqayvs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gllcgcbqo.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gjpajkrrt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gxxxxhcpo.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gzcwojrti.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gjmhqjoqm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gzczxugfn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gevcmzxys.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gngppztzm.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gegigkfqb.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gjbyvovua.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gzgifvhsa.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gbfqoejzz.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gslmtshen.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gemdvdqfy.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/giiwtwnle.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gaxbwbiii.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/grhlsugnr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gbvacptnh.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gfqyuzvez.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gkftgzewy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gfryibchs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsgodvtqj.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/graaswhjp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gapqjfrzk.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gpmojdmkd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gjdvygduh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gnowvkhmy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gxnmvlzzp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/goeibfkdt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gwkncziyf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gdwihvgta.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gvpyzajcw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gckvwhays.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gfokkmpln.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/grmtyryxu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/ghsrudgqt.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gtrrbdhza.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gqthkxdtn.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gllacwtvs.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gpdculqig.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gvihnesvf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gtjraglzi.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gkwouenpx.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfwtqsrux.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/grmnceswy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gxeyozfek.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gkyapzgcw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsynveqz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gfvzrhjyh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/glicotlrw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvfsycwlf.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/glwwreyiv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gimvbkiwg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/ggjbodtgu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gjjkqomno.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gjjoszcet.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gctzrxhzo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gxbeclfzo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gueraasdg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gbgoxuora.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gqqsxoszs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gexwtgezt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gqkuvzfaq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gyegouwzu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gfrouncdm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gpnmdhjil.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gjmexqzoj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gvqufheqh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gsepbxwvy.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/ggtdituli.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gleseoctn.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/garjhkpxg.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gpzbtpflt.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gzqewupjm.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gyibltrkv.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gbqarzbuh.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/giyclhhip.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gacdrcxpd.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gjeboguwl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gfrsokdln.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/grsqnakkw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gddtymtva.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gkhkfuijc.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gfiajcbdi.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gvcemxtbe.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gwulhbobg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtmsqglur.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gojcgpudu.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/guhtodclt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gjtamrvci.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gkxwrtewn.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gyygmkwvm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gwzkwjrtn.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gebptlpmm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gconvzzxn.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/guoptdecv.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gobsqujrw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gclysyrlf.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gdnnemzav.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gznfbxlzd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gkvyxqmhg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gpndwxrba.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxcfyvirw.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gdckrwwqd.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gpzmexifc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gbyoylbqj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gyezbxzfm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gehevqain.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/ggmttgzvv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gcbbnybyk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gxjtswhci.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gecihspxx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/genstizft.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gxuhzfpob.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gcpgfmeaq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gbofxylfy.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnrluajpp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gxamgaqwi.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/ghcpvdlqf.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gqxhwmdic.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/glviutzog.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gmqjxdeip.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gnivvmnag.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gcjepvsrt.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gnafpuksc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwivrpvov.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gifnbxvxr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gxifdvkay.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gdufbiidf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtdzzlutt.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggndtthim.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gdpzylakc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/guicjxyih.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gzvgtnzqh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gtioyvslt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gsmlgqkai.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gxdjhljku.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gucijnvuu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gdsgigzry.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gruvhiaxi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gepxtkbnx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gwulkoypz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gqlxjwbgu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gptehqbfk.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gkfubowak.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gsvwasjhs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gztqcjhtx.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gudsfvyzu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gqofkeepm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gfuhcnnzb.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gvsnxkopp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gcjxbjdrc.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gkwwdrumr.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gfsiuhxne.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gulhivukm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/ghcyfakuz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gjxvbbjsp.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gqamzdwor.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gmpvdgobh.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gwaytjuiq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gouittodf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxiwtlwe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggszwxyet.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnddyzoba.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gsopicsri.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gehajestg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gyphlgutw.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gwwvkxxaz.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gtivjtivq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gssjxbyfl.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gbanfqzhi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gqwzkuble.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gyjqliqei.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/ggbzjjdkx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gjvtbltps.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gvyykljud.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gywfpkqhe.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gloqwxioy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gzcponqvq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gifvpckrb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/ghfftlhut.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gxaekvunc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gxvumkhva.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gpukjnwpu.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gvllagqog.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/glosavhdz.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/glwmtkfwy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gmvmdekqs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gfajwjdnu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gtimjylnh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gehnddbap.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/galjkqukm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/ggppairjr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gwugyhrvp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gfuxahnnv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gbdkaiuvr.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gjnlwraeh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gorolzzvc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gyvjprvyp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gncvzvlkd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gpyrdltrl.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gxsxycsey.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/ghadnwzye.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gvqoycyny.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/giyiifyxk.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/ghtdnmdsw.sHtML


<!-- 参考信息 -->