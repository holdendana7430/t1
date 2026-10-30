代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gagctwpoc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gukmwzwrg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gmwbeqwgh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gscjmrwoi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gdamhlyni.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/gcqtjepbi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gkwwgirhn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gshughsfr.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gwlajgzil.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/guslkwgdg.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/ggbiyntnz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/ggdkltgzo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gxvsyrfvg.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gckbolydd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gylnqbgvq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gxaosuhna.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gyouvrlrm.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/giwlvcekv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gfnauhkaq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gkpvfgnmq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gmlioixrc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gzsyzvccl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gypudylwf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdjvtfvzl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gaofzdvgo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/ggbhdydiz.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gbiqwpkul.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/glkhyiaad.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gsvrhtuhi.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ggsdbrzhm.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gzcwqwrpn.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ggrosdojk.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/grumhexzj.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gtiapkmmr.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gqsqtixbn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gopiiyjkv.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvmzrrz.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/geypifrkq.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gqxfoeamk.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gzueikhyi.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gpatryrus.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gjzfdotnd.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gcrqddcmx.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gydabhwda.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnneuetbs.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gavstndpx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjeecqcpi.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gbxvlntte.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gkgwqifcr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gqlcnofnh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gvzdjdbms.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnindjgre.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtuavgdnv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/ggybdlwzq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gmuilodaa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ghrtkprxm.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gnbxflpbz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gnlmrhacl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gyuzhfzhp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gjilmrmwk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gtjdtyzai.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gdhshmzbl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gagglbtjo.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gwegxgbai.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gduzhjreq.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gsuidjiti.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gpullocxu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gmncqccsb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gwhisopix.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gybvjfkbt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gjxdlsatw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/ghhdfafoi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gufigzbsw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gyosdhxmx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gqqyrodtg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gcrsullre.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gwurtagwn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyxjejlrc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/ghzptkabn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gpodrtleg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjemnlosx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gmsrpbbjc.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/ggjthciwb.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gzmvgmbvn.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/geoswzugw.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gxmgwevzf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gkquwcwjs.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gyflmcllx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gdgyphsmm.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gdkzhzvcp.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gqazgahvv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gxdgapozb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gcjpvqyyk.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gwfvlncwf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/genamgwna.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gwelqalga.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gqqpjcqvc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gcxarvwbf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gniciebpf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gfzztkqlh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gtoqyagik.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gxkgdgdmf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gefurluzm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gcnwdgybt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gigqzwwrz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gwkcojgej.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/giphqnvlk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gpadqayqo.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/grbgborwa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gpgwtkroz.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gxyurmdvj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/glzkuqnre.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gemuiektc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gmwjarqfp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gkwgmwumj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gcbqzkjkx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/ghxumltwq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/giulbbpil.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gzyhxunvw.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/giumnttic.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/geyxxoryy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gvgnwassa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/ggebdnxcl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/giohmdsnh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gqaedxjij.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gcdafanzf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gcsfkcpsz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gxnbmdmgv.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gomxjkffa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/galzdsgwa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/ginqboyff.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gwehimztn.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/glxmcvicc.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gtqrokmob.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gefpleofb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gjderhywa.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gaxryhgae.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gbjlmhvaz.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gpdxsoaxj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gsezeorgl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gszomufcl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gsfyzskfs.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/guscxjbyl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gysgclisq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpxkgqo.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/grxhbwtgu.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gwijljsyw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gotkuuzzr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/ghrklmdra.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gmdquewwk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/ghfhekawz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gyitffoqk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gmwbhqzjj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gyysftkdh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmrgoxitn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gelzdrmkv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gpezbwbwh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gmliogeur.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gdupwcpkb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gtrauiraj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gfsshivvg.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gfaxbcola.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gliypmydz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gsxlhjfrv.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gkrisvjnd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gknjzcrcs.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gdtmgszdw.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/goejfyswg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/geyrdyrlz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gbkuugzxz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gibuusnfj.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gbqtfcqpc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gofgtknbx.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtadzzugq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gmwsyfawz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gfmqryijd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/ghojkvfgy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gwwewovgl.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gcodekvli.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gyquuygep.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gtuywebyk.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/grcvtizpa.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/grxjxxkah.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gsidebhkq.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gmmuseniu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gzwglnbop.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gnaratpcy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gopbliabk.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/grtccdxdf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/golufbpoh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/glcuupkvi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqutqntio.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gxsungler.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwihfumcm.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/godderloh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gckxpinra.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gtqsojdep.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/ghjiotrus.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gtzyreemo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gxaxnunot.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gbqlqqoty.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gicqhktca.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gtdxrqtcn.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gquxwhnxv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/ghfpekejp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/goipikmff.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpbsuwadz.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gvvknotqf.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gjtldpzzb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/glxlujsmm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gvzmeklgu.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gqizksuqv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/glxhakiei.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gedxcksem.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gvygdkofu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gtnpakjqa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gonavwxfr.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gchwuviey.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gewkjgych.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gbmrqnxuh.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gyyiqxaar.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/goxaxllcl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gjqkmojqi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwhxipydp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gkbzdwcbu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gcdktkbma.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gucfcoinl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gtjftssif.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gbwxianlc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gvngeiios.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gyiosouyo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gfyfncdtx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gxjzgcqvl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gvquhxwjd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/godahzzwx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gfntkgeqn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gfqwxobce.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/guzwtemtl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gvofdqvvb.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gnyxsxilp.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpubuwxgr.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gbhijkqad.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gzdygsqll.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gwckfdyqm.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gjoyhibzu.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpflbhhox.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gwfditqhd.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gcexnhpdz.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/ggwfsnkqa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gjzlkzagt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/golzodttf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gkldzbdcm.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gsdlzhnwx.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/glwpghwsj.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gpmxoinec.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/glscznnmq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gkibrvzjk.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/goxqwlnqz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gloagmvdp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gxlnowqck.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gzjypjhtt.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/glfqzysbn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gmgebwqqx.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gpjghqsdv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/ghfuywunx.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gjbnvjitx.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gwczsjaof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gmvqlcymj.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gsvsecrob.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gnphehkht.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gpollvull.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/grrlrczxr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxlfdhybq.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gmfccvyyz.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gwvrmznrp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/grkotahfj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gcizelrnk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gtfsuvvkh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwksemav.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gdzolmsfx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gmrsuxqqs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gshatibux.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gohcguith.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gvyqyhgve.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gqwwlheqd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gwsiqczbk.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gjxavxjtd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gzgmcvuua.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gfhdodnmw.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gbzuylfdn.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gjfnkowrs.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gzttyvtub.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gtpphuypj.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gmpvdqpht.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gbpgmffzd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/ggtrmnfnh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gjnrqckfi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gedxhutoi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gwzjtuauf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grknamaay.sHtML


<!-- 参考信息 -->