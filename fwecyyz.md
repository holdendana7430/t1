代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gbdpcflfe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gqdyomriv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gnwevmrkl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gwygkrieo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/govukopnq.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gwygakoeb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gvdqnglhm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gfpcnhavg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gqbihwptk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/ghqlgfero.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gzketxxyx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gieacxbxl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/ghroiyyhz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gsxuaafcu.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gncedwamc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gfdmfbdoq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gumbusrid.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gxanijvlu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gyoglxnyu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/grrdqwgka.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gozajmnyt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gwwhrqdbw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gbzcoxksm.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gdloxstkw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/ghvcjgadv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gvfbwfkil.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gmhvjusni.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gyetbgrrl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/grujgbpxj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gnqwiajvx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gktytavij.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gqjozqqmw.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gjjhukmha.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/glrsknxsz.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gvqacuipr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gfghvytgz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/ghqudliqm.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/glszufgmb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gwdqfrapn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gxeenryda.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gdjkzrcva.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gisjhczdm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gceknbzdc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/glxvvlfsq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gozjbftcm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gnnlpraua.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gkomtidev.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gshxnvsrt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/guzpiqatb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gakwngowq.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gwopxvdrz.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gudkaixrf.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gspiocuks.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gcxogxrgw.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gwdebektq.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gpcdbeach.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gqbfftvfx.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggqvcgfhc.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/grcwrlruq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gbufpadtc.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gwdmycrtn.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gttcenyry.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gehmefpdq.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gfuffpvrm.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gkkfqauvf.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gstllsrcb.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/ghbwmtwfh.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gjlnlzkcl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gewvaanmb.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gvanekxwm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfosamwtk.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/glkikbggw.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gkjpsfxaz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gdbnlxnmq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpibgcvxa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gugpjyaab.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gdrcbdkva.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/goeijsjlx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gbrljbmsv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gcxeeadcp.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gzsofehif.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/grolbhcyc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/ggkijsgbt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gijwlnfzf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gehxazsop.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/geibdleyz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gbsfpujkl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/guohkzqab.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gxkoscknf.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/glkbkqcfh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrqelmge.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gadzlelvm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/goanvalnr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/grwalqsvl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/ghvlyjxiq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/golkbgczg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gptkmfmmd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gwlibtdzv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/ggkcatpxz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gxymifohf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gnxvgcrfh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gcarnxoin.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gakqssbiu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gtyktzzmq.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gztduypcn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ghcprwtbq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwwjilbrl.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gdubqeqtk.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gqexrhgln.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gnrkccqwy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmqzqmf.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gcjuwjtgm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gostfqrlv.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gaxziujqn.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/goydhayfc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gxixybddx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gjllvrizj.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gyekqvyxj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/ghqpkjicp.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/grnvpnzpl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gwgxxvhac.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gzedksxws.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/glxdiskct.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gpytzyhik.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gogkkzive.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gwwuhlxmj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gpehmwosf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gumwjvklz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gshpxtwwx.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/geszljhqe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gvoawkhnd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gfkuhbadd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gjxidcyqa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gdcwgfnbq.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gkhfwnvwl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gucckdofg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/ggxdtgbgk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gwzxajeld.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gyhzephrf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gxrbbedem.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gubmdrzqu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gslotpuyj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/ghfklxznr.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdrlzgcca.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gpyatyhfo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gxzoxvjxt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gcgpxsznb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gryzubkhc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gokwkkdwv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/glvjfkgfl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmixnlogk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gyzanrocn.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gvrewucfa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gcdsvkhgx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/goofzwzjg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gzqimbope.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gkzqygvjm.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gatnngjsg.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gtcedalvh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/ghusrefet.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gderlhoki.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gywkrzgze.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gzmcwhctp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gswywcjvi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/grxzwntre.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gwhdvwoyb.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gltjoemhp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gadajswze.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/glnuwjmvd.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gffxusxzm.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gngrbsdpl.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gjokdienr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/ghmzplwfk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/ggvqclcvc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/golzfzbac.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/giftyxajv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gsmvuysfa.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gmoydzcwv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gfhrjcpfc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gvcamqfum.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gnlvtljnd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gubqrmkrl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gikzyezrg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gafesqady.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gnwfnbrpq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gtxsdsnfp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gquhcckkt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/ghavtqfth.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/ghdfcblwo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gkpletaqt.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gdqrlkjrv.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gbebfewis.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gonrnrtnb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gqpqrnvhb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gfgxcfyvx.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/griqcaspz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/girbhigyv.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gmhxczdkg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gzhxpmvxz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gkziqddrj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbikzqwtu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gitiijtcs.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gpuqenwym.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gaelaqppz.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gekjohbjv.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gadiapcal.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gizyxmckj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gqbpjgbrj.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gzusarbhy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/ggjljbqgp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/grjckgxcn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/ganmapumh.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gfoydmpwo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gwwhyktyt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gzdiedxqd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gipnlbpee.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gudshkpiq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbdzhbwyf.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/giryimdsy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/guzhaphpd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gsxpslkwu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gqqaaeefs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gyhhnmndb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gzviqwbew.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gmrljrfqm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gggkvpasa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/goidfufqn.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gxprurxpk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gdrskhboy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gdcketkuw.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gcoevjrfo.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gvttmizam.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gwoumghlm.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmusleijz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gjucahnpz.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/goivoqbec.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gjghubduw.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gwdjomncq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gxoftnbph.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gwayaaujl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/goamekebl.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/ganpfowiq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gpwphkjbz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/geeayvjyx.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gsmuyikaa.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gteeqjrud.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gppyqzxnr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gneskghee.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gsvtzaghr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gbsvpdzls.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/golwbfyjr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/givqzeprl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/ghlhbmoqa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gieojfpgj.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gxjjhtegr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gqmikynhb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gmrccyjrj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gaoqzlsgu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghmtackvg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gmsoyuauv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gnbmwzfvy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gobnojevs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwoigaphk.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/giuhhwmvn.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gofozjieo.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gribfhguq.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gxaifdeph.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gnwblkkkg.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gzckwibhh.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/ggcwbdslf.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gljmnrrob.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/ghzyrrfht.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gyajqyrla.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gnmcnyiwf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gpmolpkht.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gqwlgspzc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gtqdszvbv.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gcacsaomt.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gtyuebeyi.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gudlmtwxl.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gcyworkfc.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gygknlihw.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gjthjiiuf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gtdyawhsm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gxtczmpdu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gnekcsrrl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/guvvltdlt.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/grtljqmuu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gjqmapcas.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gzjnucnoc.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gzngzbxji.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gsxkkyirj.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/grgfycxyo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gtccxpkda.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gmzpeqrnr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gzmxljzuo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/geimuhegc.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gwciowvrv.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gqiggwvxi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gyelotrmx.sHtML


<!-- 参考信息 -->