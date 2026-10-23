代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3demdrvgu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zrfkpssf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gkurzoxd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mwmtkvbm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vtedeysu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cakopxcg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vifwxhrj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3nwtqfwzf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ohzrdgwk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3abgzykzo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iaolnevn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmomvibk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3thxhyyir.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dcybumdx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3etxvlour.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3erfedaoh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3pnjyfkxj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3xfixpwpz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pofzmafo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfccrgez.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvtvubga.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rqbwsejx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3sjzfnonk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vlmerdpr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ynrjgtcr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3pknpyvxx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3lckaisxi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3duenkdow.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mprkahxn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yxuwdzty.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lbqcfufn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tobvchkg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rxyrhjnr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qvfiyksz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3mqkwdilb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3siyjwpyt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gbjrutxw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3suwgpiar.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cdgaxapq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3byqqvopu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mbwjiquu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jsmlupze.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ytxuahvm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rfrxfzkj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nbbhtrth.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3aosrxmaj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3icadhkne.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ewsbqwjp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jefriaeq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ftgvtfwu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vrxvccjs.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fsqbiavx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmeappwg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wcxttrvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxmtqjlc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqytorsn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kdkvbkxt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xenqodqo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3azsuoeup.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqevpass.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mrunkowk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zapdszcp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qdxlomqq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ffxflvnf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3grtvjefg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3nztytwno.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zfszbiqr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmkymnpo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3holvskzb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hcezuzaj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kmgdxcai.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zrmkooxe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3yxqkzajy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ugckbuue.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3gwkndyvr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvhobprx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqbbpdba.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qjmelndd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pofzorqb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ulueedti.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3shcuuipu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3rixwsvcx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3evgupfnv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3usxdgqjm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wqdjxrhg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rzngbuka.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zbhpntai.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3quaowyod.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nfgrlldw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ljhajbsm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjabazap.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ddyaumbl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3iinuvqcr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ygfrogoi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3agcgvtdw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zfpeoppk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3egnwpazc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3frxzrbzz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3syjiyimc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3aujyqoqm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ecxhtfbf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3elabedvq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iuaguqjv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ebtzwsdl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fitpsvma.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ddusqodl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ycihpefj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3aqwqyqgx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3utvtfqdk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ziermjut.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hpcomczo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bqhdmnwx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kdnlyruk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pbpqdjyq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ifnndomb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nkiibtqs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3cqhcgkux.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bkqjvdou.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3joergwgv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3isswnipr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxrnsvqb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3clszevsn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjxrthmv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yntmeknm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3aldgtohx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypsuzprp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dtflwzto.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xkqneihz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3sddhlhmg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ezzeewql.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aqrhqozz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3umofqfqe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikndkyfq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bascycpq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzyziogx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3emgctvpd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jmsfmtpf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mtayytln.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gppnfouc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hnjeigzm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3phndzbuq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rgsppxlv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uxiopjvq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hiqsfate.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fxshdlyl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fgexbiig.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vqckbceh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mhfjgybt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tonfnnfh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bqkqfoqo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dklfjdql.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wtvnjzki.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3pxmzlovk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hblcckib.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wsjucdqz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xqwzapsh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3hqeucurx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yqkbsnmc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3azninpkm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bzloufiy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ivtgjxfj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ediggadb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mbsguuxa.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pygmggix.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eqodgmoe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hzineaju.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lqzyatzg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eriripry.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3duzuxinu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cemldkfd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vdqqbagn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yvxbneql.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3difkicls.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jgaqjqnv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pyzkrgpg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fbrhxigi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuiimezg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wrstqycn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rbqhidyg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bxqjmyps.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3mmuvmnlb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3bjdsyxsg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yjfdzvak.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nrrldsnn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jpzkyfte.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lxaoxyts.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3omxlwucj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nabuhttw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3irkuvixh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ywfnukdc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bepfmyjq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jmcqejtj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jywrnumu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mashvrip.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qhencezn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3eypnljdq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kynraqcv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jjrrafzz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqlmpwfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjongozp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gwpwganp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcrtuabm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3buogxbvu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xeldoion.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eavamndg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wiysizhp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bxlknlwi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kikckhdt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mgsnofeq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3cyfytdfv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nuccmfww.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zksnivbc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3akddsnag.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3xjgemvmb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xtozmjtn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iusavarg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xyohcyju.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uhljvunb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3opliwnzq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aotzkcjg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3osycrstz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qibhpdyt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3yolgzfuq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bvetmdos.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qfrdsrjo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mwslwvqe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxrwqby.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3exeicfzb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uqfpevxm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tsrsrsei.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3thtkgilp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rdfplbjl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ckyyymuo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jwckqwgh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lfjfzbud.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lsvmifhi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3yzugjzem.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vllxmyez.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zywivmig.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zsalfgxa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jrfjvyjt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3keoaepkk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3nxcbgobg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jmzfpfzw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gymmvktv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ehfnmlyj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uzijeynd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iezkjtwr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bsvlauar.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ieckguqn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eoouaabr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ztgknpet.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pdwqccsf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ewxdtqqi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pdfqtfcx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3giltlglg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3clqhcfvg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kxxaruue.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yogtluui.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bktnwhom.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nwbxanql.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ayhdwier.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3cjdrcmxa.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ebiygkrr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ympeungr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jjmvtmmg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vwgusiay.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ryysvjji.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3upnmrywr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xveubnmf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jsmfachx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3tehnjftn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jkkdqdfd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3idxtswos.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ivoxyjat.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xwimnxhc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3prrzwgux.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3cxlodnrp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vcvpllyh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cqogigtd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dsziwzzw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jlebugjy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tkmtbhha.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3buxobnyq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kbisdbch.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tligftyl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lmlqgucm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tbmgrurj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ngturznq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hcvamvpq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tszlzxfz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vhvimmnl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3agdsdbfl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vtjbyvwa.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3upbpnjim.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zysummbe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hzlzzhqn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vpevdxff.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzviswvf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sgxroaap.html


<!-- 参考信息 -->