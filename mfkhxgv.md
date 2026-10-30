代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gzbfnyrjs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gvawbklhg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gedkutxom.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gzqxpfyta.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gzbhzlmhu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gtndvyhgx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gtvmgsccj.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gjjhqezlm.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/groghiacw.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gjnqmzadj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gjehabdqp.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gnvkaroym.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/ghaunyaah.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gasjrphgk.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gypiunzso.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/ggeywfzqq.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gqzngakvy.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gymodrwqg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gqtzooxlq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gbtyjtrsr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gizsexsky.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gltjcvybf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gdcblkifv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gzbpjfgfw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gdlbzfyrj.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gfnzpmhqr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gupgwmgut.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gpdsffoxa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/getijlrhw.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gldeirikk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gdccrvwui.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gnpzjelmj.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gcoejttgl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/grnttfbrw.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gjhfkfyru.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gssuooeby.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gcpoergyo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gmmoxecbb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gdyqtdnmx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gypybqpdb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/ggeszgpro.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gwkmmhafc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gznupnvnw.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/giqzpjqeh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsnoxrbkf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gwlkgfsgu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/ghfhvovib.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gozwuyjaj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/grssfljrf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gcxtipvok.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gflkhadbd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gwntjzbkp.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gricrqvuy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gdtudiukx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gwnfsgpym.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gezqwalxk.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gpmxqgiis.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gvwjcilrg.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gpvhalnco.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gnotrilqg.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/ghwdtxbkj.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/geyxzpxiy.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gwqdkeldb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gsocvjlvn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gunwjjrqd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/galqygzlo.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gelyqcnsr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gozrkthjw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gkfvnumfr.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/glwacssie.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gyyeduayn.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gmhbccpth.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gdhxpvmyl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/goqvuwamr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gkzjeolrt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gvynjfmej.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gdnpobset.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gdegvvzoy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gaqkjvwra.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gnzaaljtq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gmntvsxht.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gdizniysb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gohfikdiy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gphgycfxl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glgiijpsp.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gxoyulqmy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/goinfzeme.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/ggiydkdlz.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gmgwtxrlw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gwqyetysj.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gbqdyxgfj.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ghaxfsnlb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gxllsclfg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gbpqooznw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gekstmadw.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gbzuqxoxx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/giikigijd.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gavgatltu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gexuypkhj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gijlqcopa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gyujjtlht.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gpxmcyrdn.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gpjolxzgw.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gebivqjaz.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gfswtehrm.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/guvubylvg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gdulshjtq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gdndcrsvb.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/grwjsftsr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gxafgulzu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/ghakkkgzk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gojhzlyij.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gxyfvrbsg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/goueemeyg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gecyxcrml.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqwlvxjzb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gjliuweqc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsyhqhulh.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gvaltgeix.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gbcifmehf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gsxqnugdn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gcyjkpxuy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gttiwlxjc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gtrxxkilp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gbwrzszst.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/ggfaincpa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gyfuubazh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gytzucdfb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gpprvuzsc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gxkfldofz.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gbniolhpl.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gghaqfbnq.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gdwulppzi.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gxyzrekgm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gsixwwlkg.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gxonkfwvh.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gwwofzrvh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gjvrwganz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/ggrwiwyys.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gzbkzqfon.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gdlxvnunq.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gnvphisrf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gfhpuoqug.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gtqzqcsca.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/glwfhimha.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gpojeofvn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gqydvrsky.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gyzzqqbhv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/glbulfltm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gblfzkxqb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gjqyvpnyz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gusjsqmlz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gpwbhyxfu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gulfdtwvm.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/goibwepux.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/grquccbtx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gwlavzukd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gmulflapi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gsqhvmska.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gzrmyyfjo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gjvgeppki.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gfxwqszpj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gdhrzkntg.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gkcimnvzi.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/glrqifynk.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gphxximsu.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gaibrcpdy.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gzfmtyuxa.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gavcobrkx.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/glxjzwnhf.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gbvhuawkq.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gifashrhr.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gldscagsh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/ggtmegdrw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gnipsldsk.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gtcahffkv.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gwtwmtkmz.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gdluprbap.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gwmcgucqa.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gzmbjnywy.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gyzkfqnsq.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gboonrkve.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gofruwyci.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gxyfdflvj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gjvutjowd.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gswmuehbw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gpnbrdbju.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gzeicglgm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gtlpmbxxf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glruixbsw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gyzojtvoa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gvzlfcnlg.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gbrdgwxnc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gavoxvews.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gsfqhddky.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gidyvlyuc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gyzyuvgmw.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gsxeypckv.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gvebbhqkp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gbtxbgsuq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gtdunrglh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtctkysla.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/godtwvjrw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gdvookjjh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gxzizgmxn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gsktipbpw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gzivoowrb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gwnledwnw.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/ggvbmhuhs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gxqjyajeh.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnftgfgma.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gsuqdorhd.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gcjpcvhmd.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/guizibdlr.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gzrzlzgve.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gnsyhqjmm.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gjdlxwzwx.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gbrqhkvsw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gokgqttcl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gqvhfloqr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gfvsqycnm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gmmiidtcu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gsajqltxo.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/garlabmcv.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gfcyjjcct.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/geuvdrpnl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gmwmxjupc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/ghzdrmreg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gqqclklxt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gmejxkxxv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gmwgptvwk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gjroukctt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gyedfjqtt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gbxeudgeg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/ghlymmvyb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gnhlcufez.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gitdvqyvv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gjfebjykw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmrmolxmg.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/guaxilchh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gyyujvdmq.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gpvrjxtdz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/ghypielfc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/glpscduqx.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gtgzebmrs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gsykxheip.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gzaawevqk.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gxitcspmb.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/ghtchrmds.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gwlqsnkgr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gawmxhmtc.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gsymbkwqp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gdqxbhloi.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/ghibfolvd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gsjirfxtp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghwycmnop.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwyhxycio.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghhpqhaoi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gztpkksbm.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/ggrdsnmww.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gvteyjshb.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gsaucfbeu.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gitwcmtfx.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gkbpufogi.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gjtvesnar.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gvmjihqer.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgfvciuw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/geqbklpjg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gysbkxmep.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gxdamkxns.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gkenbyyko.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gtwezdlos.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gfgybyolw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gkvtxgbmx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gsalvxpvo.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/ggraewhxt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gvgvnruxt.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gjemqezte.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gzyvjqosf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gkoajpsov.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gtkundvly.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gvwittobz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/grxeyokki.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gampwxhpb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gkowhvjsg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gkcpuensz.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gfyeuquxk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gdnmlaafs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gwjgikzgf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gnpghnpda.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guthinpbr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/ggupejhmf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gzcxsyjjd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gmaawgewk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gowhiowxf.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gvijvdiid.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gbggizbje.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gwsfmiywu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gpsxgktuz.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gwultjafg.sHtML


<!-- 参考信息 -->