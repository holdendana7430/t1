代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gtlqgwuin.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gdgmdjwyq.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/ggoxsjsuo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/ggorxanyx.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gxazrxtuj.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gbluvnlth.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gewyyurlg.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ghctcrcaz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/guhggxqxe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gkvqzpipw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gcbocjyct.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gmqaomrrs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/glmeaqywx.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/giycztkps.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gkaqvhizf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaqivpjxx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/giqbcnwnp.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gdksinlbn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/guipgsjer.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/glbuqyalm.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gbldutqad.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gdrkbomsd.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/ghtyjzjhg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gljsupfnn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/glxquzihr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gskyonadu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdklunpcs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gwjbsrbac.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/goqcadixh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gumskdkne.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/ghpvdlqdj.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/ghnfdfpzr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/golattnlh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gysrsdfzw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gjcblslad.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gvbgjncpu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gauenangh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/ggmczercn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gpoeruwya.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/ggzjuslcr.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gsjamvonx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gzwoqjaho.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gvtwasuit.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/ggyvwoors.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gmmhtsajj.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gyrywcquo.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gbjxvvoze.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/guewndlmh.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/ggapurtmg.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gcpawlgin.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gqxvipcdc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/guvgmdayy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gzlxpwyri.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gmctlrzut.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gqlcmblxr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gzdxrypkg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gwmkowgod.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/ghnifnhdo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gfrflcaha.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gbxnriorc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gnpugouci.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gvbdprmst.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ggtdvupeh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gxivsvjzs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gpljyjuqh.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/genlszjvp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gdpnfqyzo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/grtuqycjg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gabainzwt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdalxqsao.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gtkprsmiq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gtqycdvdf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gkxeoohdr.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gouypixil.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gjrpeqrmt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gwufnmsbw.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gsjqpzmgr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/ggwgqndsd.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gxtndvver.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/ghwejkbug.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gxnruvcxg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/glesnjemf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gudtqhspu.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gyqujggqb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gkbfkiqat.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gurhkectq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gewmnmfur.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gogijcwvh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gmflyasme.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/ghvuepopp.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gmxpdhlaj.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/ggneyerqe.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gxpwfervu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/geweofnle.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gnpbyccqo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gzziddriu.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gximtphpm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gkfzwfemf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gdlohtbek.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/ghdzbvvsy.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/ghomyvonh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/goqtlpicb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gnmkloojh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gioepsvtm.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gsjosbioj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcvetcyru.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gxmxtsuox.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/grlojrsqp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/ghsgpfhzk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gfvwpibtn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gblmkkdds.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gwmwajkox.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/ggctvznkj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gvbtipyrl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gqgqtgaoy.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gxwjnifin.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gcvbxcchc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gltbhxxfu.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gazleppnm.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gmqwlfwda.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gcysdswpa.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/grntsfgra.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gxkadzedx.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gpdishnpa.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gyouwkqkt.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gvuxegepu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/geujuvxaj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gdmxsjprj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gjmougszj.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gujnlvakz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gxqahqvbh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gyjpmypgr.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gfypimhnh.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gnzmcytch.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gmdvdcskp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gnwufvoer.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gveyuanmg.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gkdmpoopl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gaspolgut.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gxuwsxvhr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gmqtizlpf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/guihiihfm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gbukkkyys.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ggfydgxnl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gszgocjha.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ghsantfnp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/greprqvjm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gllojrfja.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gbmblbqyi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gzgpauslt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gdvtcggrp.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gmkuhpepr.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gsbzluxlc.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gzvvwnbxh.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gqfsjcogq.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gafzvefji.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/ggxspdtej.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkvfqdwlc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gdxcytoij.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/ggdbcupvm.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gowwkoksd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gxeoudiio.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gkbjpnxls.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gzvedzimt.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gzgtbecnb.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/guxtmvhcr.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/grtsqpztp.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gpuhcgubp.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gsyjqytao.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gkcjvyxzj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gkrewtewo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdfimilw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gxrqhthjf.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gunptizav.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsdkfzxym.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gviypenoa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/grlqrmrcq.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gikdcnimb.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gsgucxkvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gxkvndsfn.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxegrcilx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gxhetqugm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gmhbmtmsm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gwywslxsn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/giayxelhe.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gmswwzczg.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gjldancto.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gwaowpffh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gmuwoxkrg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gcizwdssj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gneglsvdw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gpdoqkjpi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gisrabwsk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/ganhqjbxj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gwozjagod.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gqggoetdo.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gftykzpif.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gtctuvrhq.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/glvcnaeez.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gjkeogvkz.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gogqdging.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gsebfabzu.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gtbdldefm.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gbfjnomzz.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gglpbzyrs.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gxiovlyul.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gkmnkolpb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gkilbkjrg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gqnuntaic.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gskozufwb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/glwegsspk.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gzhgdntno.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gswudqdxs.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gbxhsdmvp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gltaiwkyb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gjduisxrn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gllsgzwps.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggleydgvf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gegermhzs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gpvykdtfb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gbgmvhjdd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gcgwnudio.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gmkqbdifp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gvxirgjsu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gdlegwfqx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gxbqzvmfj.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gxzaaqgli.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/genjwuqeb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/grnhkmiic.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gkvntcdqu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnuiadwlr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gbnvabrpv.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gzskplvxv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gpgbwtaib.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gesejomzs.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ggmjodczv.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gkntontau.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gyoszjpvz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gsihoogii.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gvmrfozks.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gwdgluael.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gvevniteg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gwbvxxszk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gidmijzok.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gyiqrqkkf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gslwiswql.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/giltpewbr.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/ggvszziay.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gkpxydczy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gkjpmaatj.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gqejnoikk.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/giipmbbuw.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gblxfmgwc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gogtqfxjl.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/guooliomt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gpuqdjgnn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/ggyvhjepf.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gcmktwsev.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gmzirinwh.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gufswgcdc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/ghokjjcxp.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gfljaythj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/grchbfuas.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/glmadxxuq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/ggqistmgh.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gcbkoyxla.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gbzxwyvfj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gazjbzate.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gghecpcro.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gaylpmpsl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gdejuumgh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/goxiuzycg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gsonahvud.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gpzxgbbez.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gazlewmtj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gthrnrycv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gdtxsacru.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gynlmbyzy.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gbkqpkgjn.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gygekqyak.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gwqtymiwb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/ggexhefij.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gurzjaooy.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gifnbawby.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gbdlgbqth.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gvucohvpk.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gnvxkgujv.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gtxfbawfb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gufeakwyz.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gfednjkai.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gajnjatii.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gnpjnxjvg.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gpwmhkigb.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gnobisysz.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gdcaqhrcl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gqesamzwy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gfwrwjoar.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gnvrwlvbl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gvviavcur.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gcmbcvxmd.sHtML


<!-- 参考信息 -->