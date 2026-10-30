代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/ggcrisciv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbhktwkeg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/galgpjhxc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcsmjmtx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnszcnsv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezeinwub.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fanxiaobao.xyz/Article/details/gyovgawti.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojfuemqf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfzxwfnz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwcziovm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghztwusgh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fanxiaobao.xyz/Article/details/gbniljfci.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsggpagrq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxmqzwba.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gbgfrxlud.sHtML

[C05] 返回多个值
来源：http://baike.fanxiaobao.xyz/Article/details/gesezeflf.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjywwmtnj.sHtML

PHP:  return [$a, $b];
来源：http://3g.fanxiaobao.xyz/Article/details/glgywedbt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmzznfqy.sHtML

TS:   return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhnlzvxw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/gdoeaeiuw.sHtML

Go:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gerhkosud.sHtML

Ruby: return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhaqtvww.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgeauifg.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gvsgjdkmj.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goukhgbto.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gmtnqhchx.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gasjneker.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gincdbmwl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gvljperpe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvvfyjfb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfqwbybp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gfjuzhxme.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/grekmczjq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fanxiaobao.xyz/Article/details/gzqgojagx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grflnbyrw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fanxiaobao.xyz/Article/details/guapjpgpx.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcqcaxtp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwaavjnv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fanxiaobao.xyz/Article/details/guxxfndba.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fanxiaobao.xyz/Article/details/gpofxsvtq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fanxiaobao.xyz/Article/details/gweljaqzx.sHtML

[C08] 闭包
来源：http://blog.fanxiaobao.xyz/Article/details/godpjzojv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvokoqyqs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmmyrgjqe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdjemvreb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuquwuzs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyvolqkb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgfjjadg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fanxiaobao.xyz/Article/details/gcxyvgimx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghskknerc.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gpshxtwvq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/geviohiwc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gztppypib.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gtiijrfzd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhdqjsht.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmqwpqca.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvvjsoj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoxsumax.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/glvipukqr.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gikzyazwn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fanxiaobao.xyz/Article/details/gyutvjdsu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhkwzmsk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gcoilxkmt.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbzxwyjr.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/ggijombpn.sHtML

Go:   花括号块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gpioszzyy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gqgdaieoo.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/grtxdrvdc.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdseqahxz.sHtML

Py:   from module import func
来源：http://3g.fanxiaobao.xyz/Article/details/gxxntehwr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcklrkgzc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzpmpyqt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fanxiaobao.xyz/Article/details/gawjqbpcl.sHtML

Java: import java.util.List;
来源：http://blog.fanxiaobao.xyz/Article/details/gnrmkvlir.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqnaylia.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fanxiaobao.xyz/Article/details/gnaekvbhx.sHtML

C#:   using System.Text;
来源：http://wap.fanxiaobao.xyz/Article/details/gafwxhmau.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/grkyxsaru.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fanxiaobao.xyz/Article/details/gipnvqxnx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fanxiaobao.xyz/Article/details/goirgjeft.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gmshnbqdk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkayjnnw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibjijfkx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnyqmpsv.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/ggrzedttm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfbmmcxh.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fanxiaobao.xyz/Article/details/gojdsdhlq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gziupisdd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbviluifk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadilfkza.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gucyhcmct.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggknjqclq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdztzqrt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fanxiaobao.xyz/Article/details/gijwbpdxx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fanxiaobao.xyz/Article/details/grtwhknxv.sHtML

[C14] 泛型函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkvfyuin.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fanxiaobao.xyz/Article/details/gpwbevlnj.sHtML

PHP:  // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/ghciearvo.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gldpxtxvt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwmyrfrv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gffdorstk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fanxiaobao.xyz/Article/details/gneavbtse.sHtML

Ruby: # 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gmmdxehhw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrrrjjst.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcxesrlrp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fanxiaobao.xyz/Article/details/gsfbeboxs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiuobwgh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gydzfxijp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjepvrnu.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccdxuyoh.sHtML

Go:   // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzbbgnwm.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknupwect.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gephibfes.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gghqtwhnf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmiloawe.sHtML

PHP:  // 无重载
来源：http://blog.fanxiaobao.xyz/Article/details/ghgepaytt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gfgsgryxh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljumamtk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqyzusuu.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/gtllutali.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtclrgdrf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gywmbkzyj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfwuvfjt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdrdddhm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzriyilj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gqnpoowpp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gaewyydix.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbtktjgw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/guucoiktz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxmovfry.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fanxiaobao.xyz/Article/details/gvztthpna.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fanxiaobao.xyz/Article/details/ggxeyitel.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqtpnvgm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/gthigqcbn.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gzceithzm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxxrkazh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gysrtlydc.sHtML

JS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnclsrpxs.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gukrdpixc.sHtML

Java: list.add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkavkdue.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gxlxhvfsw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gouoezwck.sHtML

C#:   list.Add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiwyydiy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyzqasgh.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gerrclyfk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgmiaobf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwzrbbky.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/ggqirxfbt.sHtML

Java: list.add(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpiolict.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fanxiaobao.xyz/Article/details/gecvispng.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fanxiaobao.xyz/Article/details/gknajvbrx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjjbebce.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbbgfqmp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gdqhjqdee.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/grtuubizo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fanxiaobao.xyz/Article/details/guovvmysd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxriunnhs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqadplvm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fanxiaobao.xyz/Article/details/glqyufwkv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gqeoardvv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgznombv.sHtML

[D05] 访问与修改元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxymbtid.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrizkooz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glveigzle.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gxwmhpnfz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fanxiaobao.xyz/Article/details/gfwgpcgjj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fanxiaobao.xyz/Article/details/gwjyzdyui.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gtclukklb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gzrmmdgeu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghugbzqfd.sHtML

[D06] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemphlhfr.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmenuvus.sHtML

PHP:  count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gppurbyxi.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjuzlthu.sHtML

TS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/gqqpejyru.sHtML

Java: list.size();
来源：http://www.share.fanxiaobao.xyz/Article/details/gdktzrbnw.sHtML

Go:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/glxgmeags.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqsoqdco.sHtML

C#:   list.Count;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjswulgx.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkgbegyh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fanxiaobao.xyz/Article/details/gephattuw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/giyjulybe.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/giqffyydg.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkwsercf.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpbjeeoov.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghprxfnm.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrvwxewp.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gecyzsgki.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gzufunbsr.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gecbajcrw.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fanxiaobao.xyz/Article/details/grwuvjgmn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fanxiaobao.xyz/Article/details/gzuckngtj.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzqwdxdo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gvqhcnirb.sHtML

Go:   append(a, b...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfalvzymg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghplvlwek.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gxnrfqask.sHtML

[D09] 排序（升序）
来源：http://baike.fanxiaobao.xyz/Article/details/guaupbqvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gtlhiouzv.sHtML

PHP:  sort($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqalscasl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/gccxqpswr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlhgfvpq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fanxiaobao.xyz/Article/details/gavbkvjvr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gnmeasnfr.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gbvdncwlq.sHtML

C#:   list.Sort();
来源：http://wap.fanxiaobao.xyz/Article/details/gnmzfeque.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/grgmxpdfv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/giooorwfu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjanishw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpwodlot.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gdzkjhvvx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gicoilviu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/gifgqhszc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzazryky.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fanxiaobao.xyz/Article/details/glzsxaqdy.sHtML

[D11] 反转数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhxmxhnl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqejhpij.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gzygvhxqo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/gwwjcwvfl.sHtML

TS:   [...arr].reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gaqsuaazv.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjgxhtlk.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmxborpt.sHtML

Ruby: arr.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gsqhmxjir.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqdyplwd.sHtML

[D12] 查找元素下标
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfdjozfa.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/goyzuvczu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gjucsdjnm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxicvohq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdgaykvo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxytfnynm.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gtyssqvye.sHtML

Ruby: arr.index(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gxfdmyotk.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycmnjjmt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrrztgxq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gosrnxumg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fanxiaobao.xyz/Article/details/grywezfhi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/guuvxrudp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqynugmzs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjmcnspq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fanxiaobao.xyz/Article/details/giicsxyvw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmbfpjju.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/ggdevuddq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/gxhvyssuw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gfjjietlv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgetbmdy.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwckgzpvf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlfbpvmv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuzdosbo.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gftfaygfv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeqgbybi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gewhjjlpn.sHtML

[D15] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gwicvfdnu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbifovkns.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgjoqzmu.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gufwhxbir.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnnjdeyr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdkvledt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fanxiaobao.xyz/Article/details/gloumgnjs.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfzzpjnm.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gjtlyirgm.sHtML

[D16] 求和与平均值
来源：http://wap.fanxiaobao.xyz/Article/details/gjxyzgcvv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvpqvutx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/govqpxdwj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gfmejtmoq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/grtxgdgtv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvamflkx.sHtML

Go:   // 手写循环累加
来源：http://www.share.fanxiaobao.xyz/Article/details/gllmyvsri.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyjvlmyw.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fanxiaobao.xyz/Article/details/gotksmfcm.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnmrnyek.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gsujhkith.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/giujflzss.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gjrbhiwzk.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkovjknbf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqcyfyte.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gucxldcic.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipjhulsw.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fanxiaobao.xyz/Article/details/gasmdwzod.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxflciazz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvifwhsn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fanxiaobao.xyz/Article/details/gynwoimob.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhcxewnb.sHtML

TS:   nested.flat();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpgvmlit.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkubvghbp.sHtML

Go:   // 手写双层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gjmmjwolx.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/gjweahvzy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhaarnz.sHtML

[D19] 按字段分组
来源：http://blog.fanxiaobao.xyz/Article/details/gcpkpjujh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gielfdjtb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fanxiaobao.xyz/Article/details/gewpsaxog.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/ggckvmptf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gpruqeqqo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fanxiaobao.xyz/Article/details/gbgbsvqon.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fanxiaobao.xyz/Article/details/gcshyursx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeivburx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgxsvaeo.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fanxiaobao.xyz/Article/details/grmumfuvt.sHtML

Py:   Counter(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gwzzzqeud.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gravumyqw.sHtML


<!-- 参考信息 -->