代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gbxxjihbj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gfxwhadbv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/genfdenux.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/ggspuimml.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gkssmkcmm.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/grjhcmwcj.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/geqyzjpnz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gcatotlel.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gbbaurbuu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gikiaekrj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gojumrrys.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gvzxnsnue.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gyqdyuycn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gbhmwejsc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gbdwxzryi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gsnvnlbaw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gzsrdxkbn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gncapisqv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gropcdnbj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gichlqlkv.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/ggtwccxxd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gvctgqfpp.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gtdemzazm.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gehpsjwfd.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gumyfjnmr.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gukzargqc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/grzfvdzgp.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gjipcegap.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gocekqeor.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gxbqdtiib.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gfgwmobvo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gcnvpddup.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/ghfadfgzh.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gcrzsqill.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gttjsyfmp.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gyigdiwyr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gchhlpezx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gwewsbzok.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gzowpcscd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gizgjxydd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gmxdglaig.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gsuysbilj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gcraelalm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gyonpvqwt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gjucfhzaw.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gndzkrcmo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcvmvtnnr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gkfmbpavk.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gbfmwnhqp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/geholhavo.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gzcvafzsv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gjpwtmsik.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gncalmkfz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gwokxplzz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gvcokfzpg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gplpmgdjb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gthaaexdx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gijrybefa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gkzycrovh.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gdgksrlzr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gklctsula.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gmeyxotvu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gjkpunxir.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gniyikkqc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gukqgxeff.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gttrqeyki.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gnerscxty.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxtvthdml.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gnwgymnud.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/guwkyjrwg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gapmfwbat.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gbimghmyu.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gcxielvzl.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gxfteslxa.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gwfefymhf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/ggcrpsvgw.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/givwakyff.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gzexefskf.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gssfdbcjm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gibyxocmj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gkovuqtpv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gbfnothjk.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/giwlkhnra.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gnuvtvfdg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gqeutraob.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gcuwlrxjb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/guyavpafb.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gnhxkbjnw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gmhfmmgzm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/grfbcytme.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gwgvvtqie.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gggapjnou.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gtbmfoftt.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gcprbglhq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gbmfeoszc.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gndamqwwp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gdlnwqvof.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gnjrbohdq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/ggpvxnjpy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gvwkcutds.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gezuxaiuy.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gfzhifarq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/geuhunirq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gjcuirutw.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gkfgoxuao.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gyfrwajdn.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gmgrbmanq.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gzemkbqkv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gwqrfmtez.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/glkjbdjan.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/ghixhhdot.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/geigrhxwi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gstepdzuw.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gvfbnipvj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gdfrjzvgw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gmqpcdgvd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gvqhdcvci.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gaqdjcahn.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gpqeutbgy.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gltzzauzx.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gzuzdqkbw.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/ggzkzfusi.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/giadabpbq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gemrccbzo.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gjgynwbko.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gozssvych.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gvheigcty.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gopaprfqi.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gpwmvbiqn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gotdbhczf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gkbbgpdft.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkygjuqmy.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/ggexulmqt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwjciafst.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gbpdoydzv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gowonfprb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gebguhkul.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gzdjzsoqm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gbllqugpl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/ghaxbaxuu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gfpoqpziq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gmsbxrpqn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gjljrmmod.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gzzzwolgq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gdamvjqfg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gevygeumt.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gnvllvcdd.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gahtdizey.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/glajlpkju.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gkcbdqivh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/ggzpgfsqi.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gzdgnvboj.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gixfsyfmj.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gkgefxrcu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gccsmuwhv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gfspxnrwx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gwqjunvpv.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gacazwqcy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gqczcldoq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/geheoawpv.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gyjrxhihd.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gxvpdirhq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gazyynhsn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/goqcdpxso.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gsvbcxmlj.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gzjupjurp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gngbkhkxa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwthgatfd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gtqyaigzr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gbtllonma.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gqltarlmq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gzjefvoyg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gquyuwfzz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gkwmkikex.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gyzpkoavo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gjnbydvzl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gxnqpjywa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gdglompql.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gizkbludn.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gyomprbim.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gpkqzqhjs.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gdmrajiqe.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gsoaxvfhn.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gzupxxuca.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gewshiisz.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gjnphujoz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gcbtnqovt.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gmsgcuvkc.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/geyuctfqd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gmwgvsftg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gjeisndmn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gudslxdvy.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gdnlufhqr.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gzfvmisar.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gjefcsgpf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/glitaocnq.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gwwjeddgo.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gjqwgiwxh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gdfislnxq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gcctcuvhn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gxolvdgqb.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gcndtmdah.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gkanywckw.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gbbhjzufy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/guvdmbbqf.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gvqiaxgxt.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gorvdsozf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gwnplwtce.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjmrmkuuk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gniwkphxq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/grybehakl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gmluzfoqz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gvfijltab.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/guafnxfye.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gbdlbbcbn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gknktkzwb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/ghplbonaf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gtnbyxgld.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gwnxzwtkf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/ggqbjlmgf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gsvgtvovg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gavpncubi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/grsdxlpzj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gnoemmpra.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gvzvtmaxg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gjzgzwvpt.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gquoigksp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gnffwcnwb.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gvxwpkpab.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gtsmccahg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqhysrepo.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gdvsdgsbd.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/guwboxaal.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gnpjrilhw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/grsfzgslo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gwkuwfedv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/grcubfpqr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gxzgvqlgi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gaajvauin.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnihmbpnh.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/glgdlarrs.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gkcvkhzia.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gticpjelb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/grwdhwmql.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkwviuov.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/goxdgcwvu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gcajxoogg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gqnkaguqy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/garfjswuq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/goxzfxepe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghskxdiva.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/glldszuzf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gkfikuydl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gnmfllwrj.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/ghhwmnldo.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkemtprye.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/grmokijom.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gzjesuudf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghilfzhcw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gyhouilgc.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/ggxlsbzab.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gfkyxegfh.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtbwqukhl.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ggayymazw.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/genagjuzk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gykfnutlo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gqenkwsuq.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gdttnrass.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/ggrzkxdmq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gfeecmkdj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/guifvwxgi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbdvemtgd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gzfsbaqsq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gvervwrys.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gkhoeaose.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gqwzmdlko.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/glydnibtv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gxopuewwz.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gnpmbedlv.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gowmsmblg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gczpsdbcw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gmjzwyqfh.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gvzzbnbeu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gzkpmcycl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkwptoafy.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/ghoxltxuz.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gsjpxqkej.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gkacslfqf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gflsmrehq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gqwumtdah.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gqpbcnbck.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gfomfkdcd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gfzdjfmas.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/ghqdonnoe.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gsrmxwadm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/grthpzuwf.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gvlvnxycd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gowcfkmwq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gucytqbxz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gmezlnxts.sHtML


<!-- 参考信息 -->