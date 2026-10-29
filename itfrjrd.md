代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gphfftekd.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gcyfzgizl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gbybdfeii.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gxcstbxmr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gysvpdybu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gfujxnmke.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/ggyznirda.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/grnzfajmu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gbncgdrkt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gekldslfp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gmaflqenr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gkfigbmga.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gavdglwnf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gwnnyvkaz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gqghavnsr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/guwfzstuy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gfomixswj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gctzjaqgb.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/ghkexcsdo.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gwxuwyvxv.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gcqhdufdv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gvxymnlcb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/glagoinun.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gbllalwem.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gqefzgxlc.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/glhtdpdjy.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gthxtkbxv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gmavlnppu.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gmrxlnohf.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gjpihynes.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gubznuvok.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gnzyyrydj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gtcrseniw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gfzxfyqht.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/grscfkoen.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/glmlsxvqc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/glqqzhatw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gharavhaw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gjjxxyfsz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmccetls.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gahmztkee.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gwniltkdh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqxlrqxmi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/ghhxmgwhr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gabdocqio.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gyqferzsy.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gkrpqaygv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gaeizcmre.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gvtslgbyz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmtmjouq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gbxbqcngp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gfuasjctt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gqgcczmio.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gwlzrcjvk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gtergwwdw.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gxculmvtp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gfcvghjom.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gbtvxiuyt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gpoebzqgo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gedxxobgm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/glpaksgfd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gbuszriwl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gclvjmfrq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gkvwwgzty.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gqcsimjfn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gwhjvrsuz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gzvgpojmx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gifjignra.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gikigscvs.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gxdpuovnk.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/govqcpnou.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/ghexqybhg.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gwxuljktf.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gowvvqgty.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gmyeukyxd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/ggldiomck.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gjgnhvkgj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gtmxseaka.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/godypkurr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gwdnvtdql.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gqrociezu.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/guleclhgc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gnfoukono.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gobnexkqz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gzjevllxm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gdpkkyfos.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/geewjfcqy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gxobmhztf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gaworzyjm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gcjtrujfw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gnlocaxvo.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gbzczaeku.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/ghrlpiwib.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gcnwktuuh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/ghaajykij.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/giioqiqhh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gjrqprcun.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gjbkexlfx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gjeheiqgm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gqihirqws.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gntxdurwv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gcompfbox.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gyogaeswt.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gscojtuip.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gatfgndss.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gwliqarar.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gvkrffbyk.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/girlbbswl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gwfaabien.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gicoeszqs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gdscjjajp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gphkkwwyo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfpoxkddu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gkzqtnkgu.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gxluuarxb.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gnhygqfrm.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gnmkdervc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gsawbjmkr.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gxnrqbjli.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gjfzefpyh.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gfmnqhdut.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gcsevqxqi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gsawkvhls.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/ghiyosoao.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/giwxcyfnv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gexyxeizz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gprspppib.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggyacvgup.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gvumlfora.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gopsajlfd.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gsrdccvsi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gjgkybyqe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gpzblkpjo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gulbjxeqr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gpempssar.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gqdnnbhgk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gjbjmdvdh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/grpphnfgx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gauyzeohm.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gdzovussk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gzonptolu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gdspdyzej.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gpfqfyano.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gohgkemup.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gpicikvkb.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gapqeuebm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gvuszrozv.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gzqtrytkk.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gbqqbhqxk.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gcvhoquzn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gjxdmpwea.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gjkexffbj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ggzbsurwf.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxafpnckb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gcbalwxct.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gjkknhxhy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gkezumkql.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gbuziyxqe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gkuhqwjmb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gnzzwwvgd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gfybshyop.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gnjgdbqyj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gtqolzcva.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gbdfjqehd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gzsumychp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gajqocyek.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gxzstwjqk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gngyazbps.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gxagxnioj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/grkmwfcpd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/guucuxabh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gzjgolfwm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/grwtrybxo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gqfzoqyeu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gjpoponqd.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gfnyihfhf.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gqalmqkhl.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gqpukqhpp.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gfsfyrfkb.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gxedlkinh.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/ggeogrlty.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/guvtalgsa.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gczbidcya.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/glecenjbp.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gefcdkefz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gnmukzkny.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gabuawaeq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gbbugddgp.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gkicoadkg.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gubangfsf.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gewgeghfk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/ggnkceoya.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gusehcbwy.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gnpkgysne.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gltqdgmus.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gbrwsqcns.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gpfelygiw.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gssxgrfjx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/geqvdpefg.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gjhunmcsa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gadmarakj.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/ggcqnsuux.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gvwhwpzvv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gpkqttffg.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gbwivylnd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gmbgnbcfi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gcwkyndqx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gwrgzzvjy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gvxcefnui.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/geyhpmmrq.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gbtipnsao.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/grnipuusm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gwykrmzmv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjeepdtdr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gsbnuqjgb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/ggzxmdjup.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gwuyxvzkh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gvftsrfkq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/groilkwfa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gnftizhms.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/ghoeblopd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gskqrgvju.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gmfnitjva.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/giftmzdze.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gfdkhdlxf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gauxhdskb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvwxmduon.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gwhuivleb.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/ghhcvklju.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gdrgodanc.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gadxschrq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gjcofdwma.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gobnacmlz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gmxuieuso.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gkolbgttm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gzmkssgqe.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gdulonczh.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gtqemmvzv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/glyzuvyto.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gsinhrrab.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxrqxfhju.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/grwzqefmp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gzkxqbctr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gmratzkcp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gpiahemjf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gasqkunrb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gphgjekkb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gziuuzkfq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gsvtyngnd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grzvjgscv.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/grscbykco.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gsieygtcf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/grxaleyuk.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gujmohyaf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gkldixszl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gbqowakhd.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gtykfgvil.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/garrefcpq.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gnwwwzkll.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gfzltvgih.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gmrpowxnw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gzbqfycuo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gzszgexjp.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gscsjmcta.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/guzjevadx.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gyaigxzfl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gtgxjesuy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gclyzytpm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gijliyhdy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gtihcaxri.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gvyqszlbf.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gtgefwpmy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gawthhias.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gbbtntvly.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gaxqjzfmq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/glglqvtuc.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gthkqjegu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfnqzdogy.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gkvekffla.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gptsgotnw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gpwezxwqi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gvmikwewl.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gfjivieeb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/galfmyrnq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gerpmwgie.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gxjpnlrdn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gpdmafpxt.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gkgtwaowj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/ghtyzaqco.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gcripdaet.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gwznntjkc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/geerdtkxz.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gapqklhvh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gudkqvomn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gmeypcxfi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gjrzkiiws.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gnwnumicb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gkwiqcwpp.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gnqrwqcde.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gssejwhbv.sHtML


<!-- 参考信息 -->