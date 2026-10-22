代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uvmzauwc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vbfekayy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vgonafvu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhwdukgj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2busikjnl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lsibdnyo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gxbqwnkt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2axbezdvs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2sprgidzo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2olcdgcbr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2iwnywrmv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lolqphlc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iukwtfix.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qjucffqe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mocisvgb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hwzkngit.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zziniraf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2edrxohuu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2slcacsew.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yjuidzvw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xoawwrqp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2dkevzpeo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anjbliys.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2blxkgejj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hpelebrc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2noufowmo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2usttzvig.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zyhmszlc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2tuwyhwiv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ixrumxxl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ojkuwhyq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wyscphtr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hntakfit.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ougnhslw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mjtizjss.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2klkeofrq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rxjlmglj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hkrmczyx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nhprqode.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dbpegpve.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ctpiexhv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kkviyzqm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ztodxsru.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjdzflbg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cggkrskb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vtyvpdle.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yqlviloq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2igdvjgif.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ufmsbgxx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2seffflmf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uvxrkykh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kkudwmgz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xbvkmtqg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mfcdsncy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wghowvgl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ltnanodf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2uhplybtb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzvxyfvn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tcwogwdo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kwednogl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ejgaqljw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cylfbtuy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2yfogugga.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fivmtpey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbtwayqq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2whlejvda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqoakcuo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vuinywkt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hzsnltyo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsyhjbvi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wfpdqwub.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfrkbiut.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fzoaimoz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xmsouyzm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2udmcecrh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbmcclbp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2psmhzrsa.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jfkdajng.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zusjxxbd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxoritdh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zjbfgiwm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2geajbqiu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uzxcdxnu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bqwjbdld.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2isisubzr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2afguirup.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jtlqfzgq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2foppwkxx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fmupgaup.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbltnjig.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyddmwnu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ccjeidxj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ptcfacoi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ytkxrjtg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2cvndrjxd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2wagqfetm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2msnzcvfl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpiptwxb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2uekjggkt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jdumihci.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2krsffjuc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2suapgimz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pakgupzu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2bkvdihqs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cnlegcyo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pbbnlvac.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jhqfglur.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bizvtvpr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2eikmsjsf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zqcupcfj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lmglprxp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dtuqzzzm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2syresyqi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ktvoyduk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2iklqetco.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gfqtkyjj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2krozcwfj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2hwjkuake.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2koagsfbh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ivavllqo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tqumbfea.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bdxkhmpc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jxswovna.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbtfvbjo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rvjqsogn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pkeffffa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2uvujzvst.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ugrqtcmd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rthignfw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xzhrdeio.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pzqbkerj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ryckzoeb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2cnmfqsas.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyxyrulz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2koycjueu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2msqlppkk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2orofgzop.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2pefyrlrn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xntbdkgb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2aiasgsnb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdyrxfyq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2djqwishk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zpdfbdwj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hlzrtjxb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xvysqekq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wocsjmce.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndzobyml.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2emqscwcp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ojywxopc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lnolxoei.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lwmafwcm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vrendiii.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vbuhawhl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uaiqepvb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bmlalwfv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tbngvqrp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bdrobauz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qqnftkxs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mdhygelm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yuqqweov.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rmcmnfvo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2esxgowmd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wtdygybq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zeiytwyc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2oigzbcpa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lfouxdii.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2uyarawpk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ieruqrcy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2knzhhwgo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2iklxtlqh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sypqykxr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pxnnlxxi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dovlbnyq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2outnwefc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mgcklgoc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vdwjcdhn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hdenjlbm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkonyvyl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lljmgsxx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2winqyqwm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfphylie.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hiwzlnjd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2uqoiveqt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hnslffdu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tqgmdmqw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2odlnfrpk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yffalvpp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qrfkxgsn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ihzcofvv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dgkmmjrx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mezougaj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wcwrwxox.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ioicktxd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2aslpwwab.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tchwhhtc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tojrykci.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nhohualy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lbxqevfm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qetgllgx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qkmvamof.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2robbwqqp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2majjyhya.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vknufykg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2crejedin.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hjbipfoo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qsbmluyc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2unceaprj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2volldnio.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tqcfktrd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rzkgsdya.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsbrrnwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hihdfioz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ohjcdblp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejmeghpj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2byrnjigs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ihwbgmvx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wposftbs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kghgpynq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2oygthxiw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xixugmqa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jwkvqqrp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xdfehyhj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qzxrznmu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2lhxkazxp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ogjpucoa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fxxphqqq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qysogpzd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uxsuskjn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kxqyuxxe.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wfardpnq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ntvrgzoj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pfdpfjnz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2towejkbn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jtguyrpd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2npsbavrx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2duziygfm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sdpsyakf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gcwangti.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2haenhkgr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tjdvvabx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iqnwmaqj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rjvxapad.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2guskujud.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qpwrcizy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hqrrumzw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fyvysext.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pczaatiw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wnipnfbx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tabsxmgp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2smmuezzm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2benmprgv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qwwzkzwf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oyfkefpu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iyqlrijg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qkodqsrd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vbofdxmh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jfkuneug.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gkguaepy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cmybcgvq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qiyfyhna.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rfjnemet.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rvxfkcbp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2trnwwipj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tjoebpor.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2emaddioc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwxyabnd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2swytppnu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wzwkkzqt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2eqkwcfdi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wxnxrvtb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2suvglpph.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2avfuudgh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2grhoodgo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hwhxeify.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pbunflgz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dlpkbgtv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tliqkaeu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ilcwkqgn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pqykevzu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xvxzluug.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2nelwbgur.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xpuyhfkq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qfghfqfe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dcxqyrfd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zimutrdd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nxrmgreh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2uizhidtb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2quvxmsjv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qtokeerx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xybwffvk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2tupcyafm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2puacyhxz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hokyvkiw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dojzbvez.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jqnpimlk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2iifoveed.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2enbokxkz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fftyugyg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2umxjiunk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hjxucvhb.html


<!-- 参考信息 -->