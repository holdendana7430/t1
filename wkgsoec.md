代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaudlucdt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gybpstzjf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gpmgjjisv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggndwitje.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrmccpmq.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gevjvhueq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fanxiaobao.xyz/Article/details/gjsvdjuit.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gltnszdwb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gkyntrbjb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfbboprk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrqyyvty.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fanxiaobao.xyz/Article/details/ggehfymyq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnnbxyro.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajmvvurl.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gyywcczmf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gshbogyco.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpyrrpmk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gepaxobfw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcxurhcv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbujjndxj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/ggghldzpt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gevfglzka.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvxuratj.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphiceorh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/gtaptboil.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdzlpmyv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/geexvdjhw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtoqcmpv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gonowimdb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fanxiaobao.xyz/Article/details/grwhihbgb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/gdnibrxzj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fanxiaobao.xyz/Article/details/gygglnvqz.sHtML

[B13] 判断是否为数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gogbqubbe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscgbpxko.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/geqgqoodh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqhttcfm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqkoomgk.sHtML

Java: x instanceof Number
来源：http://read.share.fanxiaobao.xyz/Article/details/gaumbthog.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxltvpxwi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdoalmcf.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpsukuap.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnxfddfn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/galtbfhmt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcynozven.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glosezqbc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdefsnep.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grbucjqcc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gasjkqcaq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqksiqtrt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganhmhiol.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkmhcrlk.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/gomjztazx.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gwbqsdjsi.sHtML

JS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gphjhexlh.sHtML

TS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gjmtissno.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gbritwlza.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gjbdjpsmh.sHtML

Ruby: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyermmzs.sHtML

C#:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvwzznbq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gszupefdg.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwihmtml.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvdwnfzjg.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlamivat.sHtML

TS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxadbxahe.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjhehvjs.sHtML

Go:   if data == nil { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gypdadzyt.sHtML

Ruby: return if data.nil?
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhypkztf.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geehypaas.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfrmambmi.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfmqnroa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbdhqjqdc.sHtML

[C01] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkzomylsx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoacmmyy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvbmeaftp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdphahsic.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxhrprfti.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvovtbfbf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvrbqihd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafitlyvz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glpkxhnzd.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gnvjpolop.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fanxiaobao.xyz/Article/details/gdedfnpmr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfcbsfnvn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfuvmuka.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gojywojua.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrldfext.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gppiufupz.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/goqjewdwy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/gdikmtxzh.sHtML

[C03] 可变参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmassxgei.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuacecpj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gflrooaxk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtrleetcd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjedkypd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giadhivgt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmvdqigf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddboavhn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gboifdzdv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwqrokmh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqefvwwwm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklahlvpu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnmxpmzbn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrvltlqo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fanxiaobao.xyz/Article/details/gyxmeeqaf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggntqhbee.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcetnzipo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypptsmjk.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsbimyzf.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtyamlje.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/ggnbbnfop.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gjpjlpvtw.sHtML

TS:   return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gngjgqsot.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galwzsnne.sHtML

Go:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gchmmkdzr.sHtML

Ruby: return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgenlmtx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhebnjez.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fanxiaobao.xyz/Article/details/grbnfihxv.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fanxiaobao.xyz/Article/details/giqogmaey.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukdgtkmz.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gygnbdsyh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gdwpsucfx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/guuxxbmtl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gcgwerxqt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/grnqceatq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/ggdlmetmo.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gphrfnzic.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimjqyxyv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzwevshp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnekxyfy.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/gnnrfzboe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuvrtmwx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fanxiaobao.xyz/Article/details/gvavqucdj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuwdwokj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnptavfg.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwlhrehp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbonrdvfk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmoytugjk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/glurhuhre.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvwyvmbf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjhyhdzs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlmejtkx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdehxaryh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohtpkicz.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gigfrelmf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glqzmsizk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/grupvobmi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/gbrrcfqil.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvmjqhqq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpoyqqta.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gomdkpmxq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggwejyrja.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnpddpag.sHtML

[C10] 变量作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gcxwmcqdq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtgeyhtd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/guxmyomon.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gdycirxdw.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/ggypagowx.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gjrhpbbep.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gakbqesdc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fanxiaobao.xyz/Article/details/gpwdgncsl.sHtML

C#:   块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gxydglbbx.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrlvisve.sHtML

Py:   from module import func
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajzzvbij.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpykcsyst.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/grnxelakk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fanxiaobao.xyz/Article/details/gidxoikvs.sHtML

Java: import java.util.List;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gparedcbq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fanxiaobao.xyz/Article/details/gitiaoxzf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidqnpxgp.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/gpcnoutzb.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/ggobjlgid.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzobvnqa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/grcilmtgh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gtsptvsgg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gpziixfwy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fanxiaobao.xyz/Article/details/ghcsxllmh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/gafzvpedd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fanxiaobao.xyz/Article/details/gytarjrrs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glkgaamsq.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fanxiaobao.xyz/Article/details/gcmsrldof.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gnccfoxvi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gshoyeaer.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqnmfiml.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrmktsgg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnscqtqar.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/guydzcnyg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnoauklr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fanxiaobao.xyz/Article/details/gumovjxea.sHtML

[C14] 泛型函数
来源：http://wap.fanxiaobao.xyz/Article/details/getofbsil.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fanxiaobao.xyz/Article/details/gliunjfwo.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gokzypvnh.sHtML

JS:   // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsgzktha.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyvxsefn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghspdvdkj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxzacnox.sHtML

Ruby: # 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/ghrdjvkwe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmbgwfkh.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fanxiaobao.xyz/Article/details/ggxidivpd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmbuibgy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjewzvhnc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgplpykr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcnldeip.sHtML

Java: // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwbfmwpt.sHtML

Go:   // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkndvdux.sHtML

Ruby: a, b = pair
来源：http://baike.fanxiaobao.xyz/Article/details/ggkoojbbu.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gvsabznnb.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslkwrned.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpkabjpr.sHtML

PHP:  // 无重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeuwtrno.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkspmedf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvcurkxq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkleofskr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/gfadkqdjb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fanxiaobao.xyz/Article/details/gozdurcii.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtplrvnzm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gciltqykp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaiqfcwc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpprhqiuz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtepdohkm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fanxiaobao.xyz/Article/details/gyxdgnola.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrvtpcrp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/grombivcf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvcosvkn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/ginqeqbgk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/grtmhvvfo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpvpmdbc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fanxiaobao.xyz/Article/details/gxxmbwbuf.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtokjdua.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjvuusvd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuplqpqj.sHtML

JS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/guddklvct.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goappcmga.sHtML

Java: list.add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgtvayfz.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gbhjjbvps.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtlfanvv.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gvklirdcx.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fanxiaobao.xyz/Article/details/glolsoxln.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzoogeex.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqezunzi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsusgpbii.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/groldfnka.sHtML

Java: list.add(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gppuwnkvj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsuzdoeb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbtkbsal.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gfnrmalce.sHtML

[D04] 删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/grxsnuiru.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gwropwiby.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gimonthou.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/gcbivlhst.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gijdgpvxa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gwbhoqxuk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlygwehw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gevqwypkx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fanxiaobao.xyz/Article/details/glvvtbmmz.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjzkfjsy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gzttmsjuo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gdjymwlys.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqixbqjm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofjxgpms.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/glrsznypm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeycyaav.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gikniekve.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gktahigrr.sHtML

[D06] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjeojxxd.sHtML

Py:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gjnlnyvrp.sHtML

PHP:  count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gfpcvdvph.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkrsrhfq.sHtML

TS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gwjiorxep.sHtML

Java: list.size();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbqadpgz.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gzmodiiyr.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gbngpbooq.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbjbqkee.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwecjehoa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigkzcjbj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gppxzbyhg.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gslgiqpof.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtgpueno.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geauxcfza.sHtML

Go:   arr[1:4]
来源：http://3g.fanxiaobao.xyz/Article/details/gamoqvncp.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgbpunyz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvsqgeqk.sHtML

[D08] 合并两个数组
来源：http://blog.fanxiaobao.xyz/Article/details/gxpbmmtji.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gpdxibgkw.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gfymkohht.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gsposruww.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gphaiaook.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gvaorryxi.sHtML

Go:   append(a, b...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzkorrhs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gammjnxnx.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gavtujkun.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjtmdetv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkptjsuf.sHtML

PHP:  sort($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gccysbxqa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/gjhezrzib.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvivhnyuw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdrnsvyo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdmkfbko.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gskdjcqen.sHtML

C#:   list.Sort();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfwgvbcf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyzutwvq.sHtML


<!-- 参考信息 -->