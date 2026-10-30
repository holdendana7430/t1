代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gdepjzxzu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gxwhrqdok.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gncmkwmpp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gswfiyxxp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/geuqghfli.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gvxfaifgg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gnxfxbypj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gvvqwpcqt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gdfwsteip.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/ggokdjmiq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gdpibwlze.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gtfotcqxv.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gprbkwqrn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrbsedyw.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gqqcbneqy.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gjzbtdnux.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gotlsidlf.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/guviksvww.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gwdieibkv.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gpgjchnwi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gafkugmsn.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/giibnfezv.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gvejcbxhl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gfkvlqhru.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/ghcsgmuur.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gdyszgtdt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gvdxqfshg.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gmpghskuh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gtayivvsj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gfycglvcn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gcsfuxecn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gyjbkofkr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gqbdmoogi.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gozkzhijp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gkylsqcoc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/glypfqhrh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gqfpmzdcr.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/glvnpzgai.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/glpdisbck.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/ghheeczmu.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gizuztwbp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gwclikbow.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gxpbwrlcz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gjayqwuhs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/giruwsoiz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gnhopprwy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/govqteedu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gvlfbnlmf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gwjxsvddg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gmstghpcu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gzqfuiymz.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gpotlihwq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gmwqwdevc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gdcdgkome.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gdcuxwres.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gnrwahruf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gqjooxcym.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gojgwqjiv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gxxrvumxd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gzhifeyik.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/glkzhrzii.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/guetxxpwb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/geotgnyyz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gjkcaedfz.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gkbklksse.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gkbvinlfk.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gwtzphood.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gkhyuylnj.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gsjvovpog.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gwiemcbpq.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/ghhlljkxn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gsmlnurnh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/giuseiaxl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/geoncysaa.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gsdlypvyh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gkeaodzpn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gwcljgvvs.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/glbcflevc.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gagemrajq.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gpkhishwy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/givylqwmy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gpopfapcr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gahdjktxe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gdykolvyt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gwbszpqhc.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gtkoxkfsl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gagptvrra.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gffvhgdct.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gslsuadmi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gwikcdeyw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gbcdbiort.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcenamhrk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gedqlugbo.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gxijheszo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/glclpgvfn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gnytybvgc.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gokhpbxhc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/genvofima.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/ggtaedptt.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gkisjpdjo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gykzqeibd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gimsgcier.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gbqxjhihk.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gidlzlcoh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gdhhtxaiw.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gtwtkhuxr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gnjggpgcr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gsradsupc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gkrvseioh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/grxmsotex.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gfgnrofvt.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gmtlegvcr.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gldvuwefo.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gshyolwvj.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gqboqbyqb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gdpvyowia.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gzsdwalpo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/goqgvqfna.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gorqyagxk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gldgezvcx.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gidloboor.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gbecawwcg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gpfbzfucp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grciwagtn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gyscowyqp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbnoysuch.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/grcbxwyvj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gejequgds.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gcixrokar.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gglwbahqw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gajklmxot.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gxeaiiter.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gaphfjlvx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gqrudeqaa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gfnzeravq.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gtrfvvygy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gppzdjwcv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gssiajyvk.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/giwdrjlsf.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gusxxkacr.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gwtrgyfbq.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gmfasauin.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gfllizwgg.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gvmueflie.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gbextmlru.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtflnnpue.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gxddulgjx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gzjfowhpb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gzcxjongi.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gegbxgocg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/grofiudta.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwoxnzzga.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/grgvbmvgq.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gykkdxlpj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghfamcuzp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gnfucacwv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gawpeimzo.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gkuoxhhni.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/ghgagtxyv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gcphuumjs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gnrqhrott.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/grekatqcd.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gyjebuuae.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gljsdjntg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gvtffyiev.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gywwhvezs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gqpxmndne.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gzpcndcmm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gvmprhrop.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbxhdeloo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gogczdyqk.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzmrnsoiu.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gubzgqlfw.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmnehdzhp.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gefolgsoa.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gjsfutpyo.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gwzeyvebe.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glxjmioyv.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gclymsszy.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/guosndpon.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gjsyqlvnb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/geratjwte.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gxcpszfms.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/glroqanuv.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gdesdpctr.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gjadikawl.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gkiprvttb.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gdgfwbfes.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gejftywfe.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/goastysfe.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/ghowjwlfh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gurpfzfel.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gtjkatxef.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gjlxbrdjn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gsfjbbjkf.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/guzkxjokx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/glapvpjqr.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gltutfoci.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gjbdzahcn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gfucyfmeu.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gnntkqcbk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gpdgzqezc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gmkaaizrn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gqzpvidzs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdqedakty.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gbfhjebit.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gzekgojjm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gjsnelsju.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gmdxlyhul.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gbkqigynm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/guyjmfosy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gkhelnqhc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/ggclmeqdd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gbvpjatcw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/ghcttulpg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gtgutphjy.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gnwtdawwv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/grubaonae.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnjtynezd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/giquwvriq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gtinbddxn.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gsoyxthug.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gorzyxqtf.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gxtepkpyf.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gsmvkfifa.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gzlsvcfoc.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gqnabirkz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gwcjasbtb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/glbxmsgal.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gisdgayfp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/ghvnxcsxy.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gsqdhpzzw.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfvbnlgjt.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gbwubdvzw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gsbknpxar.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gkdoewbjf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gridxxcly.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gwkiqtalz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gtgqokivt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gzvgxkkzc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gfzfqnnpu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gpsqazadq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/ggqwmxuzz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gtxhlgmda.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gxlrqbqfo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gryrbofbb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gvdeewjsa.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gwgjikscx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gvclzflgk.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtdcvvudl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gzyfjgovn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gznhguiav.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gszybludj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gbsptevha.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gygblitvd.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gjmmxsbyj.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gfxwuogzh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gackyyidk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gxgicebcl.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/ggcqheyzh.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gehyjsron.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gasybntio.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/ghmmtdizm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gyknbonoy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gjccubfuq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gbidwvqua.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gzrbqpmeq.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gkggknlga.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/grpsllpvy.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gcyinhzwg.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gjwjgjygr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/grznduciv.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gnzswloma.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gaggkaegt.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqaumpyyo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/geaaqnyil.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnrleowjx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/glukserrm.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gthqvypes.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gyunuyluw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gbqyjnrpf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gstmcenbm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gyonyqshc.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gekxmrznn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gihqhtvjz.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/ghsbknopv.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gpsbjujyg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gsctexojl.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/ggnytfshu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gvfqhvjxe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gaockznkk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gbkzqhvil.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gtccmvsom.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/grrmyfppq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gkgtuhgch.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gqxvjhjmn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gskdxlfuv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gavbtkbsi.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtdtihrpc.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/ggsijjubh.sHtML


<!-- 参考信息 -->