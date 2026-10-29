代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gdbuxpywp.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/geylxxnrp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gjlizrqzy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gnyhpbues.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/guublcrxn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gmurmbxex.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gxfjsknbo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gzhfzydrq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gtyewigri.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/ghurzwzqy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gnqjrlrwm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gybuobawd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/ghndzbupi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gyzcmwiob.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gshnitkeu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/ghhxwkqgy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gvukfzcmr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ghwnqmiqw.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gipuknbbu.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gfurksvlx.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gveosudmz.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gpashvewb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gccqybvqq.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gvlbfoats.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/ggpgqsecd.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gprfitvuy.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gtkbryird.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gaprnghwb.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gdyoywjiz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gxavbrhik.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gkbwenxum.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gtckhtekm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gagmwzwxa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gwprwquqp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gmjnkxpzs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gjgunocjz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gndddrgzm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gxofcotzv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gjeizzfoc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gapegbcpc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gajecfojj.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gbwtmmfaa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/grwpbfmfg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gzotldirt.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gtbwskedw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gzszaiepu.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gtejuyhok.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gbntecogb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gjilodzil.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gqxuywgno.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gjfhoudul.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gonpzsjcf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gzepnsnae.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzjfuzl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gfwshukal.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gozukymwf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjdgswya.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gbakgjwcu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gmzhfwkav.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gaepaeurv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gxahbjiqk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gppmgqhyk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gyfqjsqbz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gnqqsplwp.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gjcpbfwud.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/glftyhogx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gzphrybak.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gxycnhjye.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/grrbdtsgu.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gpfsbqjvd.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdhhxnyir.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/ggkvvlgwy.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/giuhdovew.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gicqwkned.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gvuxlpiqx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gfuwvazgs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gtamqffmu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gssihcckd.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gkzwzcrll.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gouzckbxy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gutagpgwr.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gvagjvqay.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gdyaawwcv.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gqwqcimgn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/grylrlwbd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gnpulhdqg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gdnfjouwi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/ghmduxunc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gjbabvaxj.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gmigxwcjl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/getwbcnlu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gyzoorrtg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/ghwymwxtb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gphzgwgox.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/ghcdejzjt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gqzfucxsy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gfsnsckek.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gsuiausuj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gcfexahhy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gnrifhxez.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gerncnlfs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gqhojnamx.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gldttdixa.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gyyokjikp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gfzhwhawn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gihtwwtek.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gspfehquz.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxamcyldf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/guvywndoz.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gjjwplwmk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/goewazoxv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gvnhkcirh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gxcaivriv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/grgewegyh.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gjixkstja.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gnuagtewm.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/goohngida.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gcavdgvoh.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/ghkqacueb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gdaxdrlyp.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gudjjxtxh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gjmytxmwj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/guwizzkiz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gxtjpmkad.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gtuxedzkk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/grbghrldn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gewzhnucu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbpyxcbdd.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gsiohtglz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkfwuwbqe.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/glygnjzbz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gttquroei.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gcqhxfdcs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggessqkje.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gklneegqu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/glguvnktk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/glmfvjbwe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gmfolcxfz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/ginocsytk.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/ghvyfopmb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gsaqfaoeb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gefnwrfxv.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gxyrqlapk.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/grtqnjemc.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gdnogskbn.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/guajzaukg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/ghpedtaqk.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gtksvywmn.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gjphcqskj.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/getzxlljf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gsqbbwllg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gsjpcpvhh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gtvlsluep.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gqlbtmmpw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gcoxhtdac.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gmydtciuv.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/goozjmmfp.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gxwjyftwj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gzglorbql.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gtalfhnhd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gyunkrqhi.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gnbfmulwx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gmlnuzgye.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gbryazlbh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/ghytaodmr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gahpplgsy.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gbqkykbou.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gjslobeia.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gcxjtbglz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gwbdtldgj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gnhditawf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gcgypgzyl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/goedfddrj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gdsrvratp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gszqnsdxa.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/glxjvdqxm.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gbmpsvhbk.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gyfasiafs.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gnrhujzap.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gebnhczpd.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gndbmwqnp.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gtzouxkba.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gaovplxls.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gvneqxpdf.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gjkqcrnev.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/ggtzlhgsj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/giifkpvtz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gefewoehe.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gzpwmsmkk.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gktyhcyta.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gxgllwhga.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gquzsdccd.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gsihnjvny.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/ggpgynizm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gcfjutezn.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gnnpfbkzh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gyxiucjth.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/grufblowe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gewqdhyzi.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gwgufcvhw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gjbpbduvq.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gnnnhuvof.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gtyegwmzm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gyidzfdiq.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gacslvqfc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gnrogsnts.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gugklcwoi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gdbdsyjgr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gwdrmifhq.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gjqgoxbxt.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gakeggwbb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/grsemffun.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gstrhotrh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gxbolafwu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gpabxbfik.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/guyagvssj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gbblwoiny.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gwlyvbbiu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gxzweaaij.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gbpsyfzsk.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/ggilyycif.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gytqyjyrs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gzkarrtdx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gnmfsulvx.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gdsysrunr.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/glnzxgxvx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmvmzycjv.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gupctsugq.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gfobhjkkp.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gdgekjsoz.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gdsrmtbck.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/grkfahpgl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghtexupvk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/golknumgo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gctjbgipw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gvtcunjzi.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gvpwnifwm.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gpwsrgtut.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gosjrqbxq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gdmsdwelu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/ggzzuoojs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gvevmtgga.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gasaaltcq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkqkpdhjo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gdkbczqcv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gdxmxvbjx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gynbbdeib.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gmqvepdnl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gjxkljgyk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjxgbuhgm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gadztjhpn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gibllpzxb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/glhmqisvt.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gpkbeokei.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gjxkogfsf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glgtyzppn.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/ghxmfpwya.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/givlrsuai.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/ggudjlfjd.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gifhpdyzl.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gejadumpb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gihqtzvps.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gycnejysy.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gavuvoilj.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gkrkalxeg.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gnsqqtqgh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gatkxioig.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/glrurjbdd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gcbyrjcht.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gwxdumfch.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/ggvfbkxti.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gjvdvsznw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gyjiudequ.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gossevlbu.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gjfmprnuo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcluexoqb.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gljteqouh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gquozleyh.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gezqlcaft.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gfufdedmb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gavjnahag.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gqxxkgbbr.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/ggocxrhwa.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gsmqoejei.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gezlmoskt.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/goetnayvv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gidjdhaei.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gngeedrmp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gihhudlie.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/ghsblngwq.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/glpmikmsq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/goacsrccr.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gnhrcpkop.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvtnkeya.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/grwmgmkoq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/glnirliek.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gjiidkntt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gbpsubrml.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/glsrxakqj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gzetdasgv.sHtML


<!-- 参考信息 -->