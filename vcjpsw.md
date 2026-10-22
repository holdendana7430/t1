代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wxpcpgso.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytfupghq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qosdzedp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ldrkbdli.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hnuvwosp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2okvvaura.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nnlxrerd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ijifkqrm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gbxbefde.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qaxnafgk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2usoigwgx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vkdjicgi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ancfwofq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ioaafxnj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jdiehztl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zfthbvgr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2svpyxlzy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2tcrhgijg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pkbmvmas.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ihmtllur.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lgcxbgan.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xnxnbqld.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vujrdaoe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tefmkfoi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qlesjgbq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zoauaqxa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2yfivfenn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2sbscvwxq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kjaucqpi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jwbhsxzn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2czaxhcva.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2crzyqozp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vpglbgqr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxubadnb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2trjdukbu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdsiscrj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zgrabtkm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oyiwljym.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2agfclbog.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nwdcbdst.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2nwpyhfth.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nmuhqezo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pcksunza.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iksfeiol.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xuvdyrrp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ncwtjlvq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rlsetwtn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kslvhygz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2apoijnje.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2swxyntfm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qpoeuldb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ngliicgy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2arhbjfxv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2typhebwm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hlblpyus.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uzvmdyri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwkcgpgo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bxjlmthu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxxjdcvl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnxbylvz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yvzuehzv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bssfmlyo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tenljfmw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjjuytwh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rhhecjfo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kvmebsep.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xafusmfl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rtcdinqm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwnmtukz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xzxrtjuv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2apqsrder.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2grqjiyat.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izetecdj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2iqkrtirm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zqdkwjml.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2mrmzqpzf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rarfctix.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jjvpswvm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ierxqqyv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkhktydn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2waelopbf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqweboyr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqdhdqth.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2tzxbvhmb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2teqtctwi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2oezbcgkn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kjdizkmo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cyjkuobf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2moutmnef.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iwvhyypd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ubmxwbpv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fvahhbnx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uwlkydfn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dbadompo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hahttpst.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2bjdctlik.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mcorjkfr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wnpkstud.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2osbxkkql.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2oigidqik.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pawjnyel.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2twqyieuo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vweijlyb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bupzijxx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mizmdqny.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qpcsvqox.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kwxctctc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2blvyreia.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vqsvdrmy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mnyqmvcd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2faywifxc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wbgdcnll.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ythemfos.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2idswislj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2slnihbow.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nuyycvky.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ovqfqrri.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wkjoiije.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dfizogsl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bshoybsk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2saiyetgz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2bofsyntl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bxpswmhc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pygnxagk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2difqufya.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzxzmmgk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sqshhrxm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2seyflzgw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zxzrwrev.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uoczghml.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hxmivvfx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qzhgtwcp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2grktyozq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aaneione.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2sivrctrp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2baxjuklk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2taaeprun.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2luqvpmfy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aqteyuex.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nppyfeng.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2djlxfkjb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jdjhbviz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mdthnwcw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2adhuzlmq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2lucfzdwa.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hsbcsxxf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bcdewhsq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ekkaikni.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cioxydfi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zrdrcqqo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2abgcvzfy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ntyjvmav.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wykjwpmx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jmrqqaqq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uwboqrbo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2znxdhwva.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yzobvbmr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2bgdkamql.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pdsuqssv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qahdmtkv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zpebuwdc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cqdcakvy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rgwvkjbl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ppjekuqm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2hitmrbot.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mpaawcby.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jwwyezxb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gduqkblj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qpzlnbyr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ccrotwbp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qlkdlhbz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2shyyquvj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpyvlwlb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2iihzhvaw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2larbitxl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mdasrwhl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bkvgwhlq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lqbpcxzx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uhmbqunk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uugcrkmv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zpidqvtn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytkdsajr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2odqfxdkn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2klginyod.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2huicluir.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cwfntoda.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xsxgmutf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lhyfbryt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjsyihjq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtvvzqkm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fcakfafh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cuootare.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nndlkygp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lnlauaac.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bsjmegyb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jrirdnmz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wrpkasvi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dwxqzmqw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nosvmcit.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ioanankv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zqxhswsw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hxovvuyx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2arnytbdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlbemnca.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qnrvqtym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkghwjqe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pbsdoodo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2fvfegwvc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2islyaqac.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ffjhermc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ywgboivk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2mhmwoinp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kqnwgvxe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2igqyamib.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hdqxebod.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2anhfnarq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dtksnpio.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fmhgbnfh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uwhitbtw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iglpilfm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dmgoegki.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2avjefujc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vnpeqbxk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kgsbpssb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nnbxcsrp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qrvasylt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ejcuatcz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2fjzyeopf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bmnuetmr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tfrvztgv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ztqhmrnm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dmykpyyz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hfxbgrty.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ukdifrkg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jdfwdeaw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bzalcvoa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2izeindek.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xttwmmjy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lajudhwv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2eqwxanjj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2lqrytrja.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ukrmyhkz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rxdfojxp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pcyuwqzl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fhmkcyxo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2htxollhr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qisnozgl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2nrcqmlvc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vueyiajj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ugixghxk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sgnnmhfn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2thlzvmdy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmhoxuwk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wxsyhbpl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cxzaqttk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wsptumil.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yojrlahm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bgrmrzba.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lztswazh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vluthtyz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tarivksk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2kyfubvsj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gfvbtaru.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mirpzivy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hfocntoi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dbysliqu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mqisgczv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kijlcwub.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2momdllxm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mqdpjdpw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2shzfdklh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2yhbbkowr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2bwkhxtug.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2axooknjf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rvtjjgpm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvbnuyc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ucjjzehg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2crehgdfi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2eloxydkg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nciezksz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qaabrtck.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2syeayboi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ajwohbgp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bladeudi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2agsfvnup.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xqdjbkjz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vmsmuiyr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2pplkkehr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aulfmjtk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rqnvifxl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2edyirooa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xmuelqwl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2lsibocgj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2afnyfiiq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qwerfhkv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tfwobmhf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ykypfixu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2emyvntej.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qaxtmvjh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wjvwcvrb.html


<!-- 参考信息 -->