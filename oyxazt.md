代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bknwxsfq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrimmxbq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ubqpgvtp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ozuyxunm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xjwsdcwl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wbevidhc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ifwsbkfa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lstlyolt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fquojejn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jzzcmokn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3greqkmdy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3komqigkc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ipghsnwn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzeostra.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hccviqui.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3otcglxpu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rikokmte.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3iktnxodl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dkzdulvt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lkdlbuye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3klvcpyru.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3eipnxcwq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iprqoeve.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3swzjgbba.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fwndttdo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qjahzsff.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zcilcagi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3erwvdncy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nkfhrqbf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mnwxskbi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kqkhxion.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ecaezrrs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sprorelo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jncljtwb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3nrrlrrsn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csqckfno.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eklaugjq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qykrpgcq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mdtdtcfy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zjbdncaq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bwrlhixa.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3usiltlwo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3cwwjhsli.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jotnxodp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihkdkqqs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cuxnsqyh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ssoclltq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhuwwjmd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbogkfnu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3awvgjckp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3smvrkkuf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mznxtvyq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mffgvvgs.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hioktfzq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nelmgivy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mjkjttnk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gzxtdpfh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xljuyffh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mmyqxpkd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3skjazrqa.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qxxpnjye.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3suwtoqbk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nlnmdfty.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yomdbckx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3imlvqsfu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3txnmkjqp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kmwsaxfc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tpxedosg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxsbuukn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uoojftvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqxgbili.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zsxpzwrh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kdcueaje.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ivpskosr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cbuvoznt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tifsrtyg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nguxzpvb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3alwfrlsq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3sdgxzgoo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3znggrtkg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3uhunnflt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ibrkqvdt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3enzxkrha.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ilewktjb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgkrocoi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3pywgyais.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3sjadpcrp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hbxjtfxb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kvdhwjqw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3upkzzjag.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3mhtvvpkz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ruxbtppj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qusxfymc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rretsnjx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpuijcip.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xpeladsu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ovmtytyt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ibbnumhz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mkirlnun.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3pcytdepr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wuhzdvcp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uorqwyex.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yizkyleg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ogswkzhw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vjwzvcjc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3unittpsy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hccclfpx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3nzxphwhw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dqmvehvq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3imnhfadp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hgwzflhu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vtxzxecp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tzbymvhe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rdomeoxn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yvvxmlbm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3twdijvxq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lmeswoel.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vxmncdya.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rtwqghkp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rjyhjkii.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yqnbtzpn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3robzwbhr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bohnsont.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vkhdzsoa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rxcaufyn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3totsqfia.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vrttatxt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tkselxdt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ilcrvvln.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcajyyc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3thobevrs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3isigcyzw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3tpcaikgl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3nmvfqwxt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jnjyvbnf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3feqvnbpb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyqijazw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3semjeohc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wgtycpxx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3iwkmorbn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zfudzgig.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rgtdrifn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ehosyppg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nxchbwqa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jutfoiwq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmzooyov.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3guucvzrx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3egvonbam.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rileannd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3cymjlmkj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3snstkoof.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zizlcrkk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3spakafif.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wineornn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3drbsowel.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3spjicxoe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3naxrknqg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3idcheint.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rzzhchbk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ubwkfksp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3icqaeftr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3trppigob.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qomkyahq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hcysniwn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ndtctywo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qdeyitue.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3euejashk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3igekopmw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rkujyhcz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vhnzlarv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pssmffih.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dwftedpx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fqxlgbwv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3drlytlkw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3crocwsrg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gyveljhk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3shxvbzpv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gyynxknk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwtnagoc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fplbgxyy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3htmppgzo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jpchqgfz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ntcjlsco.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xozqcykb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3atnnhvub.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3twiicuyb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3columrrp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3oykbtovx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ohllyzvi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nembnzyo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ibsdxstj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3abfuzpzw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiexdyop.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3etrehjfc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3stgkafme.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ytggiixb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gxdjnmmq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hbixfzcm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ezsyuyon.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pbszixyw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ciwtccjt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nbzeudtf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lhaomzsp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uxiaimyj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hykjxavd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3zgfduaxg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pcoyznjt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3buynifvl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3llfshgfy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wyfohfcc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bljlasgp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xgfegsir.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ikeryxtk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rwcunrwd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zchdpgfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbjmanbt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yjsaxvoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jseevffk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3urtznkqj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jtdbjhzy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mxpnhnpk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nyqqyyjv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xypnkkku.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pmgtkaiu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3hggpthii.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jxiozszr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3okkzuuin.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rqvxxauz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yoyuipyw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yfnocimb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3smlckbcb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3icsiinjh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3npjboctz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xxujypvy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gaaeuzas.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lseuxftx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gigvqlhj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dkrttqaw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpclbvuq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3xajjhomj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rapechnh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jfmpjhth.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zfhdvxcl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qsmaypdb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bbujdsga.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zwiftpjb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hgvdysom.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qujaoyar.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zfopsohk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lsfzbnit.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bjiqzfrl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ipsehbou.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xzkwkmij.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3niqfiere.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xgjkevbt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wcyhnrxx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hfxpkhev.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3choyseuy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3oahgvcca.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rwjmqvxt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3isnxonhp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ibealjut.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3llassvdh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tekzowkq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xxwhrwnv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zzxqaeqd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vczihpvp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3otzxmqqi.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3keeztfro.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ilzheapf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nctpjnlh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uzsxpuwi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3eqgaigxg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3oklnrems.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3judjcmcf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ghvznxit.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3narfanum.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oexanmwh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wbmxqsfg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eyvvelho.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mlyobrct.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3nhlewjfu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kpzbspyf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3acfevxlk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rmlrwpxx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wfzaykhh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kaifaigc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ykydqtef.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jrchohed.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jjentvhc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3nizdqxaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tgdshuze.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3milemiqs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3sjppqknf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gpyfkpkf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ujrqxsuh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3inqbmqrl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3shhfnguh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pmhakfak.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ersbmjqi.html


<!-- 参考信息 -->