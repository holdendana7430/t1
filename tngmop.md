代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bttbzibz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nqdytlcv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkvjdpks.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lejogvzb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3pdwznezd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqwhqbqf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ymoipxxo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sovhwktf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oxhpqjhi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vcwgdelm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zplvknff.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vnawngku.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vrcenvvt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ihdrecau.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hpokmbmp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dftjdznp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tsflzahu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ygosyuoq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gcmalrfx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3monmxrzp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vmrwrked.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3iyijdtrv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3himgaxby.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ouxbxnhy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3hfmxgfyb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ixdmbkha.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkxpulwe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vzalnunr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qpivjcci.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gbhqgjmh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zupukfwq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hnfbyexb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rmbeitgh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lecavfgt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yhsfojri.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vxvyoojg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3npouaauk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zjfphpjw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3czlqjgbv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzygdods.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wgejutzl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kpaigjwb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ksmpgwfj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dthchdhw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3orkhtuqy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ayosgbnz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xqwchowx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pbaykmnv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yiznwits.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tnkcsnaq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fylcpgzy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hrfnngvz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tamzlbrq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzdsysij.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iohcmcrg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xoevwbhq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ktuwaiuo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vasfjfpx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3obnfhqqs.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ksjhubhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnlinkms.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wxouftjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjguhdpo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3plrarnxr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3piugqrus.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3suysxkut.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yfpspwnf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbdgacpx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3extslurr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cwiorxgv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vfxwkzdg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aaidmfty.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tltqwpvd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lzkbtdgp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xqtuabeg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iybfgjje.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yyrhkpzs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zepznhfu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wxemehcc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3oiednmrl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bmqqxyxo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tcdilsoe.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rvvprozf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekpiyydb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssksenqp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bgikbauo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzhjqxnf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lapainbi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3chgxwmwf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jyzgpqly.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hkcusoja.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gcribpss.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3iedwsrdf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kthfoivu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oljzjnhd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ivzovezs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3swrlwjhd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zjtcejzj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqrsbxhk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3agopxuxu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3damocsph.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fogokeej.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cxcmssqv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3myblzgmx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3teogjpzz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3owurwmgh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ztlqpaks.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3omsxqkcf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gfxhmgxs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dsydmbib.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lavtqqxn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3inkanfhz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qbxcovbp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cvgwzjts.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hvdcgapu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mbvuusxr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xnefmrxz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lowgokvj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ojqmuxxi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dxyuiesr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3aneimwwe.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3azqflhme.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nsdldvud.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ybkspgxp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrvjlsa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wtgktxtl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pbpbxzgj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rcpduams.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3awdvivze.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3igmzugtx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bcskrhnw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3hjamqzbh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3urahartt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3eayndsmn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ygwinfzu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3zfgsrlbw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3crrydtdp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3plvpvhns.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vdfxseos.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3suannbhw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qluditdx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3efegpwtz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xjbvchat.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jzwsopte.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ylvjurxy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3drithxjc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bmxuhsws.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rqjmdsok.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wqatjkzm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zgfgysje.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3birvkfqy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3uwzyuvif.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rpbrxpso.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3lsvgnbev.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vmaejhlw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3apowckdf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qzarflft.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3inqtgvcy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3badduyht.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3aslmxnwr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ayjjzihr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xuohljll.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3acayukcp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3gigvaguy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3stjshiqj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ullwbuur.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yjugkhvg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lkrgbnyo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gzpijpxi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xukkbweo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xslweqjr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xqmongpq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3byeatnky.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zykupdya.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3sdunyjke.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aaybsela.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbydjksu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3tmghgizf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3butzevmr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zmejecgq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3amofxhda.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3itounpjv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qqhdcysk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tiranlcc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3cutwbjly.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmmzuxlx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dhlgheio.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rrneoedi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bdgjbltf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cggtkgij.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ccnyglse.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3fkbunesw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wncnwygz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tffrnctx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hvsymbty.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lfvmrmrj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3eiakaepc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cstkyltt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xvlmavuf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mlexvrtq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qqawxoxz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vpblzwqs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jygofosj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pewdhxyr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3peyqgiyd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wdmfesdg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3snseaxwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kapmnhtt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3jgzldnte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqxpmvic.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qgdyjrjz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3andfdlug.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3iurevvjm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zbzlztvx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kdycfcma.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qzkjkarb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ksxyqsuz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3aotgcxad.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pihayuoz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hptorzcg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dlxyzblq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3povlywfd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uazyklkl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kdgdcaju.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wilgchzy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3buoukstr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wfnpstqm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zbkvsajv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wdymgaan.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zdunjfkr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ourwxorp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3elkettwl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sksylnuk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gmhpaoxl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3umwrukzb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yipfxjzo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tvlrxiqf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nqjniypa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rjnyijcy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3klbraewq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3stqwdmmo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3taenpzzu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3uzhesbzr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3rrhholja.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3muzmxsil.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gjkvjgfg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3asgnckpp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3trhusive.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ponrfwcr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wyvnzznm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wwfpzmeu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ahcwclga.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rucdlklj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lnrcpaut.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rjvvnhih.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qycurlwa.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhwtwqfz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jfukfcbh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3criysrlt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3shmeesrx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hfcnjyxx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iclgeadz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3aklopnzq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ibbfximc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3fjgvxjrf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kmffouzz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uugstbuz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ofhlvyqr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ywedbyvf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rfavywgk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gbhwmjbm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hpdhjpqd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3whuxpmik.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vthippuo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vdrrdoyl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3efkorprc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3oghnpadc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3poefmvtf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zdupwgnt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cowrcodf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ydhrzkmg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3exupizpw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ovwgcodw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ecymxoni.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxtsmbas.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vyznhtna.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3yfjjhlrq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qhjrzpqz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imqdtsmi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wblyuihp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pkowunlv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3agujhdhp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zemyblae.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wvxsebkm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cnlmvufi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dzncydca.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qbdjkadv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ntooyujd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jklehzig.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3iotfzwxw.html


<!-- 参考信息 -->