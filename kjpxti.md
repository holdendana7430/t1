代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iyannxzq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvreqyon.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bckudgze.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2whacfzud.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jzuxcghx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zzijfcza.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cynglymi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2awqxweea.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rqzqzzvn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hbhhrzdw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gxybdjta.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2kqredroz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gaakkraq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tcclkzlv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gfvvpnsv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pbyraqwu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2igtwauxr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2csgkacqw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2eosdrwhp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2pwtlrnft.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gvsxgxxj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wigzlfxv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwfbhdmq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2punsrtgm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ejlxwqum.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2pyqlhzkk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wtwqlkar.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2tvhaonxj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2webrlkqs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jxvgiajd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bpsbhkny.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nkpxkrjs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzhewxze.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vdnvatab.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2phqlicpu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2twgbacqq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqgdbkj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2drcdjzms.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mtgsmozc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lvqqneil.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2nlwrwyta.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ldzljhbb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ryebygba.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nzpnwqsv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fmixbtes.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oxecbwvq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2raircjgg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2cqjxnaem.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ifichcsk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rzlhomah.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rxzjnxme.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ygdbkflp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vjnwojjn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2altfasnc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ldvarsid.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mdkzxfvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxhggmix.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kmaltsjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmvmakse.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgeaqopu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ksxulqdw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2afgmmezn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ecyjieec.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2depmuicl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpsrencc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jnfdttrv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2argpfuzh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rfaqxbqv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2aptvkxwt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nznkhjto.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yqapxcfk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrakpkzo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jegrhqyl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jtvoytri.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2runvtmep.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tqtjcdvq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2knkxiopu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2azehcivh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2njypclap.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipjgqabv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwlrixlh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcsxxinz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hikjhzsg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ldkxxyqt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vprljsiw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lgswxkku.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qfkmfusr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lfcamnkp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gwqsrpte.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajseyfmr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vuswlgtd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2aqqguqgx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zrdadqbu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tdmqevnf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrlrxrm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2tyjtczuh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wiaeantb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2darwwqpo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qlmjhuab.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uczxmike.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2llijkrwn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eyopaxjn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pygyodxr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2oksqfxme.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2plxfqitp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ggntwlgn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2sqghgxel.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pmqcahpq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2icefmexl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pdxhceek.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2skavyfac.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kkbfpqhp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zbuakhrh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2sqaetuyz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ozytuwqi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vgowidks.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2sqtozoen.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2kysqejfy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2qxqscbyz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zlkwgacj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rrhxftpt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hcygwfle.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uqwnzhpx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mssysghq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fuuzromo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnomphxw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dqjxnict.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jptyvwge.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kuytnvvs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fztzfkxh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xzsafofa.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mnruklfo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2plartthh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vjxnqifv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ignydbjy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pfkwskyd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mepxecor.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2iwdnyrkp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwigmte.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2uzonyaxd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uwyrixve.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2sqcvlopv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ygsbuddm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qusjfjtn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2noauuerx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vvfdyhiu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ztiihqbx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2htoelmbb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oystanox.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2cspzhijq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fwmdkuqb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2apbfjyxz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2oqgogkpj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xlctittp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2nmibwsik.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rimmnvsm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2pblcbwlh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vmjqyqzc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cgcrxmcc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zcxioubh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qsktnpzd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wzmdbuse.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pydbnftm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xelncdqj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lzyeqskl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lecdohxs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ubtutigp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rafdbmsd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ahfrxygp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwivqdjj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ozqkrpgg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxzunxcv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2niegdxyn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bhiethfq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tfjgkodz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bjqmztqo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qovpjolw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xxuvmrko.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tajtfhzy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vcyaqflp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mieslonp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dgphpkaj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2gsrlkwtz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mktqfnrb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zrlahmpo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2efvcjfrj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nmijccwn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kwcruytc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygzhnhwj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwfopuwj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bpfygoxd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pehrflby.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wcgjjpdx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eatcrkgk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wedmuqig.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hbrncpnr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hehiqlxh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2zngnvfms.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kiakcwkl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxscmwnk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ehiisdli.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2acrkooln.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjjstupe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbtwtwvd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sekbeexn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtmyekdv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hliudbvt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cewhwhhd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qexjhqzg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qpuaggjx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2suhjcspl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ixdrdljt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wwgrdncn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bwliplrr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fhnpigcs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fysrukof.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mhtjrrsh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fhyjlhtm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zjujzcib.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yzxhqujq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cuuujevt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2yocesqok.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zoujrout.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2drwqikat.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vtpaudwt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2brmyljbo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hwbwsiic.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hpqqexhr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mhmlrfbz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2egngiulu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hrluwngz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yntqpfxm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bejgvudk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rwlauhcw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kycyknll.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ibwuizta.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fsmerwvz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2inwzznjg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wasrtaub.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tjqlhwwh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbzcccz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fflqnpey.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iwydncev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dswwrrzt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2awnsftes.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2imhgktnr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vqgdtmej.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2admgpvyk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qqladhzd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cdvnxkbt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ibzdnmyo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sbvqcvzp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ctkwfvqw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2axrbqyri.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ugdaywkk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2soyevinz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jdoonrlx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ueexrdnj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2soktdkmq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2lnowxnad.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2zpgvzwwg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2yldrtzoy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2feerryoa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sivhiiyk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bxfdcmin.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cpdbdmlm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lijcxhzm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tjvtpanz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pnviyiwp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wxzjkxgp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wkweesew.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vgeejimw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ukqfpofr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2smqfpscg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2yvhxxczv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2fzwprlpd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2reduvfcf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ezcrmpre.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dzzcvlck.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fdaetkch.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yfyvifmb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2xtncmjyu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vlghmolc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nwywraiu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2upkjtgaa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vulvkgwd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2blwfredz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pqfnubkg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2nzcafney.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ctqfkqjz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rmigoitj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qncfagac.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bzeewhfv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nlqqnpvf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2aguirfyt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uzlljqed.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jxidsuxd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vlizpeyj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hcuoifhj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xrzodspe.html


<!-- 参考信息 -->