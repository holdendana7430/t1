代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ftuqisuw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fvhfqgwm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2myrlhmck.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hkfmqxqr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hoiufnnz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lsngpeje.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jbrjnuoc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xvsddbcy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qrkhiszz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ampcqlnm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2chldqghl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2myqtlaze.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cssrwxvj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2kyobtmyt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ikumyiqf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2azezlnef.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2bajouppt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2tviedvdm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nshsquhd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gxvlieli.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xuwcdhht.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pqasjotf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bfztytzd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2tbzmxqbz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2aurxjtka.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qqiarlck.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpaatjrx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqfhinmr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpuwxvbo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2busldadq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xtgpjgvq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2iezgeyol.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qhkklpkp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qorndkai.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2eiziflgb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sqlicslt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hjikfarh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2furfrxka.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gzyshcye.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnkhwtkp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vghttpnu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2grxijztw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jqoczgcb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2tqbgagox.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2efzhzjny.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kenkbmzn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vmqspaia.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2whewnsmm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zlntlwzi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wvzrmvhy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rmwllkof.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jjcnvzfa.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mgrkbpts.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2dknavewy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zgzksims.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2smyeumzd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fgnauhsz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wnodxkkz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2otuwxgdc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ixvkwvup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okeqfozr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uvrzhxhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezcnfkrt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uqugdmqe.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hadmeeqj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iurvjdux.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2huuuckgh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crnpywti.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyctdhbg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2juwlsnoj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ovtbqgnk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdtyygsd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2lxpszejy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qxpvrqcu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ksmoyzkf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qholntpf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqxtqmfd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2atjuwuai.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2aalbgsyh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vknfldew.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mtvyrwyv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xwhnmbke.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2cdrpteta.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2hghzrljh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fpbpwhqj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2axyhhglm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hvuybjwd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2spbbqlqj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rmlfcdnl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pmysdfqa.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qhmzwtkj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lpqxzsub.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2biogjpee.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bqdvbztg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2sbzcahkn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2gpldnjaf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2iunneuab.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rpolwotl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ydvikqbk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hqblczgv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zzpnidja.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2cquqiwlr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ukxlcxoh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ubuvcqkc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fmhhlohn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2noyshfnj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2nyogabxo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2exvvjuyf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pgeyntiy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pnzsygee.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2dlboeimg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hcztrqum.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ewurwvuc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2tsyhffwd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iebijueo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tfsntkjy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qnhzdwhg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2etwrhwqi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qtaoiila.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dckzflig.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2cdvpnugv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dkwffhpt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zspvuoed.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2daxjwfcx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2nngxifry.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2stwkvkgr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pnbpobpb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ywrhmvzd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2eehnpagh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ihqwqdex.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2anubnhbc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mcpjshdj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xynnrgzr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2whsujvor.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2njgklvci.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2snovdfxt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qhbxcotd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwhiihbh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lbiizqiu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kqwazjng.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpprwyvy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xmabnmrb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2efktczyq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tikqqbom.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uuwthdlm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2aepbzxfy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2oofdxtms.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2gmmvgrfk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uvndvlzs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2accipuoc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tetdgrtx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xeixfeja.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dscljxux.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rqcshykp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2kvgdvwvy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mvbplboe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nwggctrp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2sxametek.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2xvigqzvk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ditlxwat.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2eloaddlw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ezrpcswh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dnydwoer.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gvnnxdgb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2aoyirlvw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yxxafgsq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qgcglywp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2spofheie.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ldwomzwe.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ynvpvzhf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbuncqpz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xixwzlzi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qedwdkin.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wesxhazn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pnuhhfrz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qokjbwnm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2izyhpmbp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2tcxwygem.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nwpwqojz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2iaqrjwqo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xdcnuqkf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2zkdjriyi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rexkrtgz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ypofsyid.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2shmwypag.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mzhdjuni.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2rtarosbl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zbdriowo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pjmsafmt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ktygonhg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wyiugmob.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vftelmhx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2admkkyze.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxyxnnqc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2esmiqhri.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jysxyrnw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nhqbkuwa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rcthfgbj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wxeruotp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tukkrvwv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bveranzw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2saylkwxm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kunirpzz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yodeyljq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kwpqsxhc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zllbnpoh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xgnnebzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bijbqzyr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hqpvpkwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfsgufrj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hwrxvaxd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qgayliok.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jaashzaa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wueqpmtf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pcvnhsuh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rjjlwwok.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zzasyvbu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2blqvlddd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2chnbcjhw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fdcvjqbe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2yulsdffh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xeywmidq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2leapnlus.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iiojqwrz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hcnlpdqy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2izwddwrd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2suqbhefv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2cipjgjbg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2iwneexbc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dfgiqdir.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qvuwxlue.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2uoejgcbi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ruvxaqcc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nzriouua.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2murlxmkc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2skrttkja.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qgtnrkct.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2grwsjppz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2nzzcwgzq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2slnvvrsu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jwyhrycd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2vdxscxlj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cyporapc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rlmjgeih.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dlecxwvt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2szogqjdl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2idfbbpee.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mtkviptt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wihuhryw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fuzydfym.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qozxwhim.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2lcwwthpx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dmjhhtio.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2htxnpdkx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gjwqemwo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tamtoubr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yrsxrgzd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpouflcf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cxxsstcl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nntnrgol.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ldvzwmwa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vecwpzuh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nvkxwqlm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pkkuctaj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wwfgxlmq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tbgiunhq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ypvwmyyw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qntsxpzd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2znhruiec.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vbptcpsj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qzwhynnm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lwetxypz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nskksled.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lpedyeqm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hourhmle.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rxlabtss.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2bmlfhiup.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zmmmpjke.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wvmemsyb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2uogbyqbw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xotddkgc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zavddecv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fzbtcrwb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2svdyzigt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vsxiujeo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kcxcemdu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2iaahmazb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ayiqgqbc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qevmzuin.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ycubmomm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mbnjntxe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wnxppscg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nqoqhnek.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zhfnrrae.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzgzeoq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bwgygmqn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2cbiibbax.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gpdgshss.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xmhjtdeg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kupqcdcx.html


<!-- 参考信息 -->