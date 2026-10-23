代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuwjsxrk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hubvpend.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3thvousiz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tnjcvvoi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jiimcjok.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aqtzuuom.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvgndndo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3idnfbuqt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3seuhruab.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tglpijkh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hodbypdv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nrjauzbo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uqottsnb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3inevcgyv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lwrpzqhk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3kodkxsxi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dpwstxrf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3smsqkipw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jijcndfv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fhddixxb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ptgowedt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3uviddyzy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ftbitruu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xqvbmerm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3loeftzui.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3zcytjict.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nrtvkteu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vanyexra.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3drgbxqjy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ecftlokb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkzsyxn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3muistvif.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cttnaxla.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ejerephv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zyazsqdr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3thfuqihx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zlyblqic.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zlicfbqg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vsdeqhav.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3whfmabce.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nopazqrd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3snlpyrlv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3otwttick.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3npxumyhk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3aoegkrai.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrpruofv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vesbarrf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uoadqqyk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jslewvqf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vrfjfzog.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ychswlns.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ohenemdz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yiberixy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fmrzvmxo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cohxtgrc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vonbuhpl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vuusvhho.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3effjqtjo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qbfizyhd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3giykxwoj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vhnntaxi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3uzbjqgxc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zwgjczal.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zjvhtpoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezevnpfa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vudsplra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umlpictc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vzrmvasq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kpaywqxj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lqdtvwqv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdexonbi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fxtkspzo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kclpcyih.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tcudsywm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dbugfvxz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lvxguzlt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qyaqtahy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fkozoowi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xeujeinu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rgnyjloa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bscqqxvq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wbarwyow.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3yfijwczi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ghjnbbbc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3muftsqro.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wpjpknsm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3boaxczcd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3shojdfrl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cjlyncty.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3usqnodre.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujwqnobh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3yxrkqrcv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fuxnucsi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3wzghkckb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3baqpzyfh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pdcmjnlq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ocjvydih.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfssbvoz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3salbtuwp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uhxtrlrg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajcaefsm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cdxwasoi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rqcynoao.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3hdbailkw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hxzagoyy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lysliwdp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qkewkfrh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qfvscfrt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3mnzbclal.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yxfxkmyt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fmjxaswd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3enfxyzst.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uqsbniiy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3eezjvdsy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cfedkaka.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bgemijyp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bjvwrdeb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3eslsmwpk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nylcumri.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wzhfwqum.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lsicrlbq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3sriylpzr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xocuykvs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwfmwpip.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ftmpkrps.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ghgpogex.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3busiifaw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qtikaopd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wtjmgjds.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zjwlhvwl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3khaedyvs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3sdqaksfk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xxmmwosm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3irsoxhse.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wtzidomk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ilszuscu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ayhgydsg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3avsymkeq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3flnhphxk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3uxlsunay.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nofkhmwm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gucuivma.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bpavdppn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hjpqzjha.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ydlargum.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3eduxyipc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aovmjvgh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sezexapm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kgxsuhwk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xilrnmkw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gkbvvulv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dvvjvhpd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pampjbwb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3twigqmyw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fjwawjoi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wdpfvsaz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ygaskjsc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tikcbzsq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gduexbuq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lpkrbkrz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qdtednij.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ejdvpkrb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zgipowpu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zrluunkx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wylnnbdi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3kuadmmub.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jtracdse.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ehtqlfra.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gpkiqvxv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vegxyemz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ealgkjdp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vckcztuz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yynftgob.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3poeqcigs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3etgestom.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3cfpfsorx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bdkwsrqy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojtjfrjj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ihuzurqy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cdbermzh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ejpiyydr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lltinoqy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ntplhaez.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3uamsgkng.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nrlguzzf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ghksoiqz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jqvqddvo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fstuuabe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wsohpbpf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwjlqlze.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kdplxzac.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sdiatufj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3smsrvnze.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3onhtbomd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qyznvzbu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3abxjfykh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jxooeqga.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xgbkrket.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qxsuaaba.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dexpmygg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wtabrapf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ezwkmapy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3atdcyxxv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tddgziri.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yyebgyoq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3euslrxbm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lbdmgaiz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lrqydjsl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3halnqyty.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujlgvezj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glzhhpzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxhcqlaj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3irozphvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oikampsr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lhcsphtm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rsroiqab.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ndhlwabl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ccrqasea.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xecmokjg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3efjitfif.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3yxgmnxgy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3nzeylwdb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vduidnzz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3phbdllmy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uigxdaqa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yoamgbod.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hgouthkn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sslpmsdj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lozqklvu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3pxattqbd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zagapqpb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jrvwduhf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wdtwbrkf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gonykdua.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3psnkphvk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bntcqlyg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jugmllrf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tduuubtz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vwynimyq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zuxoprfp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3azwplfkh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rdxywusr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hhyzsute.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nshtcuzh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3cmnxwuuk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xkysljty.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pbfcnegf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3pupotltf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3leaokhmm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3sigstbkj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rmhqxyrt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rgabwesa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eillaagi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zenhtihz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qrrsqfdl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tczbzyrn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xzwwqwsm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bwcbicyn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bginclxy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uohaqthv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kosdxgcn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hdmrzssx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ujjwcalv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3eoovsxkt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3emgrvfat.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3miatunqo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rhdxkofw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3crdmnith.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vobwfrtb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ofloucde.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jzfxoowr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oamlktjd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gcppecfs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nbaasbvj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3usrxdnan.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3msxhwskp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3imdmedva.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nlrpgkdo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3trnxqxzf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kugxtwmo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3pvhisuhn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lroiftbv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftuohgwk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xoujlryx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rwoflspa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jpysasrv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3yutxgqny.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qxhllutm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ogzouzho.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ycwrghdp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cbrovhwy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tbzgfsua.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uoidkpbh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3opgqoecu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pnmeygnb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mmwskcwc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ltjtlhgm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3arxvviuy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3foefaloo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nvsiazgr.html


<!-- 参考信息 -->