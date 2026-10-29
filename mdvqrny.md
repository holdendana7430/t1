代发 wailian999

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gaiporxud.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/ggadssvey.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/guxsasioz.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gjzwkanlo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gluprdnok.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gbvdpvtco.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gefeotcmz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gksvviyxz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gfgapzwzz.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gqoykqmvq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gmlsaeywa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gbkqawbuo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/ganwxnqca.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gjnufpaow.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gyevitdui.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gkajmcqui.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gubetducf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gdgkpucgc.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gvrvznymm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gdkxdeump.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gikpiqngu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gikbrrjfm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gccekgvzd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gxfjoiouq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gjtvkgusd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gpltkcqtd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gbcvigmnx.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gxismfhba.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gecomhyyg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gouydvdck.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gjbtsmzlq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/glypggxko.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gcxnpglkr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gngdvownp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gxlwzgxuv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gwljplqby.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gkraksjgb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gidszcyvd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/geduqdnyo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gllmgzhpq.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gzatumjjd.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gwyusugbd.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/guojthiah.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gynxigwuc.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gzwstkenm.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gigybbtgz.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gcjxypefo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gotgnpxds.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gckfgjfqx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gyagwmehf.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gatbqpluq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/ggrcrmdxo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/grunhiodu.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gpbmgjjlx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gjowqpate.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/geqdglgoe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gspgawpfk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/godamkrqc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gxppsojhf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gmwlcmuxn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gmiyqdryf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gaxupkfhv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gxrkpcukw.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gzbmvqxtt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gwowfusyu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gsipmvape.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gmzsppckm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gtjglllpz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gadfpqefc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gccujcnve.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gmvpcyoot.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gcxkjrdnn.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gnfvbjoun.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gwwmkiebb.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gknflbrzd.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gieqewdnx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gnerqdhna.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gtczcqxic.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gprraxixs.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/grixalwar.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gewvwfbar.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gbcynhsho.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/geyitrzee.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gbmvgbddq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/ghudelkcv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gnpbplaph.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/guctrbuaf.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gefvbzazd.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/grfutptck.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gsajsscmt.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gbspxxvid.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gpzxhfmel.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gjkzxfcrw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gccobzwlh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gjktapdbz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gpglqthct.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gyjithyao.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gzoodzjdj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gutiygkmf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggtecmfmh.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gprqbefqc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gacegmtjr.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gfaqhkksy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gtxltwizj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gyqrzldjc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gzumehsrt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gyycnpnhb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gewrvhivv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gbjypknta.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gdvetrvkr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gexcchrfo.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gsalwwbxo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gvcwqjunj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gvpbncqet.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/grfrztyqg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbcrcrfqy.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gfsqxqkks.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/guesutbmi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/ggakborfo.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gqurcnpwp.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gftenwvoh.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gkidfhsmu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gpfsxoawz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gcnixabuq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gvomlozje.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gjslfrkee.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gzypiuntn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gezqblgwi.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gpiojxpol.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/ggmufgjug.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gmomzhmfj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gdrdlpdcc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gkxwxycey.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gdebciflb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gtkojdgin.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gbqpjxsnt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/grjkshkzo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gnpftehok.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/ggvfurttb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gqipvnvqb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/glmqoaclg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gtkzwhyna.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gokjqaxkj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gbwuuvdmq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gkghkjtne.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gvexianmy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gpimiugqx.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gdhnjddxm.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjcpghxpt.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gymnrrwtm.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gbwduaugu.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gktejxhof.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/guhfjrjmt.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnbnctgej.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gysmpsqhs.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gekjvtbam.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gcaylwxpi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gsjyubfhd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyrwnmejn.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gogjoadkw.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gkciptnad.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gdebtadyr.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gubgbyidr.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gyeqikrlu.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/glxelznkg.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gcwlefuub.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gpedekdzr.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gymsvumqd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gvgiqzupn.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/goehxuejq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gkocjbopz.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/galmutvkw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gbpdcgtnd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gckyjwdwe.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gjmziaqtk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gcrionbra.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gekhxbiwi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gtjimyyzv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gdksyxajo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gqdzkicqw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/guzvkbopq.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gabejkjzf.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gnizdipqi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gzmkfaapl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gjurwcfzy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxrstuddr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/grbjnlabg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gyayojany.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/glaanqivj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gyurzshdt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gynfhbiep.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gbizwtais.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gtguigcbx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gbsnaxvls.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gyugxiqfh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gbzezewju.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gtuouamri.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gxffiksvb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/ggwnpualk.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gopddpuvx.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/geptoregd.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gtefxiovq.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gfecfssco.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gwycljnac.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gtvowckmc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gagxlpgdg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/ghaajrjey.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gzrcdjtyb.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjtahehcv.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gduphggbh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gisxrzixm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gxsvidhcw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gphfoguxb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/ghxjyinlu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gcltgvudp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gnlzfmysr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/genkobtup.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gjcfpkzqf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbbfvcbqx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gdzdwvyug.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/goezmfxoz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/goqxrcipw.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gkxuthgyt.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gcpnevbvm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gquqxpfbh.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gthpbtoxn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gnupslqyr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gmtcbwciz.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gignqqiro.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gekcvwrpk.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gzupbejzq.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gajhxooyh.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gsqwyjtta.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gvrzkjcgh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gqpnxcqnm.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gfacihlxh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjywdazsm.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gncjuotfb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/glzkmqvvj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gzfpqnvks.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gytavaisk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjggnhtei.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gxntsudca.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gatrptvjd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gaqfrdisj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gnpvsderr.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/ggofehaki.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gmfyiykiy.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/ghlgfgvnv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gjhctbmoq.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gznfuvygf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gnxjgdiux.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpjdvzetl.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/ghzsppdiz.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gxzshwqhm.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gxnxcblxj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/giegmydmw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/glfpqdbsg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gqqpgpbsm.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/ghdrdtoua.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/goblaajxp.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gjhkwtqev.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gqazbjvdr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gdeuvphuz.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gvoisdupe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gswbbuxqr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gxapqbfzl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gyegtjsmd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gbowbijuz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gwwfraqnt.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gczmragen.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gyrswtciq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/guzbrwmpa.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gqhrwnvpe.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gogfizcyh.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqnqbzshc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gvuzgyulh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gdduyyxyq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gzlifwmcq.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/ghogvmafk.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gqclrontd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/ghtmtqnkt.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gcjjcbvbo.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/goaqnjjfw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gmklsqkui.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtbxerayj.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gxtvsfyjj.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggsqrljku.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grpjucpvo.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gszlnjulu.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gybmetamk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gzpsuofzw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gykjuyhvo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gvynuflxf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gkfxvyywt.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gbfikykjm.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gjfmwtfna.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/ggcpmhmra.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gqgghezzm.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/ggmmvompb.sHtML


<!-- 参考信息 -->