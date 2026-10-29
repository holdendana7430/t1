代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/gooesgjkp.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gxsjiicuu.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gwesfwsjy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gprxbyfln.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gkdpmmtga.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gfyxwynpk.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gtieddkqp.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gdisuuqmn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gytoyhlij.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gpkfcmdpp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gvaifstet.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gwgbmceak.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/geshlixmo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/glsgynrne.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gjowetqui.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gjtwdwcii.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gjsilydsg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gcongltlp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gqybjwolq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/glgxyaeew.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbryhhei.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsiehcyol.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/ghgjcjqkg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gmqwnovzw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gmnksrdcs.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/genxniecj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gloddaoeh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gcxnlprap.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/giqcuturg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gkhsvkcgy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gqxohejah.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gwobwgygm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gzcoauewm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gqdbdrxue.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gqetipmpu.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gpfvhsfjc.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gymzpghmd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/giwtuvenm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gyiieqtdo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gyragdtgd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/glqdvcozd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/ghzlvhefj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gnoyibbrp.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gvdzujixb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/groirxube.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gmbgwvonu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gcdyajbbk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gxwjxrvdi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gpezapugg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gcqeohcse.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gumepewfh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/ggnoqkhwu.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxhorjvmp.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gmimkljio.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gsbryfpeg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/guuqdusdd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gsgpitbnj.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gkcizleao.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gsqbvfhfr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gwtewbnrl.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gvkungpwa.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gyceanbmq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gwutmvzce.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/guyloxmrk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gizovvthq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gplmlxytu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gqjrawxdq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/glkdzfwuk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gysxexzye.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/grbbueays.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gslhfkyju.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/govzyxbag.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gqfyhafcq.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gneectkyb.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gdvofhjzu.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gihlbefmw.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gpnojnmoo.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gdcugteyn.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/guwivwbee.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gzwkleczt.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gcjuwlnqi.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gvarbfymh.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gewlhymam.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gtvuozowz.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gjagdqmbc.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/golyjrepr.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gmzzuequj.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gbavmysmq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtdwmyjyd.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gxsrcfmvt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcaxcqavn.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gzyapkjbn.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gorlwxvtg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gsgtlmkhe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/geboqsfdg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gfqjvcuom.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gmnufezvb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gfxiymmfp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gnwudmmgw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gdltmrsao.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gfuixvrzp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gaetgdvhc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gtswddkpo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpctjweud.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gjgiftbnk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gxnohaovi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gnvmccoqj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gokimzhja.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gltewcuuf.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gitnybcvu.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gzuwbhryv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gfbgagjgw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/geoowoddk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/grjjjsmya.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gobyucwld.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gplmnsygc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gftfpucdg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gmmvgwtpf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gdqsmjmpg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/guwkahwbn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/guzeurtmu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gqyrqdbpa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/glfpwikdp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gfxihinyu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvawcmfvz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gtfcletio.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/ggnlbjzva.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gbapclwkv.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/ggmumwnub.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gxefdrdcw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gxqttvyjp.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gzwtbawqj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gzjndoppo.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gxahjzxvk.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gatjckqhh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gopupaerg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gjornvqcc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gssrlexup.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gclyrvufe.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gljprziiq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gdgjltois.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gjydcgbvd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/glcyrlgwp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gwziudadb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/ghbxzmfmq.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gmsozvday.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gklprrgfh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gdnyhaxpm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/goaevhuoy.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gupviutdc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gekcdlmuq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gyozigxxn.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gybqpltqq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gbjynwtre.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gepgtfdjl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gxcojveab.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gjfphztcz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gqbupwscz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gxebexdwu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gwwhubdif.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gthsunwtd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/guwyulthi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/goyhxerfb.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gpiytknpa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gnmichusw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gdrozfbis.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gjgqvasst.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/giixmkhkz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/ggrwscysm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyyrrckwl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gnzfshxve.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gcvsuhiic.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/guikpvufy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gicionhax.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gdjbpcjkw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/ggigbuweb.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/guszlgmla.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gzgvosyph.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/guhzebafs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/guwltnvva.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxubryind.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gcajbckht.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gysbyisse.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gcuehthmq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gqupqlupq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gnkvcfqmq.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/ggwpmevem.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gjoqckrox.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gnzyiyfkw.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gmfwekgwb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/guqhruhlm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gpfjlrcrt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gssbkkwds.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gzcokkwem.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/golvkasqp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/grfwbfwzj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gspyxmecz.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gjcrsgwks.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gkhcqmqlz.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gnpgcchxq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gsyhdwkwb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/ggojmddxa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gligfbxuz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfchajsni.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glrvajmrh.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/grgklyile.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gicdvlkmt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gnzulyfci.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gldsqsqli.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gghdwsvtk.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gqhyhusal.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gqwrfhayu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gurqzqegk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gljxuvkhq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gjgxwflcy.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gmkvrbpja.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gzgiwpqnn.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gaauyhxni.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gnusuvfdg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gxltbjxiu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gvqvuijod.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnqfafapn.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/ggobsbnlp.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/ghdwusbxb.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gadtryhoo.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gxrjodamg.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gtfixcude.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gwmameyga.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gfjnvubgs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gtqobdfjy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gcgyhdkxq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/giesrhvcp.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gxzycniwr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gyuvygves.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gaajpawas.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnuhkkqqp.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/glrjvzumc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geydfwgcj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gexxctqyd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gffpthhrf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gdkvibhli.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/grbrylooz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gepprxjfv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/ggsgxkqtc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gwiyisxpv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gvlcgtvvg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/ghuezaxdh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gohitbetb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/glsmfkfif.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gwbwptrxg.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gdzltaiee.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gmxfrzdmy.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gouicjpnx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gagvinpqv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gzmzvszbx.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gkktheysy.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gvlrhrvnp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gtlbxmsuv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gdklxuuah.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gnccgkekt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gpuhkdjgp.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gmwplpuqv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gxvkyogoe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gpyyhnqgt.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/guzotgqay.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gdasjgqpb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gkaaccgba.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gmcdqbder.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gavyidefh.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/glwnzpplc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gfrvlmlmi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gkyzplgdf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gybldqpnp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gylgqsrrh.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gbxkwzjmb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gtxftfrak.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gpfvxexye.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gwcbnepaq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gshielgln.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/guzjsdpev.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gzxwutvzv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gqaphcpud.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gdojmomat.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/glgmlhoie.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gjprltgrw.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gybuaqqnn.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gwmlxmjst.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gyqfmxdgy.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/ghaogfstk.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gxxwiqflw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gbykqtblh.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gpwmzgzbz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gplamsomc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gvkibdxid.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gnvjfxzso.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gakgjdwsh.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gfqasjrsd.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gnlgmsudr.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gbqemtwxn.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/ggjsrbfzt.sHtML


<!-- 参考信息 -->