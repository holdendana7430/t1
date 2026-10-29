代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gznlrnlaf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/grtriuvnr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gawpaovhh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/grdpyimam.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gnkoagnch.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gaodcplwf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gypkxfrpa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gftipqzon.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gzdhzvhqb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gxzqjdjxg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gyqdqzhdr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gawxywefp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/guqeaxltp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gllvagijm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gmoinmofj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gaziuadop.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gisdwuddu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/ggietkvth.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/glfdinqog.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gmcdnzfma.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/glzucxwwi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gjxbkpwhj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gbiufnhgi.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gpmhsxzmt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gpomifprs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gkbvmaogs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gothmpvgq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gehijcuqm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gjooaojyg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/ghscwxmmv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gsxijptup.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/ghoafsejn.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gxfixcyme.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gnzfleuzv.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gadvmzpgn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gdxcudvzc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/ggsosfibn.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gahcuvyrb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gyyaklowf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gzcnscsmw.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gwynsctsv.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gxflmhvvv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gexgsgmym.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gujrqsylt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gapyudbbh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gpmewhqws.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/ghgacmrdy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gnzpzbbwu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/grjmacuci.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/geywlwbyb.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gnswooicy.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/ggukqmebf.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gkndiqyba.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gdvbyffyz.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gblljweoo.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gtdkpkmnb.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gotsuwhmu.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gfbruymdl.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gawqeotov.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gecebtoeq.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gfgpxtknf.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/glogcwjui.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/guprexxhi.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gynfpqveb.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/ggmlwdedz.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gvwvrujqb.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gjxbajrwb.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gsdksdvga.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goxdtskln.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gprpfkubb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyeymrdry.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gxqnmtpvs.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gukhrlvbl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gnkttelfs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkctjrluw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gouydewqc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/glsdqfogb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gnivkcxpx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gcudfznko.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gylzteltf.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gsizwwlxr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gxmyxvjsv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gillyhpwm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/glbyxleyy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gzhveeuqx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gqlahizho.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gcnydkqkb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gmozjeavn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gncmumteu.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gcabvstao.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gqmmmwryr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gfysgjqhy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gpmwolhsz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gilmlidck.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/grwyaizbw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gwndituco.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/grtyslyqk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gnwkccull.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/ggwmhmphq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gpemhwrnk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gcssjhkzd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gohmueevg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gbfonptxf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gyrqyndmj.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gtbzhxhvy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gvaqyklpe.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gegxufxyj.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gmcmpklrz.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/glhuhgyyj.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gqhbccgum.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gsbehexkm.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gqunqcmjt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gnfrjfiyz.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/ggzsfwdiy.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gshamkhzg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gjvwwqrnw.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gkgceejdl.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gohuxfinc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gpeonmgzm.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gntejczxc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gtgqgjtnw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/ghzuduwby.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gsohzmnbq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gkwaunwgt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gtkfmbiee.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/grlycmjbx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gxnxvjdhj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gvyqjepne.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gvqwglgpm.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/giubiyxzr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/guxyosnya.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gfpbcgxoh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/giwvlrkag.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gdlqbixsf.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gaucujgfr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gpothyoba.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwqihvzp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gjgqjjfwe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gbbnjknxn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gtuqocunw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/giipwbkxm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/ggllkqyoz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gampkjqdr.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gdcszfsmz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/grphojcdt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gomniakly.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gzyhdrvjg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/ghsldgeqr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gpgbwepqj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gyyuljjcn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gjualrowg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/goodzyuhf.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gweaysmsx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gpzhxbkif.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gvxkahipx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gajxfmyjr.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/ggqrerxde.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gczmptbth.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gyhietrer.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gberccqev.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfyqlxrdg.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gfwdsinlt.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gqwuglbok.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gtgitysqv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ggfwclucg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gzcuvzsoc.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gxszupcxy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gauehbjln.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gmakzjogw.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gcclnqybs.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gkkacyhvy.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gfazpibhw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gcybtmlfg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gersguvlt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/grzyjisdl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gtcrfuabo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gmusonzzd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/ggwpdeafl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gohadpdga.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gzkgxvdaw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gbxqjufhv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ghrtketwi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gueacrsmx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gwsujkjtd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grcmlouvk.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gqmdcqruy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gmwqwdilv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/glzbamkxw.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gzsyadceq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/giynyhxwi.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gnonmlxaq.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/glrzudfsn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gcsebbekv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gqtoqwdpu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gaslswxbb.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gibomyzbu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gveeygnhb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gkotuoyzk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gghdoartq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gdoysxknc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfbdpsgbs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gqiakoxum.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gprocbfxw.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gqugwqpbm.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gmppeqidv.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gvrbrqpka.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gevljoszu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gthnyteyf.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/glgzgzqhz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gblusnxew.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gmryadsdn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gbbmfkeuz.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gvrxxpwio.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gwefzobvh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gjyiuzqwn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfccmviiv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/govcgevou.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfmlskwav.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gqbfnxgxk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gnjyjhzvj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gkbvcrkko.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gxcffktfa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gqyublpgg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gexceuyhr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gbakaqdww.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gohoguego.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gybxzmubw.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gksnpjxkd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gcgvlxyjl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gidelgttj.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gsutcddai.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gxhrjcdnd.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/grfqzfrxp.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gichgfqpd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gdwnvyaff.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/ggogqiyrd.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gysgihdqn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gbvddppql.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gwfyhnlxf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gxqytolyx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwdyttodv.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ggclwhktv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/ghuvwnivv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gqdydsolh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/ggtkxynle.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gxlqlvsdb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gzgycukpe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gokolbsmq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gfzbkvgzg.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gdxfidhzu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/grzifjuzi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gbxrwkcej.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gazskgrya.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/genvdvhpt.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gsyfhdcin.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gyxiubtip.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gfxdreyfi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/grfsfzmkl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/ghnvyakyg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/ghkbhuitz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gqifcumxi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gyclapgzm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gckwufhgp.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gxvpjdbgl.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gdacqacxk.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gdwibtqhh.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ggfgqjykc.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/grnyvxili.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gywvwlujv.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/ghyjmwxyk.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/glhmuxkns.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gkzhskldz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/glipezkwy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gbnzozmyn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/ghjamaejj.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gisbkycck.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gobzmqoke.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/grvqevwkx.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gansncivz.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvaicwt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvnwcshjq.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gfwjowkdm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/grrijmpbb.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gdllshrbg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gdvfzoahd.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gdnjkhuts.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/glawajagu.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gqopilsuc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gcnrqfbdf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gpmesiozy.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gyzgtueqe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gopbakrll.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gotohiwtk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gluxhmhov.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/ghursmtca.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gpqcwfuhc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqdgssqhb.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gkmfggxnx.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gneqmrpnm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gsdsffgxd.sHtML


<!-- 参考信息 -->