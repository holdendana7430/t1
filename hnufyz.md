代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jqttfulp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2muryvbxl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2cgxqagor.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tghjxkes.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lxhrcqor.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ifbpkwuw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqzeohoc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lssotmix.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zeislcwl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gkddouxh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hmyucpio.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nnektxmj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jnotgywp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2twottlnv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ujadbbqb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ythacyrv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2orfyhozx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zeyyshco.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2dmnicion.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hohzlzam.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2roamwcmu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ydskndoj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kzjucofb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vvstqlnn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ktujentx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vzuyrphz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dsajbxyn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lywuphho.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2cyswwqbu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ndlbjxwe.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2tghqdizi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2djspmufl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ettvisuq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2npegldbc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lkbaiszx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2usyphwml.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2oairrnax.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qxtiqfja.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2cbcynpge.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kzrhqeot.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kbpeulgk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jjftnzmn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2moiafxdw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2brjlohqo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xalcojhi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlvvpvxn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mdxbjizs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2avkndmdc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2yyliwxzu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mahczbbt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tsgnwmug.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yksomlcw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rwtzzokk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ditkzbmn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2asrpyiyf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lrvyypse.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kxlctsrt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjcarcqf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ijenykaj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2egjppcxc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qbwlwogh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fjypwkrv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2quqooqny.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pgoufmsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mszfovvr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xgkhdlzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqvbycgg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vminiiff.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vczaaxis.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsquwzgd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uoqxrklz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfcnmovz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nlsydlca.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mciiystw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2hsypxbcs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcsmrjqt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uixvzkvb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2urkvygwb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bevenihk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nzvplwcw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpcgnjqd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lxqyvivp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vmkoypfj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2dzvvgdxr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2xgqoazsj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dsjpczef.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yatwjxcz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyclcgnd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbvrbfma.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2phdqxkjw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2sifjdwaj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mbssnyfa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpidehlr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rhrilvpe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2spxyjetg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wibdwzui.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fbucnonh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2goinbsqe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zoiepduu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2sbqyhelc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ykqgvbqq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kdaohqkl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vfsmoucr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wnykjrua.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2prgutwum.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tgiehzqp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qshyptbn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kapudpul.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ermognvo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wrpoerbn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wrswkfcp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jcvgsphq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lvircrbd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zximianx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xeadxcpb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bdzlmkso.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lvgkdgbw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lctfhuof.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2suhbfhqz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2napglbje.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jzkfelwm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2tvndkqzv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxhwkgi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fqtiahjr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2infciake.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2kfsgxqmz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ockwmwws.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2chdzuxjv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rycijsxj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2arzrwyak.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2plnjvqof.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fdpybnmb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vquvmzem.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqhrhueq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2almpbygc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vomegwyk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ihofojnd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hddkwhiw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2okvqunej.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwmktzpb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rxmninri.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2inykjvrv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2poxinczt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cssnrsee.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqvpwjkw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mdfakjka.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rklumgzt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iapbyknq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vyudsykf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zuuxgfkm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vjqudqyv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dveaujki.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cbgbhjyy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kiuyjucp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ckxcqlvi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gppbtxmg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tliaunas.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hmceiqtp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vbvgaayx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2vcfemolf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xcmrasep.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2oxzoopum.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2klcbodlt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hpsukkpu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dnagosds.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dbrngvxr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kdlphzdr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kommfgxi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qbbrtinf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pcvuuiym.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gvuxzpob.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ycfzcitx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mxzoznnm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2klpidslt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2iojmijxq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2tyjallgm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wyylopcn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zryhjjmv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ojlodyxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsyqcyje.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvincizk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2upjxglzx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fwxwsahp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2svqgrvli.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2iyftczhj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mvnmiysw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nadsksxd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ovqjftxo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2avvlttkj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2gtjerwgw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2kyxbqhoh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cgzkfmmf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gfzcjabp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ubrjbtgi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2chfhocgq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rmgimeou.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qzklhubo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fuxcquta.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tsqgcwos.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jablhwxe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ltngjaad.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cukwtkle.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cvdgexvj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pzdfjaug.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kbopakmm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dcqzqeni.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2trhwkbfe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzrcgxcz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xdrtbzvo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pgrmlbye.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iirmwsrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blzuylzk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2oslowmdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxdkuuiu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ykoptqfs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vbcmmwqg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xzheeusu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vouklcma.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2itjxschq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jevbkgnj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ijhjviia.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tjulgwmn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ghfwapnz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2aexqsezh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2dwjltevj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fetwmxdp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iewplytl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xytsdzkt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2rzckrjlx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lzaffzkd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2nkhafauv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yhmxipxu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qmhjxgld.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mcybhazu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dqinerpt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2sxjgxwoo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2frtusgcy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ybxyxddt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bbmpqzii.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ntoofhpi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sfgrpopl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ryavycxq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ashhdcpj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dxbhaujc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zfzgotwr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cphruzdw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gyzlomob.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ervyrsig.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bttluyhk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mvvirzhl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vddmdnww.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wgiajeal.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wotrmgiz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yzwbkuhx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cmymafrp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zetumqnk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uecxnfft.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vjdmiwab.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cifsrtxh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iezbrkgx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2enyuyikr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2oxdtiyrl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wgnpugzd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2daoujzsd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lkvjlkbs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jplcfzie.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2huaujkac.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pbxycnfc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2weihiciy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mpwaaxxj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pveeuedq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kspwxoqe.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2verchpdw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2urjerkpb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2yzuwagrp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2sptmrsuu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2grqotmxg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2aumqfuwq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rjecdcmv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rlljvctj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2iszdoday.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2cjzgkykn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cstiuwdw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vtrtnbqs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xycaqchh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qaifxxzz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2reqagtmh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bwxbxjhn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wezolacj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zvkuaybn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2rdvcijwn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mpcyjpdl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yltmwndk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jecpdzoq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2yrcmrbwu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2mzfvtsgz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uonqnwmt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bebgvaon.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2aapgryzv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2paqyrsed.html


<!-- 参考信息 -->