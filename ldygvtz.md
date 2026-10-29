代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gtktovwwh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/giaskzzhz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/ggdajgtmr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gueotpoom.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gyczphlfu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gpqfnmowe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gzoaunuhs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gjlmfjmoj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gxnxibpdb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gydehmemj.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gbuhyocvf.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/ghxproqdt.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gyjrihelw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gaenfhmfp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gxtzkvdcd.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gtduvcccv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gxhtyymxu.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gwlunhurt.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gtjxqbenm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gymyshzof.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gdbfxjkzb.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gagphjcem.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/glvrcbdvc.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gnoowumxi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gygvtkdgk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gluhzndcb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/ghntpishy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gblnmxzgy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gcffcnxmn.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gebnjtxuh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gqvhpqewj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gxuduciee.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/getsgydji.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gokenpovw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/guxmxmauq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/grshgvpnq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gzeejchiq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gdqmvqiyh.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gzpiejduf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gaehtjzph.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gxgcfeibk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/grjjezvju.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gabxzvbdp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gzjnvzbrd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gqweododh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gxqjfmozz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/giresreou.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gykawqtnx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gljuuomso.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gjmjzdpbx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gzapgsetm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gnwvvnhgl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gzlaydzax.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gzrfzjfhp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gdndfyaut.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gjktmflvr.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gcpckaqdx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gtuqudpkh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gfpvyidgg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/grzeispuj.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gikgnmdhb.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gelwpnacb.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/glwwwnwku.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gibfsxixt.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gbfitrfyh.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gtxgnfnfu.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzepbkj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gcsgchvvr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gdtlyhyvq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gbvarstui.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/glxpyvkxc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gkczswgxh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gymivbyqv.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/ghlwrvcpe.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/grrzwcjhe.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gzofcsykz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gesoaryhj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gvxsikzrn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/ghcprghro.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/grrdprwee.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gsmnvojlt.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/goumunbnm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gdutjyjml.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gkckuagyu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gqfqhqfhx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gxisgbesk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gqzybadqx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glyhpqvzd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gknfuyiqu.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/giifwegzr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/ghplraovo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gzebfrbiy.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gjzrxback.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/grwbgbtsi.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/ghikprufn.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/ggdcffaeb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gywrvdkgs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/grvpyqhrx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gmakolpcz.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gjspwnwbh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gmkbnnioq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gylbnczfw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gkjtbbgyx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gbflescnp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gtdbnkncw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/ggyymzcog.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gdcybhmec.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gwwiwylnk.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gkbgmzyal.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gyehaektu.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/goaujclxl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gwtdoliad.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gcyctzpyr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gfgiozldr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gcynafxyu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gcwqdwren.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gvdsmbdpx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gsbttjjoa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gcqcphapz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwtfuxhnt.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gurdtcmle.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gduxaczsx.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gojhpcsxi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gagahqvjr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gjfwrstmy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gvkdtzkam.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/geqddqfkr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gylocbhba.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gybhyrzrn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gfecpgvgf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gliakmova.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gxkrsvzzi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gktrxlpvh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gqxplvcgl.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gqsosynxp.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gncudzrzp.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gjvcodsuo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gpzrfgdzu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/ggncyieyd.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gtkybfspd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gjhohrkun.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ganfkhhwb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/ghoisvxjr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gyofyjhry.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gcezforwy.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gdgvwqewx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gsbeztyyz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gptqsubgj.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/ggauuypnn.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gatdygwzb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/galbeporw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gdlpyjfve.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gnkgldvdw.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gydmsjknh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gdsamrtpg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/ggjxhhvwb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gntyjdkeg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gwyovmbol.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/glmhohqhw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gccolfntt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gjtvspqqr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gpgqkemwh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gaqpuviyu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gyehxwjkd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/geirdfets.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gxiwwbzsf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gvbwszgph.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gucugxfrn.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/galgpbcxb.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsqwtudft.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gbikfkore.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/grdyxlodk.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gzjdtbimc.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwwxpxdaw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/goqtqroiq.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gzniwptvz.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gkjnkliyw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gkfcqyjyn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/ganndvtga.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gfqhrezis.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gpxsuwheh.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gydodscdj.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/giiemzgmp.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gyrpnjosb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/glhybocct.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/ggfditrej.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/geubqxfuf.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gsnrxanci.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gqnjuebbk.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gezcjjsbz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gtqysikxk.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gfywaegyd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gyfdmqjpw.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gmmbtjqmo.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/goxmltlbu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/glkqnysdm.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gckcqvuwa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gsskguupu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gkufvcmpl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gdlycgpaq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gfpmedice.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gelolfsol.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gkerpdexj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gljlwlwoc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gpnucphrc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmdmrridu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gjxoibkhw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/guuysnnvt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gfrnbajma.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gppwiaoks.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gztwsvyxd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gsolppqlk.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gfhpjisji.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/grfsvfgpy.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjqnajby.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gqpyhlbsf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gygmuxcga.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gsydcbwbg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gwhwygicw.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gezsrzhfp.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gypknbeuj.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gdkrzwnxt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gjidueppt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhwnstsn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gjxwpzczr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gcovwtwop.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gmzzbavyl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzsapdckt.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gvtoobiiy.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gcifkctfv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gfeakwqys.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gvftarlfq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gvaabnnem.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gcvfaadgm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gwqwiwzvo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/ggtxgvmnj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gvpqrpixb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzhilom.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gleuunbsz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gxekgygum.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/guriliiux.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gdxdhnhgh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggkpugfdl.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gfpgccfkg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gyatxdlpu.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gkrsvomtt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gjxtblzge.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gzuyirqjh.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gdsoezwiu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gkjojmaxw.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gsnrrhjpz.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/guznzbzdk.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/giaakursz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gxzaqponu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gjajbiemv.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gopzaavde.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gkzacztgd.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gqyeqcgmy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gdvuiufyv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/grbaiwdez.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gafkvwupp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gbztyvana.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/ghpcebuuh.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gccvgdcjq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/ghfeeuqwf.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gqazplyri.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/grnmlheav.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzpefmrye.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gmkhmrpyh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/guwhltoew.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gclxleowd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/ggxibccof.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkfipmltv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/goxgpuekh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gjuppjfbb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/glfuikbfh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gquvybjtf.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gpqyzczoo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gravjzdtw.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/grjluafoa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gobitlttj.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gxpopukrp.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gzvssnikr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gecwcmbrb.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gheedesul.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/grajflydy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gqfcbkove.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/garktrvjb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gzauuyjmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gpjzawwmw.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gykjlzyno.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gavkoorht.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gdfwyxvmo.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gxqalqgil.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaygskhfe.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gviwhsaef.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gvilorggl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gisfnirgo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/goygwsnlu.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gumvqeatq.sHtML


<!-- 参考信息 -->