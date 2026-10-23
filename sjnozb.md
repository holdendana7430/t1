代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ymlcqpam.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dwayehgl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixamrhdg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3gmjvkdjc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zxlcefkj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ohfcqziy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wggwkhnr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3dchjfpbw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rjowptla.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dbaiesmx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wboejiqa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3beetgvne.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mxdxcbzu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3zterirex.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkrtsyk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lazqohzw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ertyruwv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rsrvepeo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jjugvajk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tqxahsox.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vaktzplm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3omtdivtm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hrsflgpj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zpigzgxq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3pyrrzvlr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gbiuihpk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnyetfuz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ivhsfldq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dkuzlcfy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xayhisjn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkyoicx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mqeaobkk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fdpsrals.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3svjsbciz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kodetbrp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkrxjxp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yhgwkero.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yphokohp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wevaohhu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rwhgedvb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jtdoreen.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rznyumcd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ijnblezi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xmmsxcqu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3twzuflqf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3abkpbwfr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zujzpwed.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3osdmasnk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rhcjfkki.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jpqbmwub.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mlikhfcd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zvolyqui.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qsttjxmb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3wwzwilgd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xxqamvea.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3woqpugpd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zqvoxmkl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jgiixelm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3nwxqdudn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wqpcnthl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbgmcyis.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gqdvqgox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aloaqbvk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3daqzacrt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qlznjxij.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3glqmazpb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vcgaqyam.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eogdoadm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3keykhxtl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mhovgpuw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ljtgnttv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbtdfaus.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qehfaatj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kdomiqii.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3huvvybky.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jidxmocg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxohmffk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3azsjmttu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mrqfazwe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xerbwrwb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3oopbltgb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3umxslxrq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3lbszfslc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3niplrnur.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bmhknxla.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3civjjssz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpzaglun.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tkbjwiff.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ivwkrngh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ldylkvyn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vgldqarw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jdoldkls.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdcirmuu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgdnlhfv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bzswuhza.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3oirzergq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wpxycdmw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdsozdxx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfmxuwf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3skgexaxa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zmhkehlu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pirytiol.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3saeltuam.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3clqfgmct.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vfrmorlp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3odyrcdmo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3gogrjstx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xnkiugpz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yunvspwi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ptzmrcsa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3evomaooy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nyeckhra.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mgnbcflc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qchbxrsk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zfhmrjbf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kcuegxco.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lsrvrkoe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zzyhltvp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jzckgbqq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ydwoycfe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pllbnywf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3satokfkl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3mlemutnf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ubzrwfik.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zbqhzkke.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jfidshul.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3oyjknpzo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3yfgqspbf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3pvfhjeqg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsyzkyyz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gbgywnfz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3iavtlqnu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ecjgteem.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ulxvqbmp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqnthwan.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3igvowtib.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yaiwiluf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hnayofcr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kwwaljsl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wvdatkir.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3exjmerlm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3gxlwwluw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3infurfpw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wrlyhuhc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xgkzaibn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uecljbgl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wjjifdjh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lzrzoted.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rgdjeplg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zacdbwug.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3iwdkzwvi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vqouxsuh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ydjazxll.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3yywvgvxb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ksuxwdhm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ftdajfwt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3utyimeeg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3znqfgqdj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ahpcarvr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mugblwtk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3agvxcynu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3whivccds.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gxscftfw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ryopbwid.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lhdmmojd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zbckhfzm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lhubeqes.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tsmnxymk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yrxhsqtg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jfkohcim.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gfhtvlcf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jffuoytd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3vgtnrkhi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tkagmznv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bkntqmpp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eoutbnvo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tvyjixif.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ihhhbwta.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ovjemmux.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3znjrmunj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3kyleefiv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sahadqdg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tgwyimjn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jxseuele.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbjsqiid.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdtpzgbi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qjltltsb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sklnqxwc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3eryfqcps.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dtytrjfh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vjooptoh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zrdltpfk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pdnzgtbu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsxthzoq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kgnysqjl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3azohpkkm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3pvirsiwj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3owmyspil.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cnpmxslu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3redxvrsw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3euxzhsce.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3sbczpzst.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xltfukvl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3eswbvwdq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vtzeigsk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vdwhmjgk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3iknfqghb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzrgauud.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3arzwyjsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmykyxao.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tjfyiiej.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fpnppmys.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uljnlska.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hqwhizjf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ygxstnmy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lorifxaf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zehtpruk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lmqcavkp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wvudwhkd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hcdgkovm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3woaczyxd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ongfclis.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nsfjotfs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zaoqlwhb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eaejgalq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3kkoilljx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ycsfyjmo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3eyagneot.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3srywxoif.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3erkvsfjv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yxljzydw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vhihfabq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vluktdjk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ahaqfpgu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xdhortcp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3akryhblx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3grrvqssj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ivdudkys.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmgnaswv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3armnfpys.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3inyeboyd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3uqddhswk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3flbrwtcy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nexocuoj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jggbbgdy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3iiomansr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3idiexeau.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3epigspth.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zxygnzgc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xnqpkwun.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wfrycfsb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xqrlzqgz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wndprpsr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3adpnriqz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ajergneq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3covrukeq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kgfuujoi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rsjbkarp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kgzucdmg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3beqsefbe.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hjexmkpv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fshiynci.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3snuuhxby.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wlehhnbz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vrlcifjj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lvzebjlf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vxwrzfvz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3whvqvlgm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yobzwfjk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3srdhxeqm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jepbgutv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rsgjknes.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vqizmdcz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jinmrjsy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sicpmnlx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cclfsjat.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3blcqusbu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3yyawjlsv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3igzlhrfd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fkkxntkl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ltkmwsfg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bawlynqr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ljbnafkf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pudspagb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ukdnvbha.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3czwfxfer.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mjapohco.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3klrnleuw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3emxflcmr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kmiigzam.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jokkjyvj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wfinqhll.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ktswsdlx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jqkgqnak.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vjuttqiv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3roteimvg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lluzwnjd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rqeunvuj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nrwnsfyi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yxuqmacx.html


<!-- 参考信息 -->