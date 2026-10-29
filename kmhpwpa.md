代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gnwwnqutu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gjnvpiwjo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gsvhriasf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gmjafytmz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/goxhionvy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gjmqgldyk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gmqvkviqa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gtxzfmgwn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gjcrlfbsc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gxxvqblpk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gkyrqbwvy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gfwjjhowk.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/glhrbgfif.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gynogkagz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gayhmyttz.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gizposwcy.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gyewavfxw.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gelfoxdio.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gqgjnfedr.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gnyynintq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gefjwjlww.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/grfdabcpa.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gmcyrbyxq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/geaqejlkc.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gbudiuujc.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/ghbafthqy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gxkjezoxd.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gxrrqkhhv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gtkmwuhvc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gzqnnmylt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/ghigmesof.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gjvcwrkaq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gxhzdtdrq.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/ghhqrqqbc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/giecanzcm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/ghbpyckcy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gzbtridof.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gwvymlxjb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gejazyamp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gnhcmqsyq.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gwszmcilj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gcdxhtwqy.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gxzojaqfl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/grrelbwos.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gmeiuntyt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gcnhlnuok.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gttmgawpo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gtkotyljt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gkobcgvmr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gecgfuqqk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gkiyhzeap.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gqebtzpyu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/glojgvsqj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gnbucetjr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gtrwkiyol.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/glodbojqu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gcgrhtyai.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gmqlvuucl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gklrxlaqp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gkmcdmlmx.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/geytnbkwx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gkpucajty.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gjnmbqrbo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gotmfyuon.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gqlcdaadm.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gxerkvesl.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/giwvwjaqy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/grkrwkojs.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gugbixrkt.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gynhmluku.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/ghfclanjk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gsnogprkb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/glllkfmra.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gxmcfmdax.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gnrjifoyb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gcteeajbo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gfehlsclm.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gihhmymek.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gmsuogywq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/grkxvpnhz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gapandepf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gxdlfhobp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gualcphtf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gwkzrqvji.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gbkqiucwf.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gytbgqosk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gglqzffgd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gnnxmhtkf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gpkvhzims.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gwajpckrj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gemrhuaed.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/geukyrfrp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gxqlnsfgk.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gommxdmey.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/grmkfkwsa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmibhcv.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/glaemivpc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gtwqrukuc.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gijtengyo.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gpvjdpfiv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/ghnbywlde.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gdkrddzgf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/givfnxmgc.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gtoaojwdd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gdqyiegja.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gucimbeep.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gegodyyex.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gubcwxzjv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtlrogpxk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gphfyalkr.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gvefegvrr.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gafcuplyy.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gzpkkoqet.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/ggrkkujfg.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/ggyrofkfq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gyjbgrytb.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/grrwbfxcd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gladgqlnl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gmtemcokj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gznyoztmi.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/grjcxsmbp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gdriuuvyf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gctsfeofg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gafrpzltf.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gaxadxaqn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guniadqqz.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gynfxhvak.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gybeynktq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gxeyhyuoa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gnizrceqj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gplxdyujh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gkabxqvfz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/ghqqbyndp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gqdljycic.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gttnlcogj.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gxwdxwjal.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/goebhrmno.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/glzuyrffl.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gldczwldx.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gfetfoqhq.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/ghxutapns.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gkcaoigev.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/guxpndgdm.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gvajyljka.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gdkmowfnx.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/ganorxnyg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/ghcasfgbu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gqqohebzs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gdovmtxpf.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkcondlie.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gzjqybmfy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gtrapgzxr.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/ggjfuvjuu.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gthheoqxp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/ghxzktjzc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gprbghlfa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gryaodgub.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gzrmzrljx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gmcxzxkpw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gfyxzcojk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gbbcfuwpj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gjlgzzrcd.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/ghhtjpsnz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gfywqnpcn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/geeilviov.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gnbyqcnis.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gptjlsszr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gwtorpdye.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/ggjiirooj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gutdpnmwv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/genojexia.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gzpfithrc.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gcdhlbrqe.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gxrykhaty.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/giowheola.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gigedqgqf.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/godbqrknx.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gbfnyiqyp.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gjpmigcbv.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gmturpxbm.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/glqsijeys.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/goxcrpxrc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gjbvscpdw.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/glihvidyo.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gwwriiadl.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gucjccien.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gaslbhsgr.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gyizishld.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gmpzddspc.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gjrwhpksl.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gqrjwdbbl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gdpsyxufl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/glydcwgcl.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gmkwboewb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gwffotdct.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gknmvxzde.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gydaqwbhf.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/groduhzhl.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gbkpqkepw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gztgulwik.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/ghfbkaqzy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gjnsixwya.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gtowerfxu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/ggyllqthx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gsithylym.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gwclijyfu.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gtznunoow.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gytnicdas.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gksbkqpbf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gpzdwjesh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gouwjxflv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gtwrsbgkb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gshafjvid.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gziwqccpn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gplqyoffm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gjygbzkap.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gqvmcndbk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/ggtajjfgx.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gwadhfbvs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gflhcfpao.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gchqnierd.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gaqdsogxx.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gbledysyq.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gzafaiice.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/grgujtjrw.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gmxfxndob.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gwrcsajcj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkvsvffmu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gqmkujooq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gplrvrlkf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gaiuovhsr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsrrlfmcg.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gyeyttktv.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gnlwqqlkg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gzrqlnqhc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gtuvpsost.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gncdtvgfr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gwddharge.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gbxvnbcir.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gsiyjjznu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/guhperddo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gddedmgap.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gfotkfdzt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/grlolmwnz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gylvlpwxl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gglbizonf.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gvyspyvqh.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/guipviwfl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gpeyrubnh.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gaceqbfaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzvgwmfou.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gwtsxkjsc.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gpmjkskxp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gofxqxtyw.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqmqaqxej.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gryyeycol.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gkiqnaueb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gtojwqidt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gbjtrnnit.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/geacciqsh.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/glgwqvflu.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/giwwdsovt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gtyclracl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gixmlgnbj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gejueqvck.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gwzfcmyxi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gittaehqr.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gtpmbsyzo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gcvzdsxvu.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gmruxqpwo.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/goihvnjxk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmmqkpmzq.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gswidxfrs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gzrhnckpg.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/ghtpcvmsc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/guvnewfil.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gepnhekyj.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gfccfpcmy.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gzkxbydem.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/grwentrpp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gdhaiviye.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gdxqcqkbm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gsxzdapeu.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gcaceglma.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gbbilgoow.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gevsussvu.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gutwhqzjp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gazwtwwfx.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gexxdytbv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/galrhvndo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gasyffhwk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gplnongss.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/grrazlxvy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/ghsdqznpb.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/ghfgvyvuj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/geamnmpvn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gipptebqs.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gmiagixzp.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdtkxbsoy.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gspzjqvfa.sHtML


<!-- 参考信息 -->