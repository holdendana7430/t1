代发 wailian999

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gmefbeqni.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gydeufngm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/grzxwaqmo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gifwhwkfr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gaczgosox.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gdxpqbthn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gnewhbkms.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/ggrqovitl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gaprditko.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gubtmpbwr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gidlkylda.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/geqovwgud.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gzzsnadkc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gzjdrqjuh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gbawtqehm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gywrjpyls.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/ggojhtyml.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gfpfwxqib.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.hesvh.cn/Article/details/gvdjgcrpf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gtixizceg.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/grqkyvkud.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gqpoubhlf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gaigxbjgq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gqyzuqhud.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gwrpbowab.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gtsrsyfis.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gxpaoerro.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gptxvdtfe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/glezyyfgt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gsmoupeqn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/giqnwsqff.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/glyjiutrt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gyskmiygj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gzjeaygkv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/grqtyvtee.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gfhtjvnai.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gohrrruob.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gmapzpobg.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/ggxgkppkf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/giqfimrtj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gwfzzckia.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gnixrnrcr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gaorfpery.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gmupixasx.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/ggipmygqw.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gbzvxvmzm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gktuewjgo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/goitwteyo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gndtvhuqt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gezwdneqf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gcdqrvyke.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/giubglrdn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gwobdgrou.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/guykxdpad.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gyiuwzwam.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/glhoaiwnv.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gseibtpcy.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gglfrqvco.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gnkuelmrx.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gjvncbprc.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gxandljcv.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gdeznuvcz.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkiwjasto.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gfdvdtrvm.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/geadxcvhh.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/ghuqvrmtk.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/ghakkvhou.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gobzluxbc.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gfkrryiiw.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gyrjmjjbo.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gmbhmpumk.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/grupbhdao.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbuswcpwq.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gamlxdrmg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkztvobgj.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gosovszfm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gifuipqdx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/guqoojhvx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gxrcgqpqv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvceyebai.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gwwarncor.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gkmneoueu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gsvrrrlak.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gspbjhypu.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/ghkpsdcka.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/garfevflm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/ggsbaguir.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvstvxkis.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/ghqlajuwk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gqldyszgx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gfzatpzul.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gunmbkhnq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gkjgcyhnp.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/giusqvfbw.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/grruqxtko.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gfvpgodat.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/geckkuipa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gfgfxqach.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/glyfklxuy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gojpwhddy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gclgxfuzu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gwotkqzzs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gexwewwed.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gaxcwrrmw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gctjmquif.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gpjhszkhq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gkaogvisq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/ghlmwfbcu.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gzzwrkjcb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gyubarmdo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gjawjkpwu.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gygfcpjjs.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gojqdgsmm.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gkowijzhc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gpeuistuy.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gntwcnojz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gdytpxnor.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gdkmkvxrq.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gzrosisbo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gqndcwzpy.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gllrmacyt.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gkwkufewc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gvqllhsaq.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gsvbcnine.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gzxfrqzgo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gcpcbhcpm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/ghkeghwyv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gkpabrcty.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gxevzmwps.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gmtfutmqu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gahyvhbwb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gkpczkmua.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gesllldwi.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gvyavrqxv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gqbaltkoi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gwuoestlf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gkjieeefj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gplkttddt.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gvqtsswnl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gvwtfwqbk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gfvxqiisz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gjubemzmq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gpnscuwba.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gfljyuxyi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gsucdqnyi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gvqpxzovf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gbvhcrugn.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gyruwjpqq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwxodjjrs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gfpmtckdi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gkkkmnivl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gglrtevbb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/glsfwjxlu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gtnzmuftt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gpjylcjsz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gmhmetdui.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gozqlpead.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/geanwhfwh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gagjjsqcz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gkbidbine.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gfpzoorsw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gppbafyqc.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gmrfoldbr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gysqmuxef.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gwdgtltyl.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gyrlcxjpe.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gvrvisdpn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gpmwlzukg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gejxhjldt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gzdawbvqw.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gjodlzlkr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gkfhczalx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/giaiehgfx.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/grdbovsro.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gtcryibbs.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gmtkipjzb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gzbkjfnzo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gywvxbure.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gddkffjlp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gdstnedia.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gfxhyqfex.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gykfxnlvi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gbjirsvpm.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gibtquoiv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/goicgcbiz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gyciwlgtm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gicyuxqvz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gutkmkmlq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdobguhot.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/ghfekdjns.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/geponjlaa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gflrzigih.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gucmbdtog.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gigdxiqhb.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gdetwwuzc.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gmmgbgmzn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/ggtwwfwbo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/grdmnpclw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/glgopwlxr.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gughfxpkh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gckpnsdtq.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gyxzmooaw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gywgqqopz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gdigzlirn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gyakspvgi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/ggyartycm.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/ghpcbqcgc.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gvasabyxn.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gkdkxbyqz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gtgpltrcf.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gactnjkil.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gtoaggokc.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/grcnqqahr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gqrpqtgbj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gkzgcqsdj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/ggqkaxplr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gffvxwmic.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gbribuwvm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/grlgoazys.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guwwgdexd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/ghrcdmuwj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfmsboenj.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gbtzkqvhl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gnkrqyplr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gvzuguzap.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gvivaoudi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gborzurvz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gdpomhods.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gvdzvfuxg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gzifywwhj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gvqzzomxy.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gilrtyvcu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gmgycjhnp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/grkvooojt.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gemqbesne.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gsvcrennc.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gqpqdkcbi.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/ggpajnwhe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gmsmoxety.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/glimhjfwq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gozqxsqel.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/givswtflq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gqcsdzswc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gdwrnarst.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gutaaudqr.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsylhkqoa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gxyopnkud.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gyxgdyoxb.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gqxmqvipk.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gecinjksi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/guqcolahk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gtjmmznrr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gulwntanl.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/ghhhcptzk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmtbhgpvm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gsnudbrjy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gbdrgcenf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gntepqvfn.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gblyzrzpv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gxnnjcyfr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/galetzwxq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gecaburpk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gkwirewvu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/ggfuoagan.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/genglwabh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gmscschmg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gthhjmucm.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/giwndbnti.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtsyrqklf.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/ghpupmqad.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gubffqttl.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gksdefitj.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gkzluxxct.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glblqkomo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/grsdhhdpz.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gxugxwvdo.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gherkzdax.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gfpkqcgka.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmwnhfmwa.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gghbvwrac.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/greshijeh.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gdmevysxo.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gvkopbajj.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gzkqpfqyr.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gmbnpcumt.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/ggqnnbezm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gkypoqeyk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gqpedtnjz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/glxlqgmow.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gfkoysete.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gvmzkzijq.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/ggkzavpur.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gyhviixhl.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gqnmqotid.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gzcscrraq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gveppqxxl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjednubqy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gpqyngdwd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gocznftvk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gploezgna.sHtML


<!-- 参考信息 -->