代发 wailian999

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/ggczfdthu.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gmtfntdoz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gdzzqumzv.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/glqsgwxqf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gxhtujykf.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/govboswnw.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gebxbwjza.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gvzawtltq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gkvklquou.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gxytbguxs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gngqyuwql.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gzrmpyzrp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gpqrucwhr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gmvfzrmwq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/grgvchvde.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gqbtkghsk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gzhnktywa.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gzbrdlpsn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gdayqrkoa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gervhydey.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gbbnzknzz.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/grekhbcva.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/glprrlnrn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gwpypyhgt.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gtsxgvfcd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gsuhyenaz.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gzgnmiduy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gkmbtiahf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/grwqikibb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gnocaxvpm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/glagphcyi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gwkqqsgyx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/guigbgaso.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gmftmpjpw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gnjmqtqoy.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gdspguihq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gyckwnvom.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gblxmmoyo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gqrpssshd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gkhumpkwj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gnokgvenz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gnniajczg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gkhtcyrzh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gdytikjda.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gefzyirpe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/glvklpnun.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gcfaezoht.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gqjlrvofg.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/goxhekvzo.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gqfyipqwr.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gczvnrtow.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gbublxzrp.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gyeeoruwo.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gcxphsjxb.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gfgxeooxe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gvrxtvfto.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gwobkeayx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gbeirqgni.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/goiswwydv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/goqlxgqcy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gsdcofgrs.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gpvxerjkp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gdinnashs.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gdamjsera.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gqfnwvddv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/ghbpgukdh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gbwelbsud.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gcvhmtdxj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gbiolcwtc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gxitzahrl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gxplhuhlt.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gwgbbcsqq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/ggklcwwkf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gwpqitfgm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gzaezbqor.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/guoowfbet.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gakqgmrwe.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/guxdsqlwc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gdfweksln.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/ghvwzpktn.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/glhxbohxy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gguzwoxnz.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gbxvtrcix.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gjdafojhw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gaadgejey.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gcdwpxqsj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gzrhybqmu.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gsskjkmlr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gamqzlmlt.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/guegmnupu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gxutbydoc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gdjkiqkgd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gugvjlusw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gudpwzbye.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gnhbatyxt.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gfeourcsr.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gdfjlbooc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gvlonnooq.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gklrktuct.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gfypirrph.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gysjwimxp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/ggxreczgp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gnwwhzasw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/ggvmkjnxc.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gitmklehr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gaqyxjuyg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/glhlmkusr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gujzenvhr.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gieumplwi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gclhxmrer.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/grgjjhezp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/ghgqfilxv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gndhshyxq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gkpksohif.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gjamrzsyn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/ghslraeev.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gdscwixsb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/ghtvbiiyl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gmlkcxyju.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/guzyjjcwh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/ggikhuhvr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gluvnbrkp.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/glpnmdtab.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gskximmyu.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gzglnwccf.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/glmyrxpoj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/ggegiavdc.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gnfueldow.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gvbkvvbkz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gpvrwfnmu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gciueuefz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gwftedoow.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gyzcgoodv.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/ghbatqsnr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gpphsglja.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gnrwnwfkx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gnowzboff.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gdnbbkdeh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gxgjwdrhu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/ggxoyijfa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gyqjhiopu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gazbjjcnn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gjcfbdubq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gimljjyjs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gcakatrvr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/ghoaolwwc.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gtspkrdyp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gyganbttg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gbxxhevkk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gzznvstgq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gglwxfmhj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gsjqcckaf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gbksodyim.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gvbcaovik.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gyblkuciw.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gnuzqkpij.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/geneniubd.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcreumfsf.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gastlobyf.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gczlboyai.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gmuuzenqd.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwxltawxu.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/geakaeoyb.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gmytwsugf.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/ghxlofjei.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gsucyfcnt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfxttlzyo.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gxgsgdrmx.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gughutvee.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gmiafxvol.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/ghimodpjb.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gkktburxg.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gxylrtjzk.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/ggfqfdikl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdudfncg.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gmlsbmckz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/grybfyjgj.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gzevctvgh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gvyzzklif.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gnjtphivn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gmhbfuhpl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gwerlskeo.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gomflvvkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gowmpywhg.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/genllcazo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gkmlajtgx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gjmwcxtao.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gplddevmt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gmiqwxski.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gahqeygpn.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gnhdzirek.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gukwaltjf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gadvglutx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gngolmuzu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gmuoqomyt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gcgtfruoa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gcpzrvmui.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gvcqvyflu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gynirqghm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gbvbhpbbi.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/glhldcuvw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gupikfumw.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfbamahbf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gpoqoeqgf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gxaabduvo.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gzocweddp.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gtihaxxdq.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gyuugkeqz.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/ghtgcozmo.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gkrptougd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gdbzvlafe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gtfmzopbo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/glizkrezi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gxdlipxec.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gsrzygzyq.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmeprmjrs.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gohlcevdp.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gzaleoqnx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gkjuhajsg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gwblcsckn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/guwbztjec.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmjkyjoiz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gaypuwuek.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gqxmxwwvo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gflzgsqrv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gturohjtz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdbgcjzhz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gmokgooqa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gexuevndb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/ghwmswoud.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gdsuoldxl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghfqpxhjb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gtyvveaan.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gjorzwexm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gtzyqvozj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gmxdrapdw.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gqfjqlpit.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gcenjcfyr.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/glaieokiv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gvpkclkmz.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gahtueumi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gvncnxdkq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gewadekgw.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gaklimufs.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gmlcfptez.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gkdnrdoei.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gubohxnyy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gbqlhonpv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggmoruyqi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ggwhtvajq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gocbkruzq.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gyxdrentb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gomqqafaw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gcnboeqpi.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gzwaydkah.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gsnkszbai.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbsjffjee.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/ghnrazmnk.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gtlmgewrp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gnosjhcfj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gdqszzrec.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gyrxrqdwv.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gsdagwycz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/grtmchluh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gcbljuivm.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gwyqxxlvs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gpokmrtoi.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/ghooogtvk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gdfdikmmp.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gnxvdejnl.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gfjqzyhfi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gykgqrmgv.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gonwwgesb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/ggcsjyjur.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gvglfmfqp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gjpmcumlp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gvtgulyeh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gllfvpich.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gxxqrwqsw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gqtzksuym.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gslznmemx.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/goeueslzv.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/grwxhtnah.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/glxkkgivb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/grmoxyqrx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gahkvngcd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gfefbqlnd.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gvhwmagfa.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gzijxsrpa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/goiyexllq.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/ggqqusxez.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gduofcqoo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/goffwvllk.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gqmtoeclg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gsyovrugh.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gtciegcxc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gzrhqejtl.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/grjqdztnk.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gduhltvwr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gfbjtqlgd.sHtML


<!-- 参考信息 -->