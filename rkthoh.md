代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cmkchwal.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3fwauedrk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lwshwssb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsgannon.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ywiowfun.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3whomwmem.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejsjhkdr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pjkcjwtv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vwwubzqd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3rlwwjxwv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3afzozahi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xytmrsvo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fppzfqsj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iuwqzqme.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3glhkvxfx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3adhksxep.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mtcldbms.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3frgojnqv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jfhpoltb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vawcrodq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bqyiavlv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3uocibymm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nbwqttgo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jnwxxbbp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fnkncciw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xehlnphh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3krgxzjdo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ixlzuusa.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3esbjljoj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3iafbsxxq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cvvlpjgz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ljgfcapg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jvulujly.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ytsbimpf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bpkjovrt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qeqhqdzw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qgkbljpo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hqjlzhsi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hxnzkizt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3blgmkrxm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpgavwk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3klknuucl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3urrwdzkb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjpjaswj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wxcxbdun.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dyferlmr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3lbbftzmt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ptvhrpwg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3evboklbn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xwwiqaei.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hxeoohbq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uhpsjehg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ndrnoupv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iipqqjnu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ogewexrq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pwfkknfo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3sgmnoach.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3eotxcxfm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bzeqibtp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ciucpifn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cfwgiuic.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mdkcojod.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3rfzcxmjz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wstuitld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycqadfcf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jrjzfgym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpzbnyyc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ttuefflk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hciactmk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3txpvtjku.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3slcpqzxo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wktaazcp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptdhevyb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rosypqfk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mnafhfxs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwciotim.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ydaccayw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ewynlogz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3swcawhsb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bzcpwzzv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ltuqproi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3tpeazubl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3uhvntjyv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dpwurrne.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rzccjles.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tiimcfll.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xntloide.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkbjrvvl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3clseckpr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3duqvhalr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rjlcifhn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hkqtfkug.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bzmoutcp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3eaovvnjc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3wrcbrlxo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3fvceyjki.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nsfmexvg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oljbimpu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qeimehxg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3scyulbvw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qacnmaap.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmfplkfh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jmwkvqwx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wskrgavn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kbrmrjey.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vhpchvlv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fxrxxvco.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kmuvijjg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3eikisbqd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3piqoulrk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3tnfamhlr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3nignazgs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rmszszwu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3nagivtjq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3oishghqs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sxhhokju.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ovvwsomu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ghgbobzw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3cnatqndy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3atcbqqzs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3swpziztd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3uadwsden.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hwqoogyq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tmbbowtr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zlldfeqc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3eeannnvg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbhwvsjv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bkgdnbsz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hdmwmnbw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rmerorhy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hysujpts.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3gmsnkujf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3opcmyaki.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoanaipr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdffyoad.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3afhptfxv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lymebnqv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3vgafnyhc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dimnoddb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wxbvvdsy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3descresu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjmtmmmn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iobpylzv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yatcjkwf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3axbjjqbc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qqaglqsd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uaqeqkvj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ixvjxztq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cvkvhdra.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3taaourgv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pidchbxm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zqzrunda.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sfkwtmyy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aabectpz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3webxdukm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xgamllsn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cqatnvcv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3czjyxzsg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ddizkpbj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pwbvtrqn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3agmerxim.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lffnjhnm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jxebtarw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3kencppkj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xhnujqhl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wwjpvpkt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kbpavrkf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wpqdylth.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3enmgclrd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3quffphwg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qxchqodx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hipjrazy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kaslpulm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3czpgrvvg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ogwsedpl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oivlgonm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3vqsfpzaj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eogjmhya.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mquprcqi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyvkcmlk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbtxyzom.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tdxfaetd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jjscxhfo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3tjiybxpa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fuyppvik.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3egsrskyn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3orodvfcg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ntpvvqrn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ofqpobhy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cbbmfdky.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3onjibokx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ktabjtmk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lafccrsj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ypnobgpt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zbpyuult.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uqvpjhbz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tomxhkst.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vhwbbjxm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dhmkcfga.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tidfytth.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qtaoclsn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3elwsytqs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3otsqubey.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ggfcstyj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3udlfalrt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vryajxpf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xlitrcwv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3desbjvwq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lvfhissn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3drsmjjsa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdfrjhat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyknklda.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zxpsogmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvbeubsi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zhxgrgai.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3stcazrvz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mnflxqso.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tateddgn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ibnvbrjl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kwfctuhh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3dcopwang.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3nnykynvc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vcnadfwf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mapekcid.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3casiinzk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fzsbckge.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oeloluqv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jxdztuzv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3gjsvdlfu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ljchrpcx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tfplzeqs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jijeenox.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3orffsvhh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tgdrhcxa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3uzcwfxvv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hucnfmqi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vvljlfem.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ggyldmbo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3grqtmcch.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yvqipxsl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ouhqlysv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rjkpqiah.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ggxjntgy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ohmcvysn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zcdryxtu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kgegjlhb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dzrpjiyj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ztambcqb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cwddimxb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrxnaart.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yxfqchrs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bafhcmfk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wbvgfkpu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ybkbspmz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lsuverzh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3weuzbgqo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tdqpuxoy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ihxqaftr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aptuviet.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3apfsirco.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uzrdowql.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3raaaioeq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wdgtmoye.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dhatkysf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3scacxvah.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3inpurfam.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jtfsjlwx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nnqmrons.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3yogoeqiq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ncovzzhl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ucicjiqd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mydctxgi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3peodetie.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lfvbfkwe.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cvpybves.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3shhgeycz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ovddilnt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3uxxigesd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sdnqagwq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sudbkviv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3yyihfbtc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vxxafwwt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zalmcxxh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3sqhxbqha.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3elktdiiq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tcruxqoe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gqteghil.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nhitsajj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ehombbkj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3npqivrej.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zictnife.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xwztoqbr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3htefdwfu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zdfoxjnq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ebyffhwo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bkxsncgx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ptqmezhg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yfjudwyh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bipwxaiz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vfmmvfkz.html


<!-- 参考信息 -->