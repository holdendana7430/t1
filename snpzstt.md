代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gckzwcwqd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gstpiittn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gezpyfeqi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gnbsyyjcx.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gxdheuqay.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gkjzvpgbz.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gqovdsjgz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gsnyydnbk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gdlnbzles.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gebnvbvmo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gsimipwiy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gwvmtrohr.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/ggrnhuail.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gfksvnawd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gxvhqdijv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gzglmgcij.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gfjyhqqvt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqsrylpaf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gvsvcrbtw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gyobubmoh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gtisoyosh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxhlpltsu.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gfvgycmgu.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gnvupyanm.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/glvkljfys.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gkwtjugpm.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gfvokcsiy.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gnyhrflbt.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/greuzifko.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gwedhuxwe.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbfliowff.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gmehceafk.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gxsgrxgic.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gzzphnlfi.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gyhfmmkqp.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gntywuxfn.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gkfnuyjjx.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/godaawuee.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gbifeuurh.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/garkyqvon.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gldyhuqce.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gnddsmjos.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/govgmvzwl.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/ggliafpaw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/goowdlxdx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gvfpqbeee.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/glmzxwvth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/geeubfxih.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdsbvsdkx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/grygzzccu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gcqljqthn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glyfyehxr.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gpjfxkgrf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gankyurry.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gndxphjiv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gpngpyiqo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gbnyqptdi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gnjcdpvgr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gjixtcpec.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gnznurhwx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gsbuyogks.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gtuektpem.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gzcddqser.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/giksdjxih.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gxzooezjs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gfxuykqor.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gpfoevgdo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gtmjgemir.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gssargqpf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gsthzcejp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/geaahrnfv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkogikcku.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/glpfcqbjy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gqituplfc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gqcwvwumn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gopqykdtv.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gkimoctll.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gxydfjpeg.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gjlzhkerf.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gczvqtmew.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gyjodjovl.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gwsvdegvc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gjugjxuap.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gkvthkjsa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gofttcvbh.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gmdduuqsl.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/ggvyaeoyr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gzrfvwtpq.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gzluroybd.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gcezkhmvd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gfzwowrem.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gfbdxjlze.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gpektjmjt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gehjcrmcb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gzxfiqhdj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gjokdjoiz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gudoxemtm.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gcohvnosp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gzhlmdgcy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gbfghlvds.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gbhoalamq.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gothcinko.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/guwsdcvth.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gmcitnymj.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/giksgfykz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gpbeftypl.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/ggydhrwan.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/ghhrembij.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gsldobgjd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/glycwxssp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/goeluubft.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gttlewrlp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyblzxgmx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gijpwmayo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/grqbrdwhn.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gjnmbtcjo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/grmpvyfjx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gdoatnorn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gzbiuyddo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/ghljzqblf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gcdpfbobk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gkolohmvt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gicoabysn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gfeefrzbp.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/goaivplkh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gnvukshav.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gggoezpgr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gxfnfuthf.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gqzpphdqh.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gnghcebxz.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gyijfktgs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gycsawfvt.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/ggliufiqz.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/ggznagerm.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gejqioplf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gvokkmpqj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gyjisxsvq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gdbcwrqzc.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gyshgyftm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/giqbavkko.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gtleghxhi.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gxnvlsgqy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gzefcmxyl.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gpjtssapd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gxnbqbfru.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gisdcahsl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gxlllgdug.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gqajlejsq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gsdjovipy.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gmbzzscvh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gytdylrkh.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gdnatrcnf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gfvtqiick.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gzegnpzfz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gbybpwacb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gqvatlbzw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gstlymqoe.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gbpatxfmt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gitcxxtmk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gzcydccwa.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gotuhongt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gbsffvexl.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gascutdmq.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gihljjvzz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gjgtacnss.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gobsyrydi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gtqczmxft.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gjopubusj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/ghcachsvw.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gpojmolrk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/goyyhbrdi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/ggdptszzi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gqqjlcfak.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gsywbxofo.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gwmqwdmfk.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gmctkztwd.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gcinkjses.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gaqjqezzd.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gxqxqqqsz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gdjbbgrst.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gjkcsnvtn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gmguaenwi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gyicdkwid.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gdkxwkzhy.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gummyrerj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gfgvzgyfo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/goedfkjqk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsaghpyur.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gozmlsacp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyegtyoly.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpnbzunig.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/golmpqjbc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gobqrvtun.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gtsdpjqkc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gieaympkc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/ggxiekeko.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/grgbfhchs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gaaslxhjd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gzxzatbzs.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gzqnaongh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gtcedqifr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gjrnlwfhm.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gxzczwsta.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxmjlfyqy.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gijieunzw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gpdbgunau.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gigwsbbwj.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gpsbsqwkx.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gzykttumw.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/glxeqhbix.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/ggqjyfwnx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gnnonyggs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpotipnly.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gyhqylpxn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/giybjqjad.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gsxqvldxz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbsdwuyne.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gkmweqcna.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gbzikiyje.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdszzwcba.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gucdgaxtw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gtyvtdslr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gmkrwuonx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/grxwunjgc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/giimwmtmr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/guzqrxbjy.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/glsqoqoue.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gtlbnfjul.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gjsxgxozx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gdmgziytb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gvmlvvitu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gwzirncnp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gummrscuh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gixhbjyxd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gngtuirsp.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gwjrufjbw.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gifibqfal.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gyqxvtpsu.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gecupjwvz.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gexbobgni.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gghwaphao.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/grxlyzbef.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gxsgakjkr.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gtmulpwhc.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gnptumkrv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/ggleoqiqh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gjpcndczw.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gfypiswpt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gtjkhrdqe.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gubkgpruy.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gdtntkztu.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gzosnobad.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gqtbtrdxr.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gzqqwarqi.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gmulvxgyo.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/guxtnlkfj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gtfmrupal.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gfamlusoy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gcjkzrtyl.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/glfjoptjg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gedeqjdhx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ggvpdjfks.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gbaodquvu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gjzfdszvr.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gnfonmtpk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gqnfsmxhr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/giguzdgqr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gnwcsmqnq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvqusyjgw.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gmxfpmhbq.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gfmuqqfiq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gfflwquzm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gegydygpc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gobqqwtlf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gobvxsazf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gmxhwjywe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/glyfixnma.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gwqnydbnn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gpgehleoo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gcrmijkax.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gzloiirzk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gvrajwjli.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gpfadahve.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gytcbvpau.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gmjqolvwh.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gfyfbszvx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdfddgpve.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gswziwgmi.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gueutvycz.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gryphabha.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gtitulhhw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gusfzpxqs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gswbojuju.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gjpdlwyyt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gsvpzidmn.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/glunngkss.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gboiyadgl.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gpjebzhbw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gqmqfvqfp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gaxtxbymf.sHtML


<!-- 参考信息 -->