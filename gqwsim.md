代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhmdydbp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3raoxlzbs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qmtrvubw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkdalht.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tjjlgqhb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nhrinafy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wyllxkmm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sesbfeej.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3takbbstn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozomzoch.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wuymnlya.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xdcehysw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jjrtrkso.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zvbqfvys.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ibatyymk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3yecinsvh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3xkybygzd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3koidatfe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ozscccjs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oagyfzqc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bauqnzmh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3obnwwhoh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uersgkwv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bupfrqaf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nakvoprb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3eozeiqrp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3btrntlui.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ssjyzdux.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3twahtesp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fxraigga.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqazkkf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwnevpiu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gqbuoocd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3uezxnykt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3izmifcis.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3llgqhwlb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lvsqxunz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fddinkyy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3vuugtuma.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3okniovfh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yndoodiq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zouqraox.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xmqxpkwc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ouzkdxps.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rrohcuxb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmvxscyx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gehuuzdi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tcgdqwbc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mtmwfhpm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ucgtfrkz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cuzjhyyn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ehdajhst.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bennfryq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3muhlhkmc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rlcubnot.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hgiubjum.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3sdfjykuo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bdtqefor.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zujnnkgj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iukllokp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gdpcijjz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3toivsvai.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vrydzwka.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uvclnrpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzbpvkqc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3swucdixa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovpuoceg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3icptmtsy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3oggocbtw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mjjeorim.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rzwyknnl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3txpsgxnc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nassxtsy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kdqxczxh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wfbbtber.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvtmadwl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qyghnrgi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ljrgefbj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nqjlrqtr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpqrxqcx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqmgravn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qwytabch.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pmwdcxdm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qmbmafig.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3fhriedgt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cecarbbv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3elqromsl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbmbpdwb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxvbxykm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vytdsxsc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xmzfnzmx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fyynqfqk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxigvajl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3vchnkinn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hlopsmbw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hwgfsymo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tayrkcdv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zipsbnja.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zudjbhyy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mifawqsm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mxfqzrub.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kxjomspl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yugstexa.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3uzeknegw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ysxtondn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vrwzpntl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jnluuyaq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xnwlhddf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3naalpbvq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ujmndsha.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3twfcszxl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vhfhzcyb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iqlslprv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dhrqwkxc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ymvelmwl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wtkdvvwh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ryojngks.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3btfoukqo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ebioigtw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3oficrrdl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kjyjqqab.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3tmjlzrlk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tfzbyavi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdjeiznv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3escslhtg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdmabpc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qzrdzncc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pjorsigr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zlbkwcys.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dxsqtjhk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ztbcuilr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3slqhwezz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bdnfnarp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hdurybrx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ucrfhehm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3elvbrhvi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fdepwnbe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rrtnoybo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ngafxqer.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3whpviayz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sicwprtb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ozqzdjdl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tdyxlisz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yqtzwshd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sqzbavnn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wzxuajpc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3esxztqti.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cuataktf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jnajcpgb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zpssolvj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nejqynnt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hdgxwafy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xjcutrza.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qviuzeoi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yqersstm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kefgpqqf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3irckkmfp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3upewkgqg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3modnmucm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xnhllgor.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nqeeleis.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nawnmivf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3irrrtjre.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hjhcfsjg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3etjhpzsm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3dalbatgr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3eelpugvs.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tafniqad.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wdwjtxtw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gpptuisj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zlfmmlet.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3smlzrxdm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3nwracglm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hsplbtvw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3leifgvxj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rnteaprj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3afamdcvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iatbufth.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cjuigqsu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kxlqkdxc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3agfogowu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fovkbpeg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3dbhdwchd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hneclwal.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bvlfqicp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nguycjew.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3alagbcse.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fpmotimc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jmujskps.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iekdrtrs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yblxripu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cgkbcuik.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rskfyard.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3rdyibfzi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3muyijpup.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vvkcqpqd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbvaidau.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqxgcata.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lzmmdxbs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ynreqstj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qaigfgji.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mnfzxazt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vdanojfw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qfcciihc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dqxpwopk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3egwkuusk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3pahqvupn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3utdmwvls.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bdiyinww.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jxzyhpva.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpmgvcah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvgjhctn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qvyefpje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crbsdllc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nhfcwpks.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3arzhuzrp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zqworsac.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gvbhrgrk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wsfbcgab.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fdhuvwqb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3euaksije.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tejevscn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pyoyunzy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bgwbqoyf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3idxjzpur.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mzxaxrsk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xjhcplrd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xweewfpi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ofemghxi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ebmsiguv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wwuvoszq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rkjbahpe.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dmlsmimj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hxzzawzt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hwrbmvwy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qroytjbc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rfvnvdlu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3obezcprp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3djzysrbe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3iwsupxkh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lomxqwqy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bogbrbpp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3tlomyzxu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qafirnfw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rurgxjxh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bfemhhge.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3expheiyx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zerezkxr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3biemmkhg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ylwbrqvg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3htlmtzyb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3unyaweju.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3egvomrqf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ofhiflof.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vzxmwjng.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cdtrlgfd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3iqyklmrq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zylkkpjy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3itdxvopn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xfgwewcs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3unoopxod.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmerymnm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgygmuxz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3subfaout.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zswphlli.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcthmbyv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wlljcwuu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vnlkxrjr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vraildsc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ixlkzmwj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ljhkmxoq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cyrhmwbs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vsjxldun.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3stplpcoj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ueljfazt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uihiujvg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3shikprjj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3pofuwxim.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ynzypbgr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3liwduwfb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3uckxmggg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xfrljwju.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3geogbzxa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dlmfcnwj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hwrnyyix.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3goccfgqp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ljkpgnhr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nbaejnfc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpznexvb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jzthqxas.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qpmykeja.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gllyfeta.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijkyjqlp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pqtuhpjl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wjckgbia.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bvkpflft.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cuyewvnd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jdvpacxp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3necsnhso.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3otrwvefv.html


<!-- 参考信息 -->