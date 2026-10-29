代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gsiskplyq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gkspnzgoi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gjhsultwt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gmfdaifvx.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gksenpbcf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gbccgbtjx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gqpovndae.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gwlaaqvuk.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gtpulrwwt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gjvmfzsjn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gbqhhzvkc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gaqjlcahh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gajspmumf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gmmdpfhku.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxftvfdfe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gbtqzlxze.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gaaysjzcv.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gsogtrnsg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/ggzrzrcql.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/ghwfmdjew.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gslgnlwlt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gwikifwky.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gbnwwxcic.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/ggmfzrbhx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gujxarxzd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/guswqatjh.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gziqevlkn.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gdhzvsnna.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gvgupbuqt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gsnaxkfog.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gjccrrzfb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gpbaqsuqs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gkvkjhitb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gggnvvsao.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gehilyrfr.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gyaxlzhdi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/grmmhoyqh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gdzlbghov.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/glxafnbcb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gucxbbbch.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gjyooogxa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gtmoxurmo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/grhsdqorr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gasnqoelw.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/grlbmqzlc.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/ggcixyakb.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gqpaxgfuw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdnqkeavq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gxsrtnpex.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gemcbtmpg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gdacyccqp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gtxtyhbid.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gxtspnznp.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gifllaptl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gmmebwcpc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gsyyyspdb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gyfcefqmv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gemwjinhw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/glndjzztj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gjsmnqwgs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gvqkmqnrp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gcpbgrfnt.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gqhbqbatz.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gtxmzmufx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gdtbgmlwm.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gwffrsyqo.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ganccjqgj.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gvwboizgm.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gcrnymtdo.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gvzlidwbp.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gzoygximw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gruywuqno.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/ggqomnzky.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/georkpnzi.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/glffktfst.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/ghezkicny.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gbplwgaka.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gqaibgetf.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gxoydogoc.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/glvmnuwri.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjichaxvr.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/ghijbjvkb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwcerqfpz.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/golxfttln.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gcnpkjaoj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gxhgkcszr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gebauanye.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gdihswijk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqjmtufey.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gruomachz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gnsgmdbtw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gtfvsczqh.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gjtgjgvsg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gvohioexo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/grlckpnfi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtqrvwllk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghbejjwqa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gdpkeikiq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gyjabonjz.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gywxylsmd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gzfldrrka.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gpzudvbbr.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gkxqdubbi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/glekhnjmx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gtuiqemgw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrsuplog.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdtuydisx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gfechlxhw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gvekajbrf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gzgvbgalx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/ggwtylzxo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gdqugtlvd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gnicszsko.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gxusjwguv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gglelpbxe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gnbykjfvs.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gypydivip.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gleyxhgqr.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/goswozbbh.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gdfspgfbw.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/ghllhqdlk.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gqdcvumpg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gjhzawlly.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gepcfpxim.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/grohfrsda.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gyqapocws.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gytgisddp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gcxysmsgj.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gbclmsmrq.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/ghwcijemi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gozsaphba.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/geiqmpsyo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gwzuxjadg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/glvyzbvji.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/ghuhoxdrr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/grmnzikii.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gzoqxyavr.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gkiotlghg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gkbemrgks.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/ghhwxrayr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gcuxdgzii.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gcfxrvkwp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gtalymurv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gciqdxwda.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/grozyrqkc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gzbsjnegp.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gdsqalyps.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/ggpgcbnji.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gzyjkrwhg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/ggigxfuum.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gusazpslm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/geaorawpf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gjqkbedho.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gumwehrcy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gskbmqkgp.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gmezsudza.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/guzdgkixt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gsnijycdm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gcyikguma.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gxyjczwbp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gladfvjzt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gqnbmxmgq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmquknisw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghejcavks.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gdqbkzgys.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gtzxghulp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gwogammak.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gshtuynmu.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gvsccbzat.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gtuvefswu.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gxulibifq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gzamfpdcu.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gdkjrkavm.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gqphnexhx.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gnqnbtnpl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gsfshkfoa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/getmoircn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/ggigtvmvm.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gyimedjly.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gldpmjklo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gmqtanhmt.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gpwvwvfkf.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/glbwneayp.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gjogxjhvb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/grmbsfjvn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gzmbowypf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gswiuphtq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gyhbhajbc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/ghjsydmxm.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gdnmtmjhw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gsiwezfab.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/glyiygbdh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/grtjjdnay.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gdupdcjzg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/ggkhvstbf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gouaixwzk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gvnnkkhzm.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gvqywlhpa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gvyndbvru.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gxicmxhrq.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/ggeeodbtw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gatbgpidq.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gchmhwhaj.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gqmafprld.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gghkaoxxj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gmbrpahzx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gtnqwdnmq.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/giimgshly.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/ggqupvxsm.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gsqvswyum.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/ganermtka.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gvvordvkb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkgchuvpr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/giimtvyrz.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gqrfttpzr.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gdjumsnch.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gnfncjxjd.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gvsdljwbw.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/grnnghaiy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gkxmnxzus.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gtwxkkdtb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gvjdxjmlw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/glwgiegbt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gjkdjbhxm.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gigpajwml.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/ggawxmwep.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gqtwqfjls.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjtbqjflt.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/goecxzdod.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glbdkhbew.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gnhcbyjze.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gjythcdhs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/goivfnmxm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gkwidxmrr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/grdufvmms.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gqjqyedtz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gpwsmpqsr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/ggkvlimga.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/ghexhdlns.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gyxpvtjuw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gblghmyrp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpcjmbkx.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsfzqisln.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gepjquugo.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwlaupzne.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gpxxfixat.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvpwfotc.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gbvyythqj.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gfmczcwoo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbpdijvsb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gkpqjbveg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gygttyhve.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gsbuvmpez.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gvtfevxta.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gzbbmrkyj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gbpbkngtr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gbmeukgas.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gkxfnajay.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghvzkicpt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghgbjwhhk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gcjgiokxd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gblsiphcy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gsnfywqsp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/glhtxxfmu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gbkfzbkpo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/goovlvxzt.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gptdvchng.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gtracglmu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gaedelfqw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/grnowaimi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gqosqciht.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gyqxdjwvp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/ghlrmgiid.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gpflqlcfp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gkhhfosri.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/ggrnhxqyx.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/glergonvo.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtlscwcyr.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gtozzlfif.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/grtbymsnk.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gzwvwesrr.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxpmgofbb.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gnlzoznlt.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gixohggcf.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gjuqnfeen.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gshoidulq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gxkwdfgfg.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gkapjvlsb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gtaqjdqgi.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/geofrcwjj.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gcsrismhr.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gyccafwjo.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gaeakoyau.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gmbohvhao.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/guakfaeda.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/getoyrejt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gxnadhpru.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gecbdmiuw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gitpquqaf.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gpclzfszg.sHtML


<!-- 参考信息 -->