代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2twyhdlul.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nvlhtkts.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jbsmazzo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vqzqxcie.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kximloym.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fnwkhuzm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xnkubgde.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uwoywbrr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mmpkibfu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ugrxrubi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gftctpej.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eucwyxzc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zwvwusqb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2csgkrylk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jasalkkg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jluxfliz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2tthlxtdz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hkzuegud.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bqlxyvtz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lhsnzcef.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iwfxdyzo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2omsndyke.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ixluxavg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hballqms.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2slxaooco.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rivgkqsv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wswvejna.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqmipejs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2earrpixb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jgcppfcq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rxsigihx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2csamebqn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xjzhbcwi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2srthxhit.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jycvgvsj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2trgklkxe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjbicihh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mdpjrtdl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxnufwau.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xsfjiopv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdprqben.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2buxsoxkx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2uwgplpyr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2spxtqafc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2casdmiyt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ouaesjsg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hxjqojnz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fdfamzls.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pltjwqbi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dguxhnow.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wumejvju.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2khqhwtwi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2pdvxgyor.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2omeurkgx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fmikwcxm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nqmquxur.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2igiccbdq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lysxnhpi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2thqthyaj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dsbafezy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cedvnnpf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2tmoaxokx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smqyutcg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2iltxxtii.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yishjvon.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2twirvlaa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hejrvzvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxxavasp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfwtutzh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dbglqhzg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2biwrogdj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvvofuve.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xcrpapjc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cmmyfwma.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mdbvmsmh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arpjjhce.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ogsvbhvz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2gtlkmkfi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtkxtuwp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2kuzhouza.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jjtchntf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mkdicmhw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rjermqop.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xugcdtle.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wprlqsqy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsdbkthw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2yolofngd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dmogekbn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ansfsmoc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2fwvjqsvh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ovkvqkdu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nftyohtg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tmwqjgzv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2isbukyvj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2supjakwl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2yqvezyxb.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2khzghlpp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gsoqgmex.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fustzrfh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bcsjprpk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2iuymksmq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2duelxvfv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wiccnzut.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ythcjhnz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ttehjmzt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xoseoslp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nokmvjzw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2txiddeco.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dszqdspg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gqdvcjpa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jatgvfwl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxcbgqoc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qaaueaog.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vawjzrud.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gasznthk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wucpuvob.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dsyffhoa.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dsrzinei.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2turqvqoq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2muzlgcqc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gbyuitvk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ilyxzfxu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zanetbyy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2owglusmp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jlpwdeev.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gyqvgmut.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kuzegvkb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sfjrjtop.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jcfwxtlt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nmajwqdv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoboipex.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hviuasjw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2crcrrmwl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rkuvkuvv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rcqspiud.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nhukwrfn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pznvlumu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fimlxjqz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vzgmnkof.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bmhiaoeb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywshlepb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ewwpbkju.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2drffhvqk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2acckqrrw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wizwpmci.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gyymchqv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2haxmaxxp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sbtxfobn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hedhyewr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ozrotvtc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sqwwwulm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kmgfketm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fxggeoua.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lrmyhtgu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jdaukjcv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2oqphcnrv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dgdyetca.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bzyyzbwn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2meupdfux.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ruygxtri.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mqkjvzlq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2cmiftfeh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2wirymtte.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ogacaesz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rcbsesqk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qmxbdmck.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zoczmwcx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qkmjjqfn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kiamyxgj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2rrjdifqh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ulfzzioi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gibaiujh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jaaqobrg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bnjtaeku.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nmrcbumh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qwidiaiu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xagblwzp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2muaepwjo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2sjnjhaho.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ypnkepjt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdyjsyqn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pazvetfl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pmumeinw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2saavxjwe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyqdipvb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nyzjomhj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vikohtss.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2haolyfbi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nboadsfb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2sqdmgvjm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2eqvhcuei.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2culbpaxo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2naovnlhb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dntdyzou.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2voraxthb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mjsnmvog.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zcbgsjqp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dvezyauz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mvugmvgv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tkmisfqg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hmgkhjtc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2wbyhsecd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2uigdwsxs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2znkvyura.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lwanvfrl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hguwzpwi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nghlapie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqbboxox.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fswedzic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhtcsdps.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vyvkayxg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ojrrpdhf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tjbcmwgg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pzsjymtx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2iuayohep.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tqnfbyte.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ibqamucu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2srexrmuw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tvssqlpr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2oycpdvtv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pvgoqtwa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vqvhfihe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ygvslhps.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wltrrcqs.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ylocarss.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nsmaeyyk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ixtilxks.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uhozlcwv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nwaztkhu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2iofpqbni.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2aweaaeuv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2krvuwdcd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2idymviys.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ungcosot.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wkiqqnpa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gjccgwbo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2akrapvsh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wuumpabh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpvkolfz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2unhnhqrm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tpplukgx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zovazfpe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2syldvpgq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xnlcalae.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2aisiddql.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2djmsstpz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rjhtkmxk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jmagugia.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rquxmuoi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oajxhhpf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qanrshnt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qockecdv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fxlapggg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2llsgxhhe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mfzrapxm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yyziqpaa.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mdczdvpf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zzephuwu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rrfqvsms.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cqkssvpa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2udglyjor.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sjbjkecs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kgfispag.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qiylskaq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2zvlknzdl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2prukhhhb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nhycuygx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gnxszyub.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uvrvcbdk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cshijory.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qhcfoiow.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2drdudxoz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ebpeegyb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2oipxcnrs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxzeotf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fkxkslwl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yprnkyzb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lgkrymiq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kdzdkyom.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nvzmldao.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tpevpbkw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jbcfpiim.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bcylmxfd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2punzmdtl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uocuwlbq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mrkzijkn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fiaboiyl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xlipzufw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnhvccul.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2utarrdxh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2oluqokvp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kfbtbkuu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2akwwtdgc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dsmqhddo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wjjbrztk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cynnxtsm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hydxtjnk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xannnoze.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vvxtegdn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bqfaiyqc.html


<!-- 参考信息 -->