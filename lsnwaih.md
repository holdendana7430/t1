代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gnwwyyovk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gyznfkmzd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gfnnzgazw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gnpohdvww.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gpruogqyq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gtckpnjwi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gleuwzknr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/glfdlyepg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/guvytdayl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gnycnxjhs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gzmiwwrpk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gquifnrof.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/greipwgyp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gaznrvxaw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/giitvyfsw.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gajcnenda.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gghdkcgqz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gwpluynjo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gsoijuaip.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/ghdnfrjws.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gkyaasgwl.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gdgolfzki.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/grsbuucdp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gingejzzy.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/goiqlzqtv.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gcyfrukgm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gsezveegv.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gylsawojj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gdlngeslb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gzgwaobmu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gzyrlgpri.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/grbleiaft.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/goebierrl.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gaowihlnj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gxwevtmlt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/ghofxdnxg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/giaqnzobs.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/ghsffyuui.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ggqoaysnd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/grkquejxu.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gamusadjk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gidfvbxfb.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gzjuqpazu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gdqivhemt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gilueikhd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gijicqctw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/grstztfzw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gzjfvhwpc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gwcczisiy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gpssdvsgo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gjciayylh.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gtqmdsdsa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gbonmvpad.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gptdopfxs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gmnmbfott.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gljqiqulh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gjgpjhtto.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gnujzhotd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/giyuskngb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/ghatkfrky.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gshlgjecp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gjfogfxqb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/grqnmzbyj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gslssppah.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gcghjepad.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gumzcjxqi.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gvfeettuk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/grwfwutgh.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gxqbnwkpl.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/ghogjxbkf.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gqrcdwmnl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gvytxgnum.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gnxbhrzfu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gwhscahem.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gwuvufxoj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gobmaulgn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gyzyrcubq.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gdpooxubo.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gnkgaeznl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gfxrdaapz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gxrdldzat.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/ghfsuawuj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gbfxbrgmh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gsqjluocc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/glxhtwbvp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gwamjysuy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/griwhryuc.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gwuodnruq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gffysstie.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gaazmvfor.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gjeyqyiag.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gvvbxhgve.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/glpttzvwg.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gfuzllzta.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gbvzkylek.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gaeauytic.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gxxjrzdtf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gkjxhuxmg.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gsboyhizw.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gcatdfoel.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gfaxzodel.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/ghgawbnyv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gyialqkkm.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gldtqtxhg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gbgfjfmwg.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gxgqmfdpm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gkddnkebp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gjcjzlzhb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gfswvcspb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gropwvupl.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gwdzpfoqd.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gxxdqkdcw.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gzllnsgzh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gpgxlbwod.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gjqgmsxxi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gnlvgfbxe.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gksgugkvd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gqkmpidun.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gaxceatmj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gbwnyytuf.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gxnsnjniz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/ghmbyhgqr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/guwggmwti.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geuaytfnu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gjekdkkpj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glkfpixts.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gfxroudak.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gikoyxhxy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gyfhumlej.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gtgdqjvtl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gtbslgwiw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gzfpcvfrp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gwuobunes.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gmdgtoouk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gxxgeheko.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gsgeedgjc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gskilnkmm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/griuwjhec.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gorlmzjxg.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/goovqwjln.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbgllwowm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gflldvjgk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gqalzxotx.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gthhrpxxq.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/goymotfaa.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gyuuuimee.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/guyycxedl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/ghpagprre.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gmnoiiarn.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gujnfqljm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gqgkmtoda.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gdvjvupou.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghvycdeac.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gyonvkxmx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/glhirezqi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/grkdjmsxr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gdcikmhqx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gnbsstlda.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/grxzpqpqd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/ghffctzpe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/glfuyokkz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gljmoypeu.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gcvmaqppt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/grtsxdraa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gkcmwrsll.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/guoqmhtlr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gxjgudzqg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gqmbydcqd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gygqkdezw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnvqkacep.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gbwoazpxw.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gatszccgl.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gjcoviize.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gvvkdasbt.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gvzgrojru.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggxdgxjws.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gchccrgvz.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gwuakurhp.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gyigebkjj.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gxfitfaqz.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gewphnvvl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gcmiwpwyi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/ghadmuwph.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gpocksmcz.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gtwoxiexq.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gwdaqonyh.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gvbpvndwl.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gopjcazve.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gioxypkvu.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gvdqrziqq.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/glxyxqbrm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gvkrnvadr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gwagnbddo.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gcuvkkaob.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gxpvzqcpg.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/glayxszgj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/grabsutxp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxsodxtrs.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/genjuxwky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gfiqegtoi.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gfczbzhus.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gccelmdxw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gysppnykp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gaszgdenk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdemmfiff.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gnffxefqy.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gudjjhytb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gbgqauytj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjnftpcze.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gxexdwhck.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gnkfnalad.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gjibtozdz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gfgrwhxup.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gcpscxnqh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gcdhdlqwu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gdwzqsire.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gqcfcqmdg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gmdqbqpzv.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gkvyfqyfh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gsfkkqauf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gvapgeqlj.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/ggrzmpqtj.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/ghjiyvrzn.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gzpjhbwyb.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gmasmifqj.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gluleujqb.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gtvzqfveo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gsnleptak.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gzmcrbolr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfauqqrog.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/ggkphasoe.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtpxrxczk.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdonwbowe.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gcuvmfmlf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gdzncapqi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gscnxcldo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gbcrjnjsr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gjzozdheh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gegbecrgr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtarasdmy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/glpgzmdgi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/ggfkgdcll.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gifouqcdm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gghtufnbd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gtqmfqxsc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/ggmwdtpvz.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gyziheruq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gnojplhng.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gtvfsjtox.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gqmagyhdx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/guhchqspp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gafqpxdhm.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gzimzmzxn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/godnkarqf.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gwpladltf.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gywwahvpl.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gkpqfasnf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gxsgajksc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gztagnsde.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gfdqxptey.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjrfvljzl.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gkcgrizvx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gmzsvisez.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gajskhmme.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnkhygwug.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/grojndjkz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gduylailq.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gtehjhhat.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/geytbrekm.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gliovvvde.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gdxgmlmrw.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/geuqhelfq.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gzxppdhmz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gafpxnywn.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gdlttfrbt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gowihgqxr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gudsfcrja.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gueawgzlv.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/ggyrngvaj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/grdyqsgav.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/goszitqil.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gwkezwttl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gjpzbopol.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gkfmxeuwo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/geuxpbtpy.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/ggbaqhctb.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/guleeucri.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gktrfemiq.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/grrtnfxfm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtgguedzg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gybtihuua.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/ghbkusnvg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/giwfqefls.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gxoxybgrp.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gezhqniez.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gnswfvekn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gexienotr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gjdkymhlo.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcbihmqgy.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsbdbujoq.sHtML


<!-- 参考信息 -->