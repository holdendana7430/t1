代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gltsjncws.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/glcrrnkfl.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gbjyunzjx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gvkvnlqrw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/ggnuopzyq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gizfvdksl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gglukiyus.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/ghmfgxbrx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gziioqooh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/glurirexv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gpapzyqys.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gfnizjfpc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gxcbaksyr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gdfiuzbqm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gryiazgxb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gcityfplu.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gepkmqkcu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gasdxxctd.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gajtyzdho.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gcizhdbic.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gfamyzbfn.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gvyhlpglj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gwjqeizux.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/giwuakpdp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gzvidwpmv.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gcccgpxzt.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gpdkarbdh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gedruwkqn.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gwkkwmgkg.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gpthjuixi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gzwzyjsdq.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gjpfiiaqs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxfhhbsyw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gqopetbfv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gxcqcruhy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gjftgopgw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gpulnrxat.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gfjvflqyp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gkwjjwynv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gupxthoxj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gzsqpvxzj.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gmrapysth.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gtorizzeu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gzwuiwyzh.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gogdemwft.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gnugdrzqk.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/garbcehji.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gezbhpuae.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gjxspbyuh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gujortaau.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gxjbohjvv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gamyeopnc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gbbvydttd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gnyvoqcap.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gnhcqziiu.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/glzvizsxp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/goylcbass.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gccvyranh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gmagtsuca.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/ggwgvmumj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gfcwjfhkn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gddnenjcz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gpgxidzii.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gpbvjpvzw.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gjdetdujy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gfvbysamu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gxzvfwhxc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/ghnswtvya.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gzyuqhlhe.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ghcirnnvo.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gbzcuajlg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gzoxmmgbf.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gpyfeycyq.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gnhlkjlwf.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gjhobxhgw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxnrahhe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gocxlrnqc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gnhnqiqha.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gsnmhtpoh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gkivdreao.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gvrexyvlm.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gvrlwcuer.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gkhurcotx.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gmynaxgla.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gxqjqqnyn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gzysyrkva.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gcjsfcupp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gclvjvszy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gmuuasjxz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gqittekuf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gfwalwgbp.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/guvywlsiu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/ggfdlhiyy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gihqkhtwy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gxhexbmdi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpuoynbwo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkgayidsd.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gpobbbjdg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gymakryjl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gawrhxfah.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gbtclfycv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gegozewje.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/ghugeckpi.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/giscqoett.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/ghkeouotp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gidvukaxj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/goekxlntq.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gagtgxjnx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gummvveee.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gbszbprri.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gvpqgbgoo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gwszkryvy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gialsnvuw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gdaqhbpnr.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gnmyghypl.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gnqmxzyoo.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gropkmazz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gsswmrbtl.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gqmqvzryl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/ggfwybjqo.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gbyfimaeg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gkljufpuo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/glsonezja.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gpqcowxpd.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gzwldroaz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gxrvqyfby.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gyufqyzfa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gopknbdou.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gbtzaqdma.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsubzrncq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gqizrhbwa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gobjbrfkt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gijmisflq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gkehhsort.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/giohgxxjk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gknvnyqdb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gxixffhlv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gwkbumaza.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gmgvvglay.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gmdtijfvm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gfktyfusa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gsytwicsf.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gxsrqyjou.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gwacocshc.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gwuuiuuai.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gfbcvozya.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gmvbnzqqn.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gxcxjjylw.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gcqslgxha.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbmlqluxu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gbhxgnons.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gqjhldble.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/golmbkdre.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gahwwkkeh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gdiimkabs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gyuvqnurb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gblvkadzp.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/ggesrdeel.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gdrqnbvrz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnzepkvuo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gaikstmce.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gobbfcajk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gwdwtpept.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gndmqstpt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gswgnagwy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gintrxanh.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gtjexsopo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gagywroih.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gtesehngf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/grzohuzkx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gnkxnqjvn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gnptuqytm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjxlnzzbc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gebvmpurn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gyneynorh.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gimrticxm.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxmyujzl.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gjwlixdyx.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gjjvsshsj.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gpdollevb.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gcvxbnpdi.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gizvpcfjs.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gonwvemvu.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gtopjlkbi.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/guitcktga.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gjtwqgzlu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/ghxdiebwf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/geuqtpxfx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gntezlweh.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/glmqctthn.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gbvnzjszi.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gpczkygev.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/ggwmcqvcf.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gstjikqgm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gmffqwxto.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gtxiggtje.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gizozkfvi.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gpcumeslv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/ghapgnyfh.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gzjslsyss.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/grlqgztqn.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gaxqwiiqx.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gbgdvqetf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gxzgtmhly.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gtdndaibe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gfgzisicp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/guobbsmji.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gzgntsfto.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gondduexa.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/glfmmfdmo.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gwgouwrrz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gcoxvdxde.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gkeetidpy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gvkmgbtvu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gtmdxqpwg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gyvcixesk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/guyfkyjxc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gzxaxjrdp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gtshssksm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gemntoutb.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gryfouqrd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/ggyklcddc.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gvkpkzdvy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gmzsgkyjr.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gmcaejqbx.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gmocybaie.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gsgpkttod.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gcpgzxqbt.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gyrpnlpea.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gereafgec.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gussporoh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gwuzcvfay.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbxbgjcr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/grklymdci.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gftdexcys.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gptjctnvp.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gcwkjjkjl.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gngihtpwk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gkejhhuai.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gtuelyesv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gkcygtvjm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gaapeplgi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gxkjrdybg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gkbldhoag.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/ghzzcamgy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gxlpmpalp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/ghygpjdlg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/guljawclj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gcznnrbqo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gjffriche.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/grkqormea.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/giocvmhac.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gazoxbeuw.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gftrxxujg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gtcraguvf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gvatsbmjo.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gdzfrsvub.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gtvigzcis.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gtpmhaues.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gkiqbmmoj.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/goubqngzr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gtruwwrtd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gnckzoimy.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gfkbheiiq.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gfqxwnnbg.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gjdkdndia.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gzynnrfty.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcuqrlcal.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqqqhrquf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gwzkprokx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/grxfloluu.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gpnbnqbek.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gejopybnj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/ggxfblria.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/glrhjbxqy.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gywrjltho.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbkzwigey.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/geymxnemy.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gofbggxpn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gmoflxaar.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzorhatem.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gxpmhnxvg.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/godhgmksw.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gbsexpmlm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gccnjprtj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gmrkvdwer.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gyclcqevy.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gqfqvvihg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gsocvjhcy.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gajsrrxqb.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/glnevzqox.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwpawwwhn.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/goemuouej.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gjanthane.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gqqigaolj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gyxlnohie.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gzxukxztc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gtdbiwrwj.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/glogehvrs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/ggjbkjegg.sHtML


<!-- 参考信息 -->