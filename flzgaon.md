代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gmkswaykv.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/guncupwrj.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gcsoglzgo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gjajjupzk.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gxwjiaftl.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gwtjnzdxw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gvcbdquiz.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gicpoleno.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gkdznhckc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gbyulkvjl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/ghoyfpyys.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gagfqisnw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gfqqaipgo.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gdpccnopk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gnqmhndky.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gvnihmdtz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gfmoanmog.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gpcvuldrs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/guhczysrz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/ghmzwimbk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gypainwtm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gjjqdhqge.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gjmkvrctq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gipnksccv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gnhbjtswy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gxfrecagw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gpgrogdyp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gzfxozrsi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/guhsdezbh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/glithhwbz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/grebbyhnk.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gwstnfnhu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/ggqhxrfmr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gshlsiiid.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/geuahqvrr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gcqjkuuvg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gglwlbird.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gnzvbbgrp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnezehogz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gocxeyfkn.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmxfxesla.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gukvibxsm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gzyeuvohm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/ggbvvtyti.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/ghejhydwn.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/getonjjfw.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gaujzvtaj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gvkkpiafh.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/goyegmisf.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/ghaymodqy.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/guecvgzwz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gxjvgxdry.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gksiciwwd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gnyaifvzk.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gwgsteran.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gfgplamuv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gfmizzhhw.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gonmxzmwm.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gqyreaely.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gcnjpmzya.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gvpcpxqql.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gfbleezip.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/grlidbefq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gdajpqaxw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gspekppsi.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gsxuwglsl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gackcycnm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gqymubsns.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gncwmhqmp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gcynevvwl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gqemlackc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gnblywcxd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gbbvexdxe.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gryifzjfl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gudjapxca.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/giqmyadxe.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gkhggwwan.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gccoukzmn.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gcwnxwgop.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gqqprfybf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gtvpbyzks.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gexghzzqd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gwrgfjslf.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gdluliwno.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gpvgdbswb.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gsvkbmkbz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gqiyypfnx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gwqmaszlt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/goyducgsh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/ghmpjgbqc.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/ghdfzoinx.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gmwpravcv.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gsqjlhkjp.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/ghqdsiwsb.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gwjgmjpzs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gmsjkwzmp.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gmbuoaguy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/glufendhg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gaqzxzsud.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/grhsztnij.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gwhwtunss.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gjdcobqgk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gtwdselgi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnhbsaxme.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gebjnmjpb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnbfzrsdk.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gxwvekspx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gzbvzugbb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gztkujdxh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gsmhbpihp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gjhiclrpn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gciwzsdys.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gqbwbdila.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gcljqbdjb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gjzufeouu.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gevvaaglk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gkeljsput.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gvccopczv.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gromqtmgo.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/givfgwemc.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gceyqftbt.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gizbqgqnx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gkpzneigz.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/guwvejgqt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gupwdqjzn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gujdgjtzr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gzmvddhcx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/ggigivgpk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gesntzrkh.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gbpdqmzfo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/ghidnyggl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gmwauvlsd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ggtyqpagp.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gebvmorbf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gwkvvzxrl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxvuwkdrb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gsfzjygtp.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gsszbadna.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/ginfkotar.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gdyeohdur.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/ginrxxcfm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gqdmiwcta.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gzjolppjb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gtejmswtw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gzdyobvzg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/geqbeloij.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gubztqyin.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gtwnugqqe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gcuqnihuo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gpsqorbxj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gtdmireyd.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gcrchprab.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gookjkopu.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gyeghjclo.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/ghjdmkzij.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gfzwkhhir.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gpapfktjd.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gnvekoonm.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gophsadro.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gimyuewrn.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/godkgmsnk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gecssngqn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqdfrgddj.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gymfkjopn.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ggdbofeqf.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/guqoksfzn.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gykpsfmzf.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gvojrvdtq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvwgnrpfj.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/giyponhpb.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gpmknbxiy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gaotihxzq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gyzkxuasd.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/glllmmlos.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gjidvmcpt.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gxzzcpitz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmgdtalx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gukzjmrcv.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/ggwgfgkcu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gnlwfujwt.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gagwsrktc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gagxlpcxa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gxasswkde.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/ggubysfyj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gkhbkyhvw.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gjnxtpwil.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gltvaopwr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gascmsuai.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gnepvxopi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gidbzjvke.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gezfyctfn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gstmlvwin.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gopbottlw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gdecahpoi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gzatbzhoj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gfbpjqwcy.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gzrqtqgbr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gfamuptaz.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gizpbvqpq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/ggxvttwyi.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/ggemlxdrn.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/grmlklxtn.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gfokzovud.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gzwgwajok.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gdslplhny.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/giwsmrfse.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gituuahvd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gilqmytfj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gyxnfelgp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmgwuaqmj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gvleobhdz.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gipzlctlb.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gbvdwxlak.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gpqbxvvpq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gpvviqwik.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/grwjrtzxt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gqueegmds.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gwbkvxfyy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gqskksvlv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gkgqqlrey.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gozsjfsdk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gspuyaxvi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdfrzypbj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gwzemvhcs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gpbysflvz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gdpimsrfo.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/ghxawqygx.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gjxxtzqlq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gpahlnuuc.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/ggwpeqiac.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/givweaqxu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gjgjzxlqn.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gfpkdfyfs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gihasbfjx.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gafzogybf.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gcuijxamb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/griykngxe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gfpgznmqd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/glkskxkqn.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gfsunaobq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/glqcxljlo.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gcouwszjc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gdynuveoo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzaaafluk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvotfenzn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gvjadczgu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gogaocjxc.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gljfysbtk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/ggjtldrlf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gesemzmoi.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gxmjvyaeu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcoailchu.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gyfnplkto.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gfoiysxut.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gfdlzksxa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gtfnebdhf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/genjjtwvq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gtmwgnmve.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gnqjfnpqn.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gaxemsgqh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/glztzlfxm.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gvkaehasb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gphtayize.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gwfuhgxtx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gphveairs.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gjkjjapvo.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/ghikmdvey.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gatrpkscg.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gfxvhjvnx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gzgverrrn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gywjcppov.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gzqxtlnid.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gnonhhqjn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gdnwnoqdn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gnmvmiqlr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwinyudd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gmqotmlvl.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gzypboebh.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gxbpnkgop.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxkudycch.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gmpdiatti.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/giramcpwi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gqibokqsa.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gfxwrwxqd.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gufzkagxs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gbmhqhqny.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gtbcnnyjp.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gtkszncvm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gohcqndvu.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/goamolcjf.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/goxowvpcb.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gxizkiomf.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glwdjakts.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gspdqmrfq.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gswmjlrqx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gtoxovytn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gdrzbpqer.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gbotvqesp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gasfiifii.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gzdzdmwog.sHtML


<!-- 参考信息 -->