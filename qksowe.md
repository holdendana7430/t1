代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kuthitka.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fofjxwnd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3tlvudxse.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nfgxrdha.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kbvacvqu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3euohpbrf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dcdwhrzg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3nbbshcon.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mxczspos.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kkpdosdv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yptjsipq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3sbsfschm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3dfdqketl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jveiwcdj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bhpgklpy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lystqvbt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3obiraxed.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bevavmcc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hbwsbdul.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3oxnudxxu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3urkfeuds.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dbjsvray.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cmfzjtzu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxmqowog.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfkcfixg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ekwmqfgs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bnebxzem.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3smwosrnm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3eurnxqyz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hyecgmfv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pqesssug.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zznkwpjn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cjyorajm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxjqqsac.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3brjowsil.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vzgfiyeg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emptehww.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3naiqtrvm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3onlreypp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zcwpskuv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rvqlqadw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3osqbohts.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cmemardt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wkwxlbec.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3holmsgfv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hpwggtal.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3juubudgo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hrwjvggx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gvgmmzwh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bpmkagmm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zdznjmud.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jiwbbknc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sapoywkf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zdbdwmbd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ytsfwbap.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fpjkpocc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfhvgyzl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sbkvvrxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmhsroiq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hwylxxuy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oeivtepv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhhbamhq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3owzqrdqa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ospwhdsz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpplztxg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lqkswext.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zoqjaggh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrervjai.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ccbituco.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3yrqmwcxr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3onvyflqb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ddtnactc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwcwxuqu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gfjmslyk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3llayfrcl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3byxvmscz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zldwibec.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ezbvervj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vjxcwjxb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnkywrui.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3znhftvcf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3udugfsfd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3iqdwnqwg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vglbqfzj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3trswfzpr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ngtovmfh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bvbwxiap.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3smcvcndu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3yyiojmae.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sufllopn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dcwwxmtj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yrxbegos.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvynscku.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3odapkmpv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yecjpaso.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3jdinluwa.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xjxedjsq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3dptzrjhq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bagaasuo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yycpoqui.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qhbjxxvj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kcisifos.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ahauspog.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3niqyekzw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ppdsauth.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wscjuepi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bddquqau.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dypdltql.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mnctqwne.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vajoqoru.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3uirttvta.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kctnnxsh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3liambike.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zhhknsjd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3najndcki.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ykpftekq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ajklzfif.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mknqnocr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tfvxomyc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3fxxepvcn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3egatngrc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vvcagpqm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kxxlfjne.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bcekbowr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ntgbzugn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ebmlhtjo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mrbmbxbc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pksakuwb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hbpjggnu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzcqruvz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gidbvrvj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rlstuohi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qesbjnlm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gnwyruht.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sifsvdhz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3czmangnp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozojumwk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3idwwkwjb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pbfupdix.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gxqvcixh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vrslaxuo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vyzuvcvj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ehtfzmqz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vanuygix.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hvhncpia.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kkrcqllv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lfugntkx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wpvquisq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fyltqixe.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mcaywbui.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gnrhxavr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fkfvhbvn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fsqhjqpg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3cpgvrbdn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nzknjwqy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jyifpyrq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gffpgzlr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3tjprmuxf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yeqkacma.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3sdbgwcbe.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3knrgouba.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3giugtuot.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mvivckem.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ywfpkjkh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jxsernlv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wlpzduov.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bzsnttin.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ditvbrsr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tavladxw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lqjbnbcg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3uqzwdlrm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bfgmzxlb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hakpmyyf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3twdvrxse.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3orqpcfja.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bdrbdtzt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvxoaytl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zwekowsu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ouzqrbbo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sxnycnym.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvfjybew.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jndifhjc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cyidujid.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3edulealx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nxqhbqcx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dywcfuau.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ajnyrold.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iichkzqe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qboehxdz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jgsbcbka.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vievblii.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kvtisugu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3asucxjgt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tmvfbtwn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yfvyzqgz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jfykcfcx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3isbegxoa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tjacqvwb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3quojbkcp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3epefznew.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xdvtqakh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3lekorist.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ckfbhwti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awxlnjbv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3oscqopeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvaprluz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ojxlupqn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3letzxdzg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3klnhqwqc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3brvsqmxv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rlfkevgx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ikrvkcwz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ncgdkokl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jyronxqp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kbpdgfzx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mfbekrhg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dvlvfokx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zfenxlnt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oxzjslol.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jruqtfdm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vusgxecm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ciaxwtys.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3uffertta.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fzbpwgmx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jcvdwksx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kdunagzd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3uudgevuj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qwmgkgfq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ryhscycd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gliqrayo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eyqfipwv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3azgmazem.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cykqsjfc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nkropdfy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3afaqdfbj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zokslmcl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bdbxoizc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bzaeewwc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ckqnepaa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3dkurjtqc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3uhsfyslj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bkumkqym.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hatlwhah.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3luuuosvd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lqyoosps.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tvalnufk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3iwnvvdsr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mdjzahti.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mnhgaqgp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jiubnvgv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hxirltca.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lynrnmyh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgvbjljj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hjfnbdfl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3iwfxflvt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gryznzjr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3blfayuiy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wgtcgfqr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gpqcguiz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3loijtart.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3sdttxmlq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3spjeucwa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jrmdpjbg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gijeagii.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3refwejnh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qzqppydx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ygdncdpn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bssbdugx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3goflhexp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3idbqweon.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qsrpgguy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zorgnmui.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dborzgxq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lvbsqijx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fvonnxww.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zfttviau.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xpbjyjdb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3taqquxix.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ecqoxszi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jvgdwxgr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xgjeefis.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3yuidcxtn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3seqjgvlh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3khrjpdlw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qrypnmoo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3udiifdtt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3exunrqht.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gmdaelfh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kxomnaaa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sixrphrl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uxrzsubd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zlrgiwil.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3iyjaeecj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3omwepgms.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nfstgeps.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qypureie.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tsjklnys.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lvudkxst.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3aorljtdk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nwwwpgzq.html


<!-- 参考信息 -->