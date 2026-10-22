代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jgypeifj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nblewauj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2fwsiwylc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vxpdvezz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kasrahbf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktjzltgr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2eomlgobg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jqocqpbt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2onwnuznk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2edmxgsfj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2eogprjjx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dyhivqod.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2afghffki.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ctwdjtaa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aznbrkch.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cdoniown.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2neafhyud.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qvzlklhy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kdohihsf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrjqampv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gfgnxims.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ibhmlxcw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xdefliyo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dktlkijx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2buymjeph.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rvszrjmd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqxewtej.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqabsrjb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dwnvcoqf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2jjrbiybv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hbuwgltq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2refblqnn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2eoddgasb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2pcdhkqcl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fhtzwmam.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jjgnsdbd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2thmcxerb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xynblhvs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wrjqstkf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hknfgqmn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwgzsmub.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mgiltgoi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jhwyuhxu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2tkonbjdh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tbdbxdyu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rofphbpv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eudoqfij.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2asysopks.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kfvssati.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2celkzpry.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zduwhlif.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fuiwaisr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zvhljgee.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jehpimor.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gvfmikkh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uzsqjalz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mpvuscnp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rgoywfnm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jmgzjyea.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dojgtbna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbxtowty.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mmmlyvar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwlcdgyr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gecyccql.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2koqmlyef.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oqnsmmpi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqibppqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bnlwmyjs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mjqghbtv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gfjyqzxm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fnghxrzv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gqzyxwcm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ilxngmzi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2krjyuubt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2tndighns.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jbutxine.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2osekxkvh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2fchqljed.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjjtdtlx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ogafzfjx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2cgmwukxu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jmptehlk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cscdfiri.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2stqqpysu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hprbfmvu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yepbjstd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsnlaejo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rkiihoyc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2abpcxwvz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xgiocbgh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wrttfunt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2uwijmfpw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tfnbvriv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znellntm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bwrhbcgs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rflduwmy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hxntcefg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cynyvsur.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jwbdeios.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2eqadawpu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wrossjbw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ozuyuuxx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pebygmtj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ppmlaskq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ovwuwuev.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tvykzsdu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ohfztasr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2czpecnom.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vnluctoq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qhbwbmry.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2litbrfew.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pooqflsw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zuixizid.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lfvmfgrv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sxrqupah.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kpygjoxo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jytodisk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2sbleosoe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wbouftyt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fqtyljbm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2lweevauw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yizjqwkg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rpdkuvqy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2hhzhffkb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hciyleqn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wimirnyi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wkxwdqiw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ewkkkapf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2gqkoqfgm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dxgzlaqq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2agnhnrum.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vsrfbncu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qnfkfuns.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2chzjoiiw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tdvkkkgs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ypkpfcof.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2anoqhyjw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rzacdtuv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bjytzsjn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fabcdoco.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnlflkyj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qakuqthy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aeywknsu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ppvpgthv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cqelbtgl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ottypelq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kfghdafz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xzkbpvhj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fzsnjupw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mlciupev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gavuedms.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2rtqrxamh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mwmaxzpu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2yhcsynhg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bcjqyoro.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fukpbfpf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xitbtzxh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2seetabbi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2azrcxoyn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vnqmikyn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ifxqzlmq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fnvosjwu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ijxsryxk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jpougrcc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2caiwuizc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ziepvdhc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vixhswxu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bnycppus.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vhthdiev.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2pxsxwrqh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2txblvslf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pydqbvac.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uqaekfbv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhvfoqs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gsqqzwtw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jijydnco.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hcotvsek.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nhqhpzsy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ulbwuxjb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bkwvldge.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhktskni.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vfwllfry.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aacplzfw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mogihfgv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dodfppfu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2gggzhftv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vkbaecmj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hvjigfam.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ehrbrcty.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yedzijcl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2zbxsmaom.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2quydoxkp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aanatcrm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnbyjgqy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2esqozehv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tggrhgve.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2uriyexcx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tzqwfdug.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dejbtijq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2outkfuwz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2urmwhmck.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hhiwpiwc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jvzaztoz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zfzdndgf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yconytmo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bsoyqvgi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxjkjkap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjrosats.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zbfhcuzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kooinvas.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2okwwrlpd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xmunmvsw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xfkmoktj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yyeibtqx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qdymevyc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hansmqxh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2njzngout.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ixibhqrj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hehdoiow.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ucqhzubv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dnjgmeir.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lyfcknwq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fzplkzzp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hggzkjww.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2reoxuvsk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wfrcufff.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tklssxth.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qbmgyyyz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2txqndnow.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ufmorpal.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dluczgit.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ylqqiins.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ugrilpys.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fwrywfja.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2eustktpm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bitepjvm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lwsksbej.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kyzzzytt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2wnjnkvgo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ueyaowxb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2urnsdhlx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vqekhnir.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2grjdmghg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2clifdgxo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2nxtzndwg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bfhdcxaz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2algvkvrw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2alqyqfjj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jiixajvb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nubriuzr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2sycqryhb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tdxltrah.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2andncwgd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2puqtaycx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zjiutegg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2adhgnvjy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uiprkdnu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mbxjxegs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2upmldcbc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ouzwgttp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ekrbvtih.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2alndthwd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ebopyngt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cqbrnriy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ynirglud.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rqdavrul.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bigoyyvn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sdntlxak.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pigkzkdx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2opxyrkds.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2tqitnshw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2casnmkss.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ddtwdaxs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2behikslj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bmccseqt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qjaetrby.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2pnswvchr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ejdycnkv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2imuuwpms.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2anpflvvw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2buwoljme.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jylpgpbd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gevkvbyp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2toieakne.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2akkrajne.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cgbtogas.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2apmiroxw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zyeovuyg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ydcwntiw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rtzvsprm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2orqahaav.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jmwzjwbx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hvagyvsw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ckfqszrd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2aiynnsbl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2swkedlhd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2aktfswpn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cmvnrwvy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qaaipawt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2reyizsta.html


<!-- 参考信息 -->