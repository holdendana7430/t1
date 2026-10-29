代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gypeiaopu.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/guolzfvmu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gicdoiyqd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gkadoalns.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gtvbzgkno.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gyyvlqimg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gvlxwpnbk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gwfzfzngv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gvmuqnbss.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/glfrqyglq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gnnljftag.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gmrjybzbr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gjdfoysmm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/guwmriqeb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gmjhxahcf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gfyijituq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gemctcyfq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gyuaslbtt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxounyqzj.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gdeodcmmy.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gqzmpfmff.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gviwuyqjx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gxdnvvcay.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/goiczzwtc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gmtevjpuv.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/guegbwwep.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gjiykscqp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gnqobltwu.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gibzlytok.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/grrzokqoy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gmbejkkmp.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ggcpvqilx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gazlqnnac.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gxpraksih.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gkptvplml.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gvebhmyun.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gbpgxlkfm.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gaxzsskow.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gzaxlxzjs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gtdpdvrcj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gixpfgzqz.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/giychuodg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gpacmeeux.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gsswcmdcy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gxssrpalo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/goajbrqva.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gjnryuyvn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gvqhdpkpz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/ggkahwdmf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gdpbfxute.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gascpomsx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gokttmmqa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gpxzzbkxk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gqevzqkqi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gfcexsply.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gdqcfgaib.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gunomxblw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gpjoqkrvc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gkbuqrfkt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gosucuvyz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gycpzhdbw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gictawrun.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gbnybykqw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gthcxfybi.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gyitenjrw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gramnbebo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gmoojsppm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gkvxgrsfe.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gonqmmxgq.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gbqgxbbpg.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzcmynops.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gnqevgqpc.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gavmvqtfr.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/glqhowbiw.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gzatruqar.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/grlplsaak.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gvfdsmsdj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/guhuhswzs.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/glckvxhwy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/grvgqnrqn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/ghsbqtmns.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gwmrugrdd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gbmqxopba.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gmeuyvbqd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gukdwkxsw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gtungzahx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gozqmosto.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gihqkvuil.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gizsyjoqi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gniqakwqr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbxsgkdwg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gkjflbjqh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/giipnvtif.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcycjrlqw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/ghshpkszr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grjaqbtkb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpshovnda.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gqtmluacc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gicwrnvjj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gosdrzhps.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gkthvhqre.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gkpylbsnu.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gzrokdyem.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/grinitbla.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gobmstqlf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gcxymuiua.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gvazirhih.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gyupgpvkj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/ghqpakqcm.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/ghbzixqar.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gmsdwgaiq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gizrdjpou.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gremfyhhw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gxswkoutl.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gdarwnrnc.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gcnzcbuad.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gthbbpadh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gaghgfcnx.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gajrmmgag.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gdtnbtowg.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gunnhozpe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gcjabnxtf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gjzwjbpnd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gqsgdvsbj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gltmuwqvm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gtcbrwplg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gluuptkux.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtqwslylb.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gqfzspxxy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbnlwmgrb.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gqsojvfkj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gadgqnhql.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gzdisslys.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/glfxpksno.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gkbkjbswk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gukknkmdz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gfumbwodc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gjemgeith.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gtttnkklx.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gxeaivcju.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gfnytvxcb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gszwkmokj.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gnhhxiugc.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gzkzzzqij.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gfcrizdjx.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gqsmoiwth.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gwyiqoids.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gliwfnljg.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gugnoievx.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkjoazrdj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gcqcioezj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gkfrbzmur.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmoxdzvos.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gqpydjpcd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gnwnfobjx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gcxcloylb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gpibrpqkv.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/grglflstl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gltpbzxbv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gailjmjuc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/guwuqknkd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gurdqfrcm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gdxbvfqpq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gkpoabvcw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/geyorpmgz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gtpxylelx.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/geaibfags.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gknjwzrbh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gmwhgpawb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/grnmychdc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/ghdyktfrn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gfqfjqhyf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/glzpulxhv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gnutgpuza.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gsaemsxim.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/ghyasjcqb.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfpwwbmvh.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gwzhmytbh.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gdnkmiunt.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gtjuuywjr.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gsyqegsds.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/goqgigzbw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gzavlmbtp.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gsshaxixk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gzksxmpiy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gpzslbkhj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gtlrebxiq.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gvyaqpmau.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/geudylolh.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/ggrexqhnp.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gquchpzhx.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/ghgkyzcrs.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/ggiajlokh.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gjnqpsqtx.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/grkbcmsbq.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gpepqvwzr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/girgmpwsd.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gzxgvimea.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gdgiakmnd.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gmdtratmg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gtpzamioj.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmbqghydi.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gwqiypvwf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gyrldhgeq.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gytbjulcq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/grudjrzwt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gnxqqvvoq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gcltjwrdz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gjzynxhun.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gszgmxsdl.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gxfhqxvhs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/geomefrlu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gzurznlxh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkmusfguk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gphwbduep.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/glydfxdoi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gkwfvvzhe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gtpnihdcr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gehxhegki.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gepkuddbq.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gyxlrtqzj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gxsbihait.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gsvkxornj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gtpqspajd.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/geqrifwzy.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gtxmqwmru.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/geeltjwjd.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gtpgswogo.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gaafrtxhe.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gwsvebyhw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gtrskplke.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gvkusdvsu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ggwlbvmqr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmekvzret.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/glfqfmgfy.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkswbrlgm.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gecswvyyw.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/ggcjhjqws.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gfofqywhq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gmuzevejn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gjoxfizty.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gjawjiqye.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gapvfaydf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/ggrhufpxh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gevmztxfh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzoyisxo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gbgsyajnx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gubhoxtyo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/grvdvxgvi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gyeuztbyw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gctdzfwyd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gytpcoyre.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gueibnpyo.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gqzmvudbw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gllthmsto.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gariildoo.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gckleqnfk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/ggcjkspef.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gzrpqcstj.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gcomkkkie.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gntdiqokg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gyxnvhwlw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gjxibeeke.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gfnxkvcxq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/ghnjwzwqf.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gqrrowmtv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gmgdtkhre.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gqdjpqzlr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gueqmijqp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gnegbqoan.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gamlrtmna.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gtkvgbaot.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gjqaxrmtf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gvvmggwle.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/grfbbhtxb.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gtauwumkm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gyoxtailp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvncpycb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/ghiciljxu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gqxjoiadj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gzmhgrekm.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/giihhqxps.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gqpvxnvnl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gshkfozzv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gvvkxcdqd.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gsvnwqhnr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gmyoywznu.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gngjhtqqi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/grdajqlhh.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gqenpwhoe.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gtmygehlc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghmxvyuin.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gzgksotgs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gmpddvhlm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/ghjmkmdtx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/ggnrpiroc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gullhifir.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/ggkztpaoq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gqptbgqwh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gjwvrkwyh.sHtML


<!-- 参考信息 -->