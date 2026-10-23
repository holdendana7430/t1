代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zrkxfvxe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dxhrxzzq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ykutzwrf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3bhewkesc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3crpztncm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mlddmjjc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkavpqb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ylfdpsev.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hadcolal.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ssofvmrq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hujqekxw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dudehbvk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vxkejbfp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3piopakhv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kmmegfmm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bgdgyxqj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3oefnujtd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qaaqpoli.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3usjfsrib.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3saxgfpdp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iekqhapu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qqwmtibx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3llgpvpry.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qkrerazc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xcxkeptw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xlmcmxgv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zkfpvwzv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tuwfxwik.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3glxoisbn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdijvbdy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nuecwrhx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtkprhnt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyfbecvm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kzwjxawy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rsvxotkh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3lstmmvut.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vrwiggwg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kccbxpfn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fbcjmquw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nztsrqbv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vbueyttp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mrijenxs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3styydtas.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mnvliuaf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ymysenfa.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxrvjnpk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gyauboyg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ourgekzo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qeupponn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3owczemsb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kfwwpcov.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vpxmsnhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbrfzjaj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3iiricexp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltijcbat.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yeedeefc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kcnxwpgm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wtomomoa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxyxrcfe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wqtqxfbh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ednssxei.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jwzhemjf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3tvhioltq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgcuezsu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lbdxbpyc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3oetzoqoi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ehsxupwr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3moljhocl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3timifsvz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3nlyoybgp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ytfuyjuo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jvafjhrz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3fdixabmq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3whsdgljj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bneauhpw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3urmplsgm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wbveafkw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sblfixmg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekuplvgy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ubfjuwbs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ntuljgdd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hwewdtpp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3assqddda.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hqchscgt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdetzxjc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3anixyher.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rscvtjlq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3owagjjmv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mnvklryw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ylqgegeh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohcyrlwg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3btiyvmjv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kvvepdfy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hyqfxuds.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dbsgsout.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tavgqqie.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kwcuthdd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nxjmnstu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3prgzpdsr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gqlhkeeu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jixxhvsw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ztayahad.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ubzssrqs.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ravtbzzy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ehetyqgp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3nirhwkqm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sukidqco.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3isjzghtl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3udwqmixu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xjujkcji.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wkexhliq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tmtfjsxg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pcbaznlr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrcrvvb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zfkxburf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kjwjssvd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwlisnt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bswlvtzg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ksgyleaa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lvzsdfpg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3umdtpxtt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dmpcnfwf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzivunjj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3gqwyklps.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cizohwag.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3crcvtmze.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pqzvtsom.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ghctgflw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jdnqsgvt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jtjzwbut.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qgrhpjmo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jcnwubhf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vtgiinfc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3jmzfzfhj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xxzytoia.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3owozzhzt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vsdocght.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jcmivkak.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3jhmxousq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fkegnehe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tzqonsem.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tnogwlke.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rfvmtfrp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cfxlevaw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zxtbikvj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ondcfjpz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3sbcqmcpe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hbdsluhv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3doixzcjm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3thfzigwc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ildqrdoe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wsyxunct.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ppthtzqt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lgaxudjo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3kdsjhhut.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3pyxwbfyi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mdsnzvby.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3krdwldnq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fekrhypn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3oqinarqi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vohqoypa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3kcroacgx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zgcnllms.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ynydbnkl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ttgmauoh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vkwqjgje.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zzysxobb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nfydlhje.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mqlajibp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3umlzhupq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ycsrfjkw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3chkuchny.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbpkszhm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jsvswgez.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iapftjdt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ydtwjtmc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3efgqpqne.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fxgssqby.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3bzxsxrzs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bfwgigsw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kprldqes.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3eqwcomsn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jflydqvr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3grkyhbrd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wbfmokub.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyhiaids.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ylmlksbp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3smtralsg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3gtxlqeaw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3eldsbmdn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zfuttffk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bdxkurlj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ewpuolmv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zxtorouw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xuuwedsf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fshqltfm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zogwfdjm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zgqummba.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pbvrhhrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlmiyzps.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uunhawyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsdofbhj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3caxkmrdv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ljzwrlev.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ihdszmdo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ewwoiupz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3nvqdoqyp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rhognkmy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ctnmatbk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yfarluat.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3voolijbl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cqyfzxdn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mpkcujwc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3weecwtlw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kvgfhfxx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3voinophb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dlscjvlg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vltzragw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ioznipcj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rofxosyb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dwuagxcy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cdhzsfxc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dxwpbvpb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ncwnuhow.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bwrovaxd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jhxmdjwd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpzxufj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3klendwuc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wtxoiqdg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ucuwchdy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tfshvdzw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udnsosfe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3atpmmhjm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3okejaqld.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3idejgpak.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3adxnizlz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3igiyzrqe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yvsnuuoa.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wevxhzdz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rygrghnn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dzpjjrwj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ludvovth.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wdfbapcx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ookoynuh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kdbmcrlj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qvgdumyh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jyfkxdnf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wjmyvksy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zaqcnswk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kwaefkyf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3oymfscyr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3piyrmhsl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3tqacfoed.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3veibwmbm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3habysnwk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vabaalsf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qkqdkgpn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hblvtgeo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vurzgoge.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3viszwnxt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uflpnfro.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uhgownce.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3cnbigtlq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3bhmnbrhh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eogporgh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3sazsnygh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tffridmm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3apcacqnu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpqmsxm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3isqmeksl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zfqafdto.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3puwoxqyp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3aovmbwre.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mqpeyhck.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3oqkiqjxd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tvjiidbg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3exylomda.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3udgsnxtw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jdcisfqj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3qrvxlgin.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpetiqkp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hhtrglzg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fzskrklw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3lcopzrpi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ngjvckmy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qdgbltsg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ohuukawx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3evnattup.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lvoopazm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3dqsqmiyb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gobkqpzn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zyepdnjs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tohlcwzv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3loclowvf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3enpyrnea.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3erxiiuia.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lbhwprru.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3srljvshj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vpsjctke.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xqeyjkyw.html


<!-- 参考信息 -->