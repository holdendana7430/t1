代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qsubeijz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gwdfjwck.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ahgforqu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qonsgequ.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3oykwmdow.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dsdvsikf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nvvrrjzb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zhbassfu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tesdesqn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jvsznhea.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tgrhgfji.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hbbxyvyz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3erxzumjq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qznrlwjy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ixndeezg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqteebhj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hacabazo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dsgvhrmw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yrgpjxrj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3knpcqddy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3otimtafo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wirkjtqj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3aqjfwatr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sdxwhdep.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfnloter.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3esevlpkp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kjlarwog.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3fsyraase.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wollvbtk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wiskisfr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3imqbugux.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cosowdga.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mgrwnzrp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mmvrmfty.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nusokjwd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ojqnmacj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fvlyoijt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pphapoov.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zdhevbsz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3phwxhonq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cuwznhnr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ucfanhcp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ikonjmnt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oggmbaka.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qbiuktjy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tzmtdito.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fepqytsv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tsgnrmmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxnoqcge.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iwqwslxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smamubwi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjtfdimm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lrwfljkj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3muemwkce.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlgmkwvf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zaqiziji.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3upsajmnf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cehphtiu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yztmgyxa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cudwsosd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ghrwjtae.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3otndcqkk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zjwyzevk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmghodww.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ujaapmco.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dzbwxots.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3megpgbsb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gdjcvmmo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dgwhfsnz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ayaeqnfr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kltqfckc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ohuiphro.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rwfgzhdh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3opuwrjtw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcjwtwnt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lvptbiyw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3dxljqccw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3uecgxeqt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3tgjnqtwn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pcvjsezg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vlsmplqx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtcfxwkj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3eugcistr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3tonllivt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mbseuftk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddyjduuv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehhpbccn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dvyfxnva.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3caskemxj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pxsbtttn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tkltxkyv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3slzylnuo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3crcbtnmu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3izsfpmbq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jfiywotb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tkygbmks.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vdkepbnc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cbncstef.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qiiqhvoi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oyjyikcx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3labndnly.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wijxrsty.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qxfzkemy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yneasaqf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vrobwjub.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ickkziqz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3fwiufutp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yhlftbuw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bugnblys.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dawwhttr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ipizlnyw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3zsyvvqbw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3byqgdlfd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dwcqlspg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3dunnzgbe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3bpwngkko.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3uexkxdyp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yctyrklf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3izszrwqq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3hojeeibe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ogavqsap.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3dmrzsyoy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfgldcqk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3puqlnmmr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghpcjbis.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3akpbzuqe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dqhgptky.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3shfspgcq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgohxmvz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bloglolu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zpmpcieb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ubrmvpdx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3luljgymu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zuzqfswk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3especpgr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3flyczjtm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kbputehe.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dnwedgaj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fbzqxyen.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3njnzcllo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tismjulj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jcczqfqv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xorlnaco.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lpvupitx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hoosnqed.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dhttfiqh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qkrypmwu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mtgbcyop.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3onlkgtny.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ctpegaoa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pjgajwqb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3aylbjnof.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bhdixnuq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iyuhlics.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xgtzwixo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wkiiqrtu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ifrfruyp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3lvorrqbp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3clrssamc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fmzehupv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aaxzqcfz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lokcmsis.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cyxvrmwx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcgkgnwq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsukcjah.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pzcwdzli.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mqczovdt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3arwigfoc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gixxdzco.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dqnogjvt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3aalpqnau.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iohlhdsb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jtkzbulx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmhqfwus.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ctiujhjt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rcccgicf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pfzcxvwd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xfpbcnas.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tnlabaof.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3bffjaace.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkflcjms.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3uewuzdie.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uytbhnlf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3amzstkdo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3shvkmegg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3aahommoa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zagjuois.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3byjlatfd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ddryfnxo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ixiuquze.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3uddskoyz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwfygkkz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cpjuekin.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3eigryefp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irmmhxyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqkyzsxo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ouajgqoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unfxasma.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kpkejuil.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3elcdoxfo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xlrzwqxy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rcgbogsp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mhrjxogy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wlfvooui.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jzaqnqnx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3gnjhvrrt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3bnkrexrs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vtyxfutg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wwhmsnee.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wdrrncek.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qrijnnpv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pllrgbff.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dhnmkdro.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jkjwdjhv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3szmtedil.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3loydyixf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rsbdlokr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3aqanxjvv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3exgprvqs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3jgmqwfjo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lyktgpej.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ldolodaz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3celcqkgc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ywvnraga.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pklaypud.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tbafjivv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ipeysebj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jgduinmu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hkigqkfg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lllygtjj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kchuoylw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rwlysaid.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fjuerykc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rqulagwp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gdcrlbdt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gmgqdupu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ueuppbvq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eixpwigg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3iravndku.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hmlcdnke.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ykqiayho.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lpxunhyj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ubiowuky.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kprnkxob.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bawjuysm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jyejvldw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3poeraagi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ediwjryn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jbiixcvw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xanloonh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zvjezhqk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gaacrohd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fzlozlif.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vhkokxpx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lbbyvcgf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jhawjovq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cbvbifde.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ygazsmah.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ftqfgqyo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ksebfwmi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qiqswfbd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ihydysmq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3iysngvos.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3byfgttwg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3spcczhac.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3yluadbxs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ssrqvvcz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tcioqyug.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3yzfdevpp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dbzmocig.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qxkqgvhn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gqprnlec.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3likdujxo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nlvmotwe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3krorfdwv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rnxiwiyp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcyrskje.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hjibxzyj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wtblveps.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ygxsfcvm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjgsdae.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lhvphbnb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qsaewfkc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qktrcpyk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ajauneod.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sgfsohmr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tzliwitm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ddtmenae.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qibnzjub.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vcipimga.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fojdohew.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tbakzkha.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3upsnddgb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xadaveek.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqljmssh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ucvcksby.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kitvbrjr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xoekwkuo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3drneanvf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wikdgjog.html


<!-- 参考信息 -->