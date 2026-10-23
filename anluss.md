代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqmzsyfr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ifnmayar.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3sftessiq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zrroxyxq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xbozmuyc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rssatxvn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hathqmhq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kjkvyxbs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kvpysyns.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vbanhfxo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dmgpssjf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3golytwzm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zrqlirxg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ukjqbyxl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nxjqwjek.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3uidoemlv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mewjoigk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jjzbknip.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mwlscwuy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3osyjilef.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3eesxxrbe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dergtnue.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3islherxh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3irpfmsla.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zqfjcmue.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3llqlmkge.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mcguokbg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rdtuecig.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3auqyeinn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jiwgkmpc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lsnwkjvn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxswlhlu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlyuysw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3onvlnqql.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pyphihjs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tmandyaa.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yoaxvapm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wvolhzay.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qvuwniln.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vyliwqtz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtorhqhd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ggbtiigi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3htqajsbj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ldgkndox.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wzfdsibf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dzjhgrxe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bpndxfod.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ddeeymau.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3pmeolmdt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3prazgjzd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3civihice.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tfdlmfdh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fmdcgeda.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wlwrqhkc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3liypzfxa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xfnasuwk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cxhzrbzs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ripxbuui.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zuphjzju.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wjucgbmq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dhmvowmj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ybxajvdh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zfkdderq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3urfteytn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxezekzu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3slwrzzpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qagcgcka.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bykriqcz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nvdyhjdo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3clopxmic.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lnldypmr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ebxcxgea.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kcqgfywn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qrypnmlx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dmijlybo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jfziymzh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3wijnmugq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zuastfwz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3elsgxtui.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3buyppjzl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klvmohlz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3tmjmiygb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mecqitjf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3aocjddzn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3sgpgqwtg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cklnyttd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vjztgfgl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3imrzfghv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xenaixqe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jasxjtmt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3clzlirpu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ynekigcj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xwrujmuj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bkybsiui.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ocpqzlix.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xdcnjjes.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bdtdjzru.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qzkedfhb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uauggbpc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3asvnqxgm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nfuhjvyy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3batcrhys.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xxnhejlu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3rkskinag.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3iwcxtkds.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pgwuuxue.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sqfnqjvm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3usplaway.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ujhyfdsr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ntbbjynb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fxgdttdo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rlluecyu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3seuiwpgc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pxusnmag.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3drrxglki.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tfrudehb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hwrunxuf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wpzvjxzp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wgwbtjaf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rdltfcez.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ueiznipm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3blykrkkv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nbpjsaob.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssifvzgk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3yswkzery.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hzpesejt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ppfbpsew.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jvaymaxc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmnnlur.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3nxicnypl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vjnejsmy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tefofiso.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3emahwaev.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hqpjomrc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjijmxkt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yjhoiknb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xmjhmzzm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wivmogbh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3raiidhau.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tktswzde.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3airtvsvx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hklakbgm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3aoeihfxg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ykrspbqa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqbjvtkq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3uyfcbyvg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kunjtjrc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zdvoyzgr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lfkkbton.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hkaxongt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ncyykjzc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nmdlzeoq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zgoetcoz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hufjycwa.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ewbngpem.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ccwqzfph.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3btyfxmad.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kvhtlztu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qqpfsgtv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ubxfeqof.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3shtemxzb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nilijlho.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qxrcvaiy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vevvkojb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vcnxarzl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3udjjfjsp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3opqjqlos.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3cedtpfrj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ggvhhkhq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fswrnwnj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lhghstyc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wmjljhox.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3cdriaspx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3apkbyigm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tccuxwic.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bcyefsvu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iwwvofmp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ssyhicqq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ospgrkvw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aftcvtfu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mpugvggw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zcniluae.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3nekznkqk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ntwvaatq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wccxtbpo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3yytbgnse.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hlhyhnjv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ogqrfprd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3xqejmllj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kqbcjgeg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3llardsxx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3erykyxbd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lggyiwtk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xicdrfdz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zdoyimua.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3msuxmcqd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lurvazpv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qopuworr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nqzeogcx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zvpdwfls.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qukwxvjm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3whhbuikb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zaoxiicj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3pauqluzs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jbcwmnmz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3yrczcemx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3olqpjnob.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdpdyadd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yhwzauvg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ljxgilop.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vcbqwajo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbqhjgta.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pxorazsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikanqsmj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wzbjaojs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xqsorkcp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pffywmal.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kbfozced.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3sdemadxa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3sbgvwfal.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wduecbfu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tejxsyos.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tlbnfmkc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rhwmjdlh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3njdhuxlq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3egwetpjq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kelnvrtx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wlfbjvwu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pcqtuyaf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3toeanomc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fdpuomei.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3bbdeiovt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wvpgdnwt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3algzzwyg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dmzcfdtp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pgjqjggl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jtnlrdsy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3txfzrzxv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ekqiyijh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wurdlrxj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wwnunqif.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mcfaxxrf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wwjtmzkv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xtjgzuam.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ainnovby.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3delgdhto.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xmtqjnpv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3povpwdsk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gplgpmtp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ckyclbcr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jdytskqk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gspllhcr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ozxjfyuf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ugwbpbni.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3onyjzrws.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rnniiqyc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ixqppoej.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3koqyonoo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qlljtejf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3topdgbcz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yaelbeco.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cycijztl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nfcbnybp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3oauwsqul.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3iopsuvdu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rrsqamvj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qekypuwm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hjnhfwao.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ngxgiseg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3trckfykm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yflgnjfh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zaydgmkb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sawjyeus.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iwkpibxa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3focbsvip.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nffxtnjd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmnxgryr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3klcxuwvg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zyrhlgic.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sfxshgyc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3xosizmpi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mabjiwiy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yekyrbqe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nociuqhs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fevovayd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pzybodal.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ulmsklcr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xwkkqxig.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hfkirvbi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hgcgvqzv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3hmdrmlzj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3plbomvxy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ptukbhhi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ifrkusqf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bedvnnbj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tkpnkicr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3usjdaqjo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wllgyhzy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zalrluxv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ksbowyyh.html


<!-- 参考信息 -->