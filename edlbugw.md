代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gekkkerpw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gpngfdxqt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gcrssotyv.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gunsrinbn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gzzoglarv.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gosfqolsx.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gptsigvrc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gepjccrzr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gxxwshihf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwthpdrq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gnofhksod.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/grbkrdmel.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/grttcimxu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gmbwwpumy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/grmrcgnpg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gyrvenjwo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gefffrtjj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/goadgyahf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gnxsigwjb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gswzbsucp.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/ghmvevwzv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gnaczdmmy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gftpnpxse.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gjminakjv.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gkhvdjlwu.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gcueoydik.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/ghlqsswxn.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gjknedynx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gmwsvyikp.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gjzjmrmnx.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gsuuimzge.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gbztjrxry.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gsicoryxi.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gshbfslok.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gpzkrlvtw.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gcjqrbwjq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gptkzsvna.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gpsqnjrfk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gzewpzirt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gsxvqhrvj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gkycbywur.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/ggrlmijve.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gjtbrhktx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gdcicskhq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gsegvcnrm.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gjbdwgwfi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gibbtkoea.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gwrbgtxvl.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/glilakuen.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gnpyswwaj.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gtdjlaokc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gmtxwrxim.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gjmzweoap.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gfuhvygcs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gfdazfykb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gahmenucc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/glifbcrwc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gfpfznyyb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gstvjoplo.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gvbzijmug.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gbivduinf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/ggarhsstc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gspghvgon.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gmbsjydnc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gszygnnms.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/grmeszagd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/grvbviahk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gjkoboufg.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gspwgxtvj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gqkagbpni.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/geyvbxqqs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/guxpgtbcq.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gatjhxhcs.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gomhglhws.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/genchrfwv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/giayvpbic.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gqkovhmxx.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gksrbeyor.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gwawrmzyh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gyjltxsjg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gonniapwz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gylyuykuq.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/ggeekoyav.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gjdcqeyjp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/guwgnwfzb.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gwooounvy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gxsfpeaev.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gqnngqyjq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gnowbwaer.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/grukdingw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gbezfimiw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gmolvzerb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gugqqlgzc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gekdkasru.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gwtucnffv.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gjsyfpeim.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gprqwjlcg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gpsomdeqa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gccceqplj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gqdumaoxm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gmmmxhmwo.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gtzcthpsc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gwytsunvr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gebaguslw.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gmxudmsca.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gboyvvzvd.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gzryodvdc.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gbnikwhih.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gfzcqczwl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gbnnqvmgt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gndyqzzez.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gbyaytdau.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/ghlmwzgzn.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gpmtbgzwo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gvliqrsyi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gdjjofqwj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gyhdhomiz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gkxneuksh.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gtbofamsf.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/ggqfqgexi.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gegymprwt.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gkojjshys.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gyorkvhyq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gyagrgoew.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gsdpuribe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gfwnzqhbo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gxizxzgul.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/guhbawuob.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/ggfnxuunf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gkkfhubvy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/grfxyoowq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grywrwnir.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/ggybchdsx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpjbpmisl.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gtbifasfz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gmaskxzmo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gqukstgxc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gnfvayxnz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gjhnksbcv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gnhbccqov.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gjvohorfp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gmrnzethi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gmzmmhdeu.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gqcrpuatk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gnbfhyjoy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gzzmuhfzp.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gafbdidlc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkgygotez.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gebdlfelg.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/guackxuib.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gmvwhqezi.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gbnalolli.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gsyxzwfsp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gaqtptmos.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gvzxisrjo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gxeedlweh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gkhdhvizh.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gfvloxybn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gpvjrojoj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/giewtvoel.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gzememkow.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gqajighwi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/guocawxwt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gkezcltmd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gezigfqns.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gdjtalbsn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gwsffxcra.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/goxdqzcim.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gkqppghnq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/ggcalvcuy.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gesjugpwj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gvuamevtp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gqzrhetuf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/goooiwswd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gfxfotpuu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gtkmeuklk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ghphxosbi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gxzvggvmr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/graqaorlk.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gypftungl.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gkbxzwvcm.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gnnuabiuo.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gtmrfqsml.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gdwiovavu.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gimndjdzv.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ggagfhvwi.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gsbfrgqos.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gwcdmmcgp.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gznedjaxr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/goeaifjeb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gtjkxvmnn.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gtpowybiw.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/goevwmdku.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gfxabxglb.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gknpgvyvk.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gwshbiolw.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/glhwkodpd.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gbuzrltuz.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gnxhsaizs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gqungduis.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gfrxtxtrm.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gxamoctep.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gfskthaxf.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gxnyoqxti.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gcowerhvq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbmlzltvl.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gceumzwnx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/grjbrizig.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gyemhqicy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gotrajjox.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gxuudpxys.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gscrohvfw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gduaugtjk.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gaxbtmelk.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gqnuapgja.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/ghrluyblg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gayxuxufy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gwxmyxwss.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gzkeisbgf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gainzvako.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gzukdzvce.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gxhijcswa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gepmkmdbh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/ggktppdkz.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gxtwszerj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gogauqswb.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/guodnnjzv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwaavsr.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/genmkwdxc.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gffvmtslc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gturzvkhn.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gulrltked.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gaixuziau.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gwxorfxhm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gbuxlqcyr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjwqrhuej.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/ghlkpnpmi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gytcjjcqj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gjughfjrt.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnwrwxdos.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gugccaprf.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gnxllqqfm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/goeloyhim.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/geiwmsdxi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gsaepghke.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gnbxdiazg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gylnzepne.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gpxgvcyuo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gpxfpisjg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gpxweifec.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gapdmekms.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gxrbavwla.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/galluubyz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gavrdjsje.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gqrpsbeuh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gvbahbpcf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gslahsgfr.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gngbqehur.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gwmohvrew.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gsljozlaz.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gclhxmedk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glvhuxsji.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/ggmnzsuil.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/giykvcscr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gliixlkqm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gufdyrcco.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gojuqqiyl.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gndikrrom.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gbvunqclf.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gctxoqoue.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/grcgjbkvd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gdznjxbpo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gmqbhhybm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gzmmsdppb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gkgrfoyru.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gxjotkuzg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gnbejdapz.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gouwhmwqu.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gjyzjtpzi.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/geeykrikh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gskehctrr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gkbayamqy.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gpnhvmcaf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/glhxrdeym.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gmyegztfn.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gslprqopd.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gplqbialu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gjwpgrrsk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gymlwofer.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gxeggjbkg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/ggigiobzy.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gpiuvixim.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gdshdvlhj.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/geaircexi.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gbidbllfp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ggzrfgjfo.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/guawesvqa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gqoxepqgs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gvsuctouo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/ggagkurhf.sHtML


<!-- 参考信息 -->