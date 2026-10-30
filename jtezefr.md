代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gzvnegpgi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gnfjfwheg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gypfcqikd.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gxykhrccx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gpjpgxsgu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gtqkaftmd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/giimcrmqn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gprgtkmgq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gkopktenn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gevbkikzz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gkpxbfsfv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/grxiuaehf.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gmmxmsbcy.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gcrzoptfa.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gbgwcbmjw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/guhwgdztu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gvgtkosge.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gafpftopz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gleiwlizv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gjyghdfsw.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gtzhcympb.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/giqfylqil.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gbqvgtdjp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/ggqsqjhib.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gprnxmxnt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/guubiywbw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/guaanbvbz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gxzqnakkm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkcssdycs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ghhmcktgj.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gvloiqybf.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gpoxinxvm.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gwybtiewh.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gapdwlvem.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ghjncjvou.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gslupkggm.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ggzrvlgze.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gacshtnmo.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gmteezfbw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gyzqbmhta.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gdsodczth.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/ghkmstlxm.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gcfyoedfc.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gmmitpncf.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gfonvyryn.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gboqjxbrg.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/grhuupojt.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gawfsadyr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpbzkqvbw.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gwaecdczl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbsmfygly.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/glqpgzwjw.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gycobqwwp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gdptkfhan.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gfpvdeclb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnxkgvujy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/glkpxqhuc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gwuizclru.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/glvhuuizr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gmdzhxuwc.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gbfihpcui.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gmdmvjidt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gsmgccrcd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gydgezqbf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gdgbtxcqi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gqibjxygm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdwsmgruq.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gcduxjshg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gfgukhlvu.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gewyldjyp.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gqzykptlb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/ggsywrgrk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/ggjllyuhm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gicvehcfz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyjazgfel.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gpfyxojye.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gunrvobmn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gnyqxylgz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gtupslctl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gvlzpmkcr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gqbrsgcij.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gqapihgdk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gtmipyufl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gxfecawwf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gqufrqscm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/ginzetrwb.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gtsqkpamp.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gpkdolcad.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gjqklisbx.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gfiznhjqd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gzqpdbljy.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gawdujjkh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gqntnlypo.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gyzskfvrz.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gefyzucxw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gzwfhkajk.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gkrxradla.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/ghzvhelvs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/ghdkqnqch.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gberatioh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gwzaxzmru.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gqikutshg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gmygewaxu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gqurtowna.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gynxxmnse.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gchdysljk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/ggvjjmkth.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gioeqqbcn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gnmkmtarz.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gaxrrtvre.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gonohxyjt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gagvsnqes.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/goqtzwqqc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gwtyjedkp.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gfiaxrczq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/griamyniu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gcrgpxzof.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/glebqsdma.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/grtgblqpg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/ghhvvaeon.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/ggzwqshrw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gjjqkylbu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gxuoimqed.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gupeissam.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gvbnhwxja.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/ghrpnoizo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gnltoymyu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gwdublouu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gluabndil.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/geatfvncw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gnujlcyyz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gyckcniie.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjnfsjzjc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/giqnsfpnb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/guzrvckka.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gmscpjian.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gszxjnmxf.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/goyptfaql.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gicssufuv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gqrozkyji.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gwqxdrrjw.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gwjcpkayb.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gcqkvmazi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/ghmgzlcya.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/ggnbpbnaa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gceruybre.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gdvczzppt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gevaydxnj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gfyegwfvr.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gonpzwxke.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gyfxiycyn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gselisbeq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gtivjykxx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/grpolugcp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gnlhscqiu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/glozpcqie.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gemsamxut.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/glifbdutp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gsknpljnk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gsnagntnc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gonqnhwsd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gajfevadc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/getwhksmd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtrivrtmr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gqebkktwv.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gqptyyfhp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gcofhwciv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/ggrfouptd.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gcywwdoek.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/ggrinwadt.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gwfquppeg.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/ghaxzumxo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gfvylzoum.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gnkewqgjq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gxjqfypxz.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gtropnovp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gojymzshq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gtjqvfpbn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gidwvxdmd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gjcgqjedv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gyjudakzl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/guvglumym.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/ggzmiqaaq.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gqqvxyxct.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gwpxhigso.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/golppcvpu.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gfmfdzxln.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/govgucbrs.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gpogyzczj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gmmqrusqn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gzkcplucm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gtabrmvin.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gaoizpzhw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gvflwvpnk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gkrjrkheq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdikkbzwl.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/ghduqyxgb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmvdfainz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gumxiqsgr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gtgqpqrck.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gcxenrrpx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gcgmuyeks.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gdxykgkzs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gmgjxmkne.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gafrdizpr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gxnkwwmxt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/glqpvdvvg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/geumydxbm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gagwepltq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gwlzyqzwj.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gtkliyuwg.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/grjomvhsp.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gakhucimk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gaogdvnjr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gwbakkwfy.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gdiuzowsb.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gxxdboujm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gelqxzahg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gadhuqjbk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gkwdvfiyv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/garzihnze.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gdnmqrcmm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gzcovogdm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gczjdqvoa.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gtawqbrlq.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gvwzyuvcv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gaseqctwb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/grjjdrcny.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbcsyji.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gchvpbicg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gtqelobzw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gojvffqvb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gfjnmajfo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gdgzbqfjr.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/guiilhntu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gemhzmvhy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gmquxpulb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gtutxoxip.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gkdwaaeqh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gutubheah.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzpuzpmlc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gzheacriy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gjbzzkpoe.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gnrudqupj.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxcsjhsuo.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gjcjlzxyq.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gqgkwdklx.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gxxavgwvr.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gjttgcgnp.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gdzrqznji.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gzzumoytl.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/glnkpokhq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/ggkarkygy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/glzviixsr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gopeyposr.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gelyxepgl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gdqwxdqzn.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gncmtnlzw.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gmlpsbvgd.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gzopslrwu.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/goycyjnmx.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/ghdmojtiy.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gmaeazxky.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gblhqmqil.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gbdonauei.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/giqetiyxp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gkccowmhx.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gizzzkftv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gxcjmlxya.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gbugwzhop.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gukkpskcp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gljpnweqi.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gkzojbanc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/ginjpsalh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/giqfkmzpg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/glgpzyiow.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gtubchwwa.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/grumxxgrk.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gsohrhone.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gsoabupgu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gqcqnltqa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gwnjcqjdo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gnrqdeyhz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gjjgyyqaa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gtnvzqsqf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gdlsypabw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/grihpfvoh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/ggmcihsny.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gxjqlpsqr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gwzvozcwa.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gbtnkcplu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gdnoefyho.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gmuewdjfa.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gxulcnxti.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guxgvcphk.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gmddxwbuu.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/godrdeaih.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/glypdbxuu.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gktouvadv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gulihygxc.sHtML


<!-- 参考信息 -->