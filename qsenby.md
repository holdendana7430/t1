代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gzhuqstz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ydxmsbfq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3oobaaxoh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3gopnhgwk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pqnnxrbi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhjimgoq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nquuwvfw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3znllnwrx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lxyeqfyc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oaduabph.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ctpnyfgb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxqzjrud.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jvdbcmvu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pmpexsaz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3esdxjlhk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cwxjrknt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bwipqpgv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3veglizas.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fnxqappg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wqtiwnil.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sbbtvdgm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekoipufn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vjihrfie.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3juxommdm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rahcusxn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tvmnhnqm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3eszbuihb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3agghpeqq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3amokexvq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3clghedod.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3widxluwb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3aboasarm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3nazgxcve.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vczmcvzp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3rjwehzxd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbbpkzt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vrsqyuuj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrffmtoi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qktbjuii.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nijpbdhs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3macjpqvr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ppkdbpql.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3iomfrsym.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3aphammst.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3njqixthx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wbzxchxi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3beneepbs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmorvubw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jovkchgb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cetqfwoh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zysrxbik.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ylplcegv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3enpyizny.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipwbbxdb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dxsdgeqb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sfyfyxte.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rusxwbmx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wqfetmpf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jpyewner.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rhwnenfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpaoqbop.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tduxjgqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmavawvi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vdtyrqux.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3rierkgfu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pzejnsjd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yuhljnhn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvdbscwx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fkdnjrpj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dpdkackw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wenifytp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3djxuehsr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3biyklmbj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dlllqrwv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggtiajrv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mboxskyu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ehdrvlcz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xohkqggn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3yocdodar.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3nkbtrnvd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zsqpnmvf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uinsdjbp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hdgldzgt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtjtimhy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xsengdjr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kttrmkhr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvkahlck.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fxokistm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kkxygnau.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tnwhdysc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dahauadt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cloaliqw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xreftqyu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yrxnxhpm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ptgsjwcz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qbxturpc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3txqgxrvm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ejkfwiiq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tykjojth.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xrqmynye.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cztazjcw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3gxvmjmoa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ioxubffx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bukddvyx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sgqsyraw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yxllpsqe.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3njfplwji.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3saisjhsc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cyyqubnb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kdtsmvdo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rjalavzg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3atqvqibp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rzxuybcn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3gkhzccny.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qyvyawmn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nrgbkmej.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vejokdmm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3djuggzyg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxattqk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3baijragb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3mgdetlpd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3iordbgzo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqbgbkov.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3weuvwwfy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kpjurxmf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3nukakfvo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zqhdebrd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3boqbkmwr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ggsvwdkd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3exrzwqjj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ksuyptte.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3emgnubhz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fsdfmisw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rsvoxojc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnzjdqju.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3oppuivrq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dupqyyaa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdvtkhzc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tswiigrq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tucdmbfw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlrwlhwg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ccptmmbm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqxzgvcv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3khezcrrm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3azezimha.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vohpjuuw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tvkyslas.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zzzdacso.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rpsdeiam.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3orazckld.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rrwgjrxq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3uomqlaui.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mbkerhkm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uqheotiw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jlpnxyfd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3sgnzhhcb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rdnnwxxn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lyfazrvd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nkrhenxd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3uclqwxsn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ulkdpuur.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ehzlvqvf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3fktiqnak.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3alsokrju.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dgnalgto.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wbbehkks.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ckuphhpt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3llowjcds.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3tpouonlb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nznkwkxd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxxsiliu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dyyksvdo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cectkgts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ammlaktk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3pcwlqonu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfjyrdgt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3adqlykvz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3etulsqzu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rjnqrdor.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nhlosqzk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nbaxloku.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3nrubfvoi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pgpceqow.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3phaoceky.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3crdrfqij.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3frqxfprt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mvamopbc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kqgngazb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3yqkxsrah.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3udahihpw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3optcsiif.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iegtfpwm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yaexincl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3iqazcngd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3btnoejqo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ojfvwyfb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3crhsmmht.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qdyitcdd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wyhmfops.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fxlcqmqq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3arlichdp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3spaaskdy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3niinjbuj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvbeglkr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3joniblvc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xhywkdzb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uijqixbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eenoyhxb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mdcirydw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucuvupzk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xpircktw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mtiheryu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fpyvukab.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zerlhlfj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dpetaxdo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ibqkzctm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3luwlywpk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3appjgycd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3enenmhtn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nmeeokql.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fehbdvbd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vjtjidbm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ekrznljy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cxlxlkde.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3owyivutu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzekdpp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3farcyjlc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3zaheivwb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yhilarom.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ptivbpwu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jkkcsdee.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hdfoogvt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ktfuubsq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ximaizsw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3srczcnjg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gazcnlen.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3onasegrn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tktkpfnw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3jdnkkpvg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rfqxxhyy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ayaijzee.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3npfxsnar.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cwatudeg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3pcaeasrm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3flobtzuq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3kxtatbnw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3umcohiql.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fluimumd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jdmjrpaf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ifhuefmy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ctmpzthb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gfbhcaut.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3limsdlgt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mjoxjuho.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jbxxrtzf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gaflzucv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vreiopdc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3llmrhpwp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3adzbwnqu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lukmskyu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3agmuuzgl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cknpvmxf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bafbqhij.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qqxfiiul.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lslyjqxn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3pisinbpk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lvvxbyeu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ealrcowf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uroisybn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ifslsjnl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3bwubcueh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ltqemcss.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3talgovoh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3svtgbgax.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bjrqggtp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jfyvyqhm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3erizflef.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hwhdaajm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzaujnvs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3wxopromv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3blvrkiip.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lomsrmib.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3iqjkkrvm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hiclnwgh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lzmirltu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zvrvgkhf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3dthizhtk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3iebeinne.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lffycqru.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aqvnjudb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3niweutcs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3cpbawwho.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3smbubrmp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rjseqvfw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dxfjiecf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nblofbou.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mbmjfhkn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3eashmiwa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vkgbdawx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ioipnhwj.html


<!-- 参考信息 -->