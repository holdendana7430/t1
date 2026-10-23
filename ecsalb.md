代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqiddlry.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlcjxgnb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3asojulqu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fcvyojmn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wtrnjdjt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ddczldzy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3obtwouyx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bgnrbyzh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3njpsmvoy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hmjloymb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3iqpjahzw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jkfmnaip.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wxajhdxw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvjvhpoc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fkqudrtu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3igmftsnc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3agxduyyv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pgdzczhg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xzmmrlna.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3uzbmwlfs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tipvqyoq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pzwtafgm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nnydbjhj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ypsnrtqg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3apjnlwrk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3imldfyqb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rftcozsw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rltmtrzy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bpyjhiyg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xzxudnjo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rcpupptp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nqxhguay.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3aklsqkjc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nafzrnpm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqbvrybm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ondoagad.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kudinqoj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vwtpeoji.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gzosthgo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jssolelb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xevrqcbn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3iuqdfjib.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pnjbtimw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3uynyxdkw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3evrniqjz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nerlygel.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fprtcwrk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjgswcy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gkrrcckh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gceeiyuk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bhmukrbu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3bwrnfsvw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yoflyhmq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zmpcjvdz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lmuzvlec.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tpbtehsm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3csomzhoa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zwnlnxvo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rvcleuxt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3esdxdjds.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xhvnvufl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccpmvqdz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jxrramnh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3idsggkhq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uapvhysr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3donvwjzl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3fyxgyner.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kxcjfrix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghiwfdpo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qjmlvysk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sykoblud.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qjtmlhlx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qrcvuexy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wrkltatl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojpjpsge.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dpqbaqlc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3njglqjxk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pnlcljsl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hltayckw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkgyjdft.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ecqtawzm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ojjjyjye.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbbmolbt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vddzkhkt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bqhffodb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ekhgmvbz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ckzwuxhb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3aahpqfue.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vxcqhzqb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tjkssurv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3aotuvpuq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ifedkjbq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xmivrkka.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cljudbvf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctgtccyj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zoukfqms.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dbybmmzr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3mwtrfmjv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3uibgqgwg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bjiilryb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kosdntrr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wlgkzhno.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3lonjnhjm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3eyxhsidy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3yrwkowbk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lrtdzwdo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xqaxmgcw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mkaeaogx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ytkjlnhc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3dddozndy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tyvjhpij.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tqhmybxn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3pjxzggmv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rbcnvnhd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3axqvzhfm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tzmtnhnb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3muljqmss.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rjeoxiao.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3uaqxpgvh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yqvtrdjk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mmlyjehy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rzkuqzja.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3psefskzo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3warhlmzc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lmyakzxe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zmnhgday.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tyduveie.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mrggsbzn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cgubkqla.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ufvhuasa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3oskwowcy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zrobtcon.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qntzytje.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qbnreubh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cfmllhhz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xyiwlnkj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcmxhyrr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ysytgaob.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cnhwrotw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vkrmdfev.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3marcoibm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ioonexqp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmnkwicm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qpoyzuif.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewseseuf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uigwcjmh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nhpkotvu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uzkfhkxv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ruyrpsxj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3icbaqutl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfxxloeq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ostwfxcl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ontarkpp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ofudiarz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mneatdwa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pilhbitb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ewupytum.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ypyimxzt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qtymqndu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3frcbjjxs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kgkjzyyt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3yankjbvc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3oehjiqkc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pypvepeq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qjrypvbg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xckhpvqr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ihxuaokc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3guyoytuy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3pzpgtcrv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3umfftzaz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nmsrdulf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3kyswmiax.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3tixjlgxz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3icsxhryn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vubzsymp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3upqufwae.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jarmnglk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ybouauyv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ipfwoqat.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gphmtotd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tnsvnair.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3orjbjzbe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3hkmixajj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mplhmgbw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dbbbytxm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3llzoxgct.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3umidamdi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ijazcsff.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvqiedtk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ntfowbjf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nxjjjytv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mvhoiitr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jkelarts.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hysjuzpv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3jpyrnsvw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vldquuur.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xsljggot.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rtgvgpcj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3odddnyfq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3obizhqgr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwvxohph.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffckmidw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dbtvmfqe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rxnwplzv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xoxhgpdl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ksychyut.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3nexqjfva.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3egrskmwf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wdggcrcp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kmkbaruo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vkdawqwb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxwaiadf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qofblpeq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ogazbeig.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxgyrcms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqocoyxj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3aebmqznl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imtgzxxy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3syzsjtpd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3wtzyhhkv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jkfxpbte.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3aywdwcwi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xfvwyyqr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3gsgffipj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xdvcfnwk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ylymqytb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jezekokk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vqclsyks.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ipbtwrib.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yjodvlgy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pesjbarc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ncrvydma.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3knicfgtl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fvnsbavz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3idmwdbgr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3esawmcmu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zgysrkcx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kizudwqm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yacactbj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3juwglobt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jrrellfh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tgzqipsd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3crdcnrky.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmwxcnv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3emwtzpgw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3apaturpe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eznjztnj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pvoptkpj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rkjqkasg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jvquzplu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pjrabtfc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ilcabtqa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lsawtoin.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xjnrjykx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3obqlaqil.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cqptblew.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tzzqoxge.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vneojtpr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3rqsupjty.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3snelgldt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ncghbwgg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mtoyauae.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xopxpiwb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3srydbjjj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tpfahysg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xkyfvigf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xwnxicxp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qiikuakb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3oyzuisdg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmtnexcn.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3echtdnil.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hhsmiizp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tkilkjhw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hujqyqxm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kioneonf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hdzkttts.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hmimtape.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jvioirix.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pkogvryo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qgnqaqxm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lgtvhneg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jrhxwuja.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3aobdcipp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tdahwccd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3brxydvqb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3yecacjsd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tdolcxtt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3iazniela.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3elxytnol.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eovcyntw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qdzmwaav.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hwovbuzu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nurqdppm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3aycxcavr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rqhemldb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dkzyxfrr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wsdtprsg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kfgsqwwo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mqqqxjpw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3blxclqgn.html


<!-- 参考信息 -->