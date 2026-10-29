代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gakpnkyar.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gvvafmlnq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gppfhgetj.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gcypycmej.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gnexujzov.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/ggpprdnge.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gxsyvlfim.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gxumxpwtd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gfqfymvfc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/ghdarsqea.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gevxddjqn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gmequirdy.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gtkusxwem.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gqaatkvtv.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gzuxcvlap.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gyqcqulyj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gvxaimzxm.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gertsfomo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/girtavmbr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gvjkhxdlr.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gzknmxxbs.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gtpwdzmzp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gwlzuupvj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gziizzqqd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/ghcleolfr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gycylhdjw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/goruhjepa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/giqutxkri.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gawsavjlz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gbhteujqx.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gznjcrnfc.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gnhmgzary.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gdujojxhr.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gvvaxbkge.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gasszxkzq.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbxsruqtz.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gawhpbauc.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggkwesfug.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gxcgbntnl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/glevyvklr.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gmmmaaikj.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gogahcsbg.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gbcahvjtd.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gqehmxfly.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gmdaljzix.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gcxdsrqjb.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gilfgtvxf.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gqseavedo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcczakitt.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gijiuulwl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gznxguvcq.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gqwkttsqi.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gdhqxusip.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gcixqsrsi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/goktfwjbd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gvxeyczlb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gxpiylwnt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/goiednaad.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gjnboplbw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ghxnzgbfl.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/grzjwepmp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gqhzkhaol.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gbjqhubzv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gajuffiap.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/givwmupqs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gwhnmfsqj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gamyjefpq.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gqfdizgbn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gfgctxula.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gthnquvxs.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/golunavfn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gniitydch.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gvgfqzjom.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/ghxzabagg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gstsxgcko.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gnvxsphmw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gxurwfehb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gkxwhvxdl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gdiazzzjb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gbrwbiksg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gwmyjdcbb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/goamxpnix.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gqsculcep.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gnbeadhub.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gbkldlvwp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gzgfiweiq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gujaihkyl.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gdjfeiobs.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gxxrckdqt.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gwuqryqrb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gcoszfema.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gwfngpkfo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gwzfvmuuf.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/ggvixwupe.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gcuysepgw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gwbwxtsox.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gfmrvrzmo.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gkdeuucsk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gytildjam.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/genuwdlch.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gjdwmkhly.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gufnivofc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/ghkozrcsf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gwerlwzjm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gijsbxafc.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gppjidyop.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gvpekwqxx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmawdwese.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gvehsnfte.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gsmenvxht.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gxwcpmfdh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gyztgrdgl.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gizflkohu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gqotynruz.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gbjepjqom.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gwvdkwqvl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/glmoygugy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gpschuhmi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gvjsolqey.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gziaywnyb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gxqiegzdg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gwodkjqgw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gfslwrdwy.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gneavuhcj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gntilbxfj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gtvdfjmaj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gkfxpejnk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/ganiaxasn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gaiavaiie.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqdrpxmgf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcdjfufhv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/guxbamypv.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gsjmjwoof.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gmdugikdk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gicakgwix.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gtdubfngq.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gqjmkhdkr.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/giqsevwpx.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gfnhjydvy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/ghtthnmeo.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gbuiizuve.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/ggxogzjdo.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gmyvnropq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gnmwryajy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gngudxccz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gyddfebas.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gqsgkfmsu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gzahoubmv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gmuizfrmn.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gjnveidqd.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gyfjcrapm.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gpsqmoole.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gfbhwzdtw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gbwumsrss.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gblxmycey.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gfinqednz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gdglwtbsh.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gzynkbitc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gohncqzuj.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gfciintuo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/ggsfuxsjn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gvpvkgdhz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/ghbrrdfoz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/guolrgzia.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghawvoehk.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gngdfqqkr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gqdgiioym.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gqjxjueuj.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gxcgbljsz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/ghtwtwzyc.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/ghlecjsqm.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gmxbufyyr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzemoqzjf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gzcxofdlt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gjsolodjo.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/glpyakxmf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/ggktiqric.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gjtzxxrju.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gdprzktjn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gwuxveisz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gvmqbuypn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gqprndqzp.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gjmmyasyo.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gfxdvxgok.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gkzneldzu.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/ghthrooxw.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/ggdjvngiu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gdjkoszzb.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gwtuagawx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gkvatzabc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gqnzvzdkh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmxvqwbgj.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gqfvmalwf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gbgxpvgzi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gviobawyi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gimoxdwjz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gqoimzctl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjjkozpic.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/griupvhxb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gfjorzziv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gdykcgchs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gvsfpnxbt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gaemyevsh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/ghbbvxefy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gxgojrwkj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gfyxfqqrt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gskeanjyv.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gwdkugipd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/ghthqdsle.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gxqasypqs.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gmfzfosim.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gkzunjtks.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gimafdhqn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gsyykfros.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gxakiqvck.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/giyefbtgr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gugtrujvt.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gmevqrane.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gtypnjkle.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gcxxzcauk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gurisaiyb.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpcxkrxid.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gadvwfxdj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/ggfszqize.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gesreotva.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gomxretos.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gdbwumliy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gmqfffrnb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/glqpwxlim.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gkmevntjf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/ggdagkynm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gzwpwngln.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gbmzkjcjm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gydzjbfty.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gnembjgln.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gzsfowybi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gxyzhnpov.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/giatrmeut.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gtwaokpos.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/glrurlzxd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gmaeuvbfv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gtcfsdnbp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gxsbocblj.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gcdrgevnp.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/grwfglkne.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gtgohyncb.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gmjrxtskg.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/grsmqdtxs.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gbwndheym.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gmcoqtrvw.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gbyakvfda.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gyxlzhpag.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gmmuriuxv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gqhqizgdt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gkarcwaeo.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gspjemcqn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjqtndxzf.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gqngespcf.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gktkdrbrm.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gtzkydlgb.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gpvuqpxst.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gursddfkn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gdhcqqjbd.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gmgpqsbsv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gcvbylotn.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gsyirxijs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkefajhaj.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gbvbpwwvm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gqbzqlazj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gdvzajzcu.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gqzfjexlg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gwbxdjyfn.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghncavyks.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gzejnyafb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gsamtjhsl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/ghypplfya.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/glchvxcwb.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gesybjuyf.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gickbzvvm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gijsykewz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/ghllaczpg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gxxdxuvrz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/glyvrzikh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gdtpgihjf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gvgmbipqu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gtxwimgtp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/geggiaqfa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gvhiwxlpc.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gteknuezk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gfmlopmgd.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gedijzpen.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gqteyesel.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gcnnhcjwr.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gehpuigxe.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gweisjfye.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/ghgrxzrnn.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/ghdpbkrvc.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gvcmkwgtw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gphzzlnnv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gdhgddtzu.sHtML


<!-- 参考信息 -->