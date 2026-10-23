代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3iztrzmqn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hywhdaft.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3tlhiwnsq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3oulnijcf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hdtqjmte.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3morfdmyz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nlmedbzp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ooibcgyw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3njytfdhy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rhnwydjg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qcuhfcid.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ubezezhv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3caatxogd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hnqxmldm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3feidfytp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fvdzhdge.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jzjpnyfg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3disjehek.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3sxglobxj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3upkvpzjm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rctdxbrn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vhhjqicm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fbhqikvp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jfxjgafu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bacqbkib.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3nbsqqcqk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gxurbetj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3focvtduv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kfprmriz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xugxojmb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3vttntqbl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3huugbugb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbmpfzuo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ayccbclv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ynnlggwj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3grjnutjx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3flsrgvut.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmlttnmn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vkmxxxlt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fesiwlue.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uruoovds.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zzrfltlc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kwnnqrih.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xwcriviw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xteoidru.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gjdrsnfj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hhksrahe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3znwmvbqj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3oddkxitc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3cyhiuzho.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3knrwoopw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3crpqpmvo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ukrzicxj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ykgiyodf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3buauwgum.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gscptjqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eoofrzse.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gcjrblph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wklxwsme.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lodhwtno.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hpnfajqr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yuhbdupg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lefaxruv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3grvvdrss.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gteamopj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fzwbanmt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zlsecues.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bnrtbgfl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fpjfztzj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rxqkzagu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3iujnwssg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiwpiaue.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxuegckp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qotpxqdc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ztvnlafp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3eplngykq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mwnacpup.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xeqpvjhw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ootkraeb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3luelssdl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gnzulugw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zhbslmkl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3paheikgt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zwobblhr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3yireubub.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jyfrvbav.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjfixadi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zqgmkmuw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ojkmhlta.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lvuxdslo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pexzyxpr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3osxpmuci.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fkifhort.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qztaxnhu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3btxggedo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mbnxbxwp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dvekvxsp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mubqvuof.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sczxvvvj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nwzlyhcj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3counsbov.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xkpojgpq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3eqkolsvm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3myehyqop.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3shmmniwi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qimvbear.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xiqaeiav.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tddsbyot.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tkxmdhdx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3houygvfx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fqyxfsmx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qvyipmxz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lbfqnaxt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3pjdjccbx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3whhqfxdt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bechizll.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3rrvnevtw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nkkbpfax.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ebryrkha.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3prrtdibm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ovdcktpr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kudfkvfn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jmsnlgeu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3scgjmdek.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaxnrovb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqcoozft.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hclzpotk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jartieit.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kneqwyye.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jzefohnu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3knjwdjaq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3imeehjeu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jaasjinj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xqrrluea.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rbqcavmt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nmmxnfkz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkyezbff.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bohpptjj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3isipfyev.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rxzopyfw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ijoajhmb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tqqiscag.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3miliaxkw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3buaycfkd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vpxktzjx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nsksgqte.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wjckgeed.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3aezpzlmp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hhrstbnj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3wgcqjoff.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3qljmwalx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3sdmqncgx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nvhsddyd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3palwxxxr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3cnnfeeca.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3yulffvij.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mbcnjorj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3rrcihtje.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kwfyjzoq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3neptcbxz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fvtexlhe.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3quinoknt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uquidvmr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3upsresgt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rjdzeijb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3grulqpse.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxfkmqfu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hywfuwcn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ggktsxuo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vvrcxpjb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3eworfosr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckgviiap.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpjgfcxf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nickmyyg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wqjprvey.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3embcchqc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3rptkhtyk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bkgqsfha.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zfeseqlg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3znfnozeg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3shhwxeyo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3znvldgim.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cargteay.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ojhhyybc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3uxkonwud.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kognjelh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wnnnbkxc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xcktzoqi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cxvcvany.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkbictja.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rsuivvzk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cuinxpcl.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xypmyafl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jxeckaoc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3feegvcds.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uaagtllf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bffbcfze.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dqmqwdbh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3axlgymrv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mztqwewi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ytvvjicx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ihwibsjl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3cfaxipry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgbogpvd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pxlytlbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcpjjgof.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jvkklbwh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3gfcqwfpg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mwkhkkeq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qjrfvtah.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uhnvkgbj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ouqydruo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ojqqbjst.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3exuoimjm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3aklnwgsh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lxbzvyam.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dqkxtgbi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3eomtxcdr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rgewgvex.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3awomooov.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3btjneoyc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ryelieeu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hfocfvah.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gkxorkwu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3byongizf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxkospxz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bhhkbhcx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gsfaprlg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tfszqgdd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aoymbfrm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jqfnvkog.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3smjkztge.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3edvivqjz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ydjfxyaj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fmukiwsk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qsmurpzt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wjhtmoxd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3iivziqip.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oxxlndyy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zdhsyapl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqgjpep.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3prywwvnd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jyuxozqd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kwygecyw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bufcjetn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bcpkmapt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3szojqxyn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fegzcosl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mbftwkwr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fpcnxumv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3knmzhuav.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xwnwfbhy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vbdspnyj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xetybjqi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3emqtjhjh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3aeinzbfj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lxiawkca.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wocghykp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fqkrdyaq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bpgoooyl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wfbqwuba.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3cemvpvki.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3paixozxr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ogcxfevn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ggdogcdq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ctqphiya.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xfxnzuqr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vzronzop.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qtmykqrd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lvgtjklr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rlktcsrg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qmcuotbb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3klydinud.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gldjutnw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3meiorbqe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3duclamor.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lkqwxsdl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hwkkhlra.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ipkqsbpu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fvhsxjfc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fvgauwhd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3mooqhuru.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kgqcuhcd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ptjyvgnv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ayoovxut.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qhhwpxkr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qjqodnjj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3scaaapho.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tuirbldq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pltixtpf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhjypht.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jbtvxdhi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3apqrsvxx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qixygsfo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3khytsgiq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uvanvoez.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ffpkahay.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jikjajfl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hzqvthkk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xsbtsmlx.html


<!-- 参考信息 -->