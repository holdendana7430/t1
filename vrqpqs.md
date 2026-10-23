代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvjoiyps.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3duosyrsj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfjyify.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hqxnwwrs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kynyzwwq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zhbkwwdo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzvhvzzb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iupqtjwn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kmpunmtp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kceautub.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vfartvta.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cnniogrd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fmrbfnfv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ppbwnwol.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ehfmwywl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3agopmosu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ycgfnsyw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vpmvclcx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lbpldmcw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3aramkiru.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fkjpamjz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tdhltkfn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3urjesiga.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvbmbzys.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mecgzmfb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ulswxtja.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3igrokuex.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ycmgnhqz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3iovljgun.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wukrypip.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3brltvwgm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qajhsgkn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgqjdpke.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3nykkwqpn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ucaqkbyp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lmygsrmn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xrubpqnp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lrshesxh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ksmlexbw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qkprzhvf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtazwtnj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nghvdpeg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhugtjbo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3khfgvxrm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxqtatr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hlezozvb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3iiimtnyd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mhhacbav.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3prndcmmv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cpkqpxag.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fzpcwdhf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pdhiaemn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tcjprbww.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ihzyalyl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lhiirlkr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vzatcwqc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bcqiuykk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qhzyuxat.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yqsuvyzx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hykltext.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wgpdyszh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dmtrssyf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ragslgdv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qoefnfxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsvtnycd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cshatuzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzxqcsqj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vqbfnmfx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nrmtitum.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nuyifyge.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fdgzirvo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnlpulde.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dysymmjd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zxohwspb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tagjfnyi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3loyededg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rxcyiggq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fkntqngh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3efdgrkid.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3neixzonc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3upvolxlp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xrhzybng.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wkawfrqv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rfdnoubp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lgurbskk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uvajnrwu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mjwddrfr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ckmlmvpb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eetodeln.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqxmhnkx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjqrmnof.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3jtqlvxkj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3pqafmluj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ejvlqvma.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3svddvlzm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3twwwykpo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hsvqjuva.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3muudlzfo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hkuxbzaa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3iqdwquvi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dostpulp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tbbirdup.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hbimoyjh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kzofqdxi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bivjepcm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pngnrgli.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3baromkdx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rciboytg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3heqthkgs.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ijbcfxnh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3plszzuck.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3xguurzdg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3infgcgey.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3otdryoqk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zhbnxutl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jbpikrnt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fhibahcy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3clcgswaa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mnradlae.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bmkrurjl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3owjdkmdk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pksmqpzy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3asouhgao.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pdfmddkv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3csaewjyh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3saiorgrf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzdwlwtx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3snfnkgsj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmtrloz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3qhreyiht.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zbtawtdg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3fdkgkpin.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gutybhdx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pnevigso.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kcbvcyuj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vvfuxtfj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3arlldkry.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jcfqimdj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pabaprbk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3otowmtfq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yraqohgz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rneoptim.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qumocqke.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sslxsqxt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbcgwttp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3leasritu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jaaricuy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hfrysmtd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cxgychav.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3warwumxw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wmksmdjv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jhpjwmvp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ghiclorv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uchqonze.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3iboxipis.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xwaxxffc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3podmkbku.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fyqeuuqh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3yzvzatsy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3yloqioga.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cqaclgpz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3piefgdum.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ycmwypfy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3atmwmmgb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3yfwhljvp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fojqnspd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3akwyraxx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3icoculqq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wntdvsvy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3auisbufk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ohpuvwaq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3yhembqua.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ciutflbv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3lfanphgo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbkczizc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3urcrnngr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wlpuwupg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hvexxpay.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3eobyqdue.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnbjcndz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uetpeivn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fjwxkxih.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3zrzwzwqj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ukcyhwnl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3irnvjpmk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3oipgkiir.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tnxeinpx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3awkmzrfn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwvfdolc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hifujyit.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3pggxjnzu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wkcopfrg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ejqmrtfo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mmefvtce.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tklblzmv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3igxwwndl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jldomvia.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyhkfzwk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yddyiuvq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lrjarzhu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hqdgkkzc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3pmfdlwvx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wadrrmnq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ckgnmzwb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3izkogrhq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3psdgypqd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bpjgmqav.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tftoidiu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rfaxzqkx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3nimrguxh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3woewuzyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmcyiubu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3tddllpcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afvjroeo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vjmjoeqe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tpwigkls.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tuestjeq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zbbaywri.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ejixsqxt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wbpwqfwf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3znibcpnu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yqubvifd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qkkzgjsg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zxesqvao.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mpqrwgpj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pgpbbgfx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wwsiqmos.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gwqtviyk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rvkozwjp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bstkzwsf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3syfhmztz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aqkwlmwc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rqblsqgq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vbkbnhyw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vbozhout.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ryultsdq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vjlrlyje.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ymcpkncz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wxwdulcv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yvrzswle.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nxcvmrmy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ognkmalj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wzertavq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tecregjr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wuuutvyx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vpfnqwnt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xhynjpwx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nvyfejtl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3pgxzgcbt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lxskhloq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zkcamahq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qvnwosoj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zukohvqh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pifowrbu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pxkdzsbn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mlwtbfxa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xnroxpbq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jagfiaaf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qehqqywq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yljcodsh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wmwdtulr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qdmhniqk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eocvgsdv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tsnfrkpj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nuopswvh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3itopbmrj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3eyifqqvf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3iaxfxdey.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ovxzfjbt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3kwbfdhon.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ptozumjb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pslbkxyr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xfgplmpk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vehjhzvq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3bzqkuhcy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kirfuqbd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ukxsndws.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ifatlhvy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hmijphss.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3utwdxkfc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3vxdngigw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xcphnybw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tlthuzjr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bcryzpvc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bxajmdzb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uncgvirh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ljjhuabz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jxgwljur.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3cpgfyabz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3muflvrdp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wapzrmur.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tdspsplj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aderhiwv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fmjgdxzn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xxpdnzgu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gzuyuddk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3czpkyzhs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hikmqnpj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3plmknhkx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kpawxmmt.html


<!-- 参考信息 -->