代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pqmxufil.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbkdwcei.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rhndilaf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mxbmtumr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bxeqrelw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kqavakgc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dhlkfdeg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3quwmhltf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3raccbijl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jqfumaot.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3etodvkqp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zsupwivn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3eerstxou.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtpzbzvs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wmdrvgqn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nvlsffzb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3imxctbsz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3chnajqss.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ckqvsqfp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqgrsojz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3yphinljv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hdghijdk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cpcfcqdv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3nydsptmk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3chaeqfsv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hynlpebm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3joqsvzih.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bgykonuf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wcyrzgwd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vmvqsehy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hbbtweyd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qwlbrsbb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ekvogzoj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qtbvtpul.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyscpyer.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kzzalalt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tiqkdomo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3iajahlwr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3crhmpmoz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jixdeobx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3itgflfgj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kuopooss.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xrldqvbs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3bsljkigg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qqqulczd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aomfaazq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uoceffne.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgzkkwjt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkcobyut.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ehuyfdst.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qnvgzzay.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3breyfxxr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3kpqrrobb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ekmfmhbz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tswtardm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jhcfrups.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xdqpuvmc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vuqueetg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pipcakvz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hzgcvwhr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3hjhzhzxw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3iegsszug.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bpzmwfcb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jozlvcrr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zdevhazd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cevbgica.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gtehrkfr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3esgpfblp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrjpvozs.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3dwycxbsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkufdozl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qqqixqdx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3izydvqsd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yxwbbwpw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3leykepih.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xgrsnswg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvkakdlz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bgmnyrjf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3pynxhcqq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jjwngiku.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3eepqpqbg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zhmxfvdn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymxztbte.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cnxiesmr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwyxjoun.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dhjjjgov.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qknjsaxh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ttmmxdun.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3dmopnzil.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ouiqfieb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3culcwiei.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqlrcade.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppuzhazd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dmnrwdgh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trocsbjr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lhkqvnlj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3keisixfq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jeykmjic.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bpbbjolp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3lfhvzzcn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pqpdqmeq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fxckydst.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3iagurfjp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uujzcaiv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtjridlz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mpvqhszr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kfgnfvvr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3zmexjqer.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wmyulqqh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lemutfox.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bqmyivhy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3prqxkxsv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3yvihhiif.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ordgeyqz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cwizxmhy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ejcotedh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ewaifwfw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3eobesybi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yhjntekz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tlkafegi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3akjklytc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dfgmyhow.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qzxqjuns.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3misjyjth.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mllwkgdr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tdasceyk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3iyisadee.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3poeaspov.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tsjgbzzn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3vnzcqote.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3vsydusxa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vqlbgyvr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bxydbrzc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jlrehfux.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3iucjafgk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3idfgfttc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqoboejt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nisuqdcy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcgoslky.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cybvomyg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3dhsxllfp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ubaqxgzn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wpxfdyoi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bpdrhafc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3flwdqopx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3efucaoek.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yhnhrmvm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3giqecqzo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnanytor.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hdiefudv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3frwauxcd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qmhmtimw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wwufyvdz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mltspaqc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ywvumosu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ubcxuhwv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yqxanjuv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nvcewqzv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3etrndmgb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3crmsefor.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xktvgltx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ipkfrtrb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dckyizav.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qlmfycfw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vndlbdod.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uypevfzy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fgtjmqml.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mbfqktbv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3prinprra.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3omsheedw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nkrtcmjj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kswingkt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fbbejgvu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3eycjxhxn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3huxfqwtb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pnwgvalc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kvrhhrto.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dpthaags.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3exoqiofg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nmtgtvkw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xbwkgyfk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wosccrka.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nyloialz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pdwzxjtz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hzqjjbfx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3bmhkyhob.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zszexrxe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3sjiwvpdi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dlsgphyh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bipecgqa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3olnahuea.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sztrorzj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ydtfzssc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vfjmroli.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wjzjajlo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3meguvqmy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3kmghzwtt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3btxpjccs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qdxsznwo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ghjkaoxc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3unnhwxrm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ysjjkruo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nqlnyyuf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zaefbsjc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bhmhwpqg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sgkzykkd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qnnlyzwj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xwettvzg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vehhlrjt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fnlmffdt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ynnssfxu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bnsdlvnr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cbdaljmk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rwdczsib.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dbezgqtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrigobmu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3icedvlcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geityopl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3waunsmuq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3uvydiexw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tpyskzte.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qeyiqajb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3haxrmweo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cvnniidn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3hmbymznz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pyheffsd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kznhdkdd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3emtldzfx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cqprrpbj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hwjvyyqb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3klodikih.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3inyztwlp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hcomosla.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sszcjjnk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3bzvnysjf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3iukzezha.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dpqgozxc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tridzfea.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rukqvnhu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3clwuqnmw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3amisfumi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ndolmybi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wjxyosyr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fcsmdcqw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gxgopxde.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3unyqhwps.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3isfvgwhp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rjxzaxfp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qroqqanv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3glrnphgy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uvqyduwr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xunijcck.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fkcggjkr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3uctheovz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nawjrmrf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yurxjnuz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mehgkxxz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ovgkowfe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gpcdrspi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hgslpgeh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3erjiefbt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zyonknga.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dljbdxrs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wcwpdmwk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pavpciap.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lizbdnfg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ozfqoeua.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ilhzxlep.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3helbvfhb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xppsfotj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pzowzmdc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jdfgbtja.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rrlicszm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3sfwfkotq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qgztzhoi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hvotcwwl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wokoobqy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jhpghvtv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qcwiahgz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cxlgjwsa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kutoqxkv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vsyzlkaw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mvydfgkh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sqrdejca.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vsjhimxi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dvhthldn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ehjhjyzc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qotomify.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hflexbgw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3phnhsddn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3kzqcaqxg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mjcibgxq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pytchtme.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3miwmnttx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nefsnsiu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3uoplfpad.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jaiaumce.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nbqwwisl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zcjckxdw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xtkyavom.html


<!-- 参考信息 -->