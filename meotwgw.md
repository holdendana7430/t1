代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gewvtrmyk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gcgrsqiqu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/ghvmzmnwm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ghxtyjtrs.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/grfzoviqx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gpzpylejq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gqprmfizx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gbjdnhjxq.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gjwisbzns.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gbfcyptsw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gozlywxau.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gvuplzeuu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gqiuahpgb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/ggvudivij.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gotmswzpp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gdufuejzp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gsfigymsk.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gcromrbol.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/ghfpmadru.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gjwitywej.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gpsksswlm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/ghaottylu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gjzfbwvfd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gebplwdmx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gewsvrxzd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gcaoxpyvv.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gzymqujhi.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gwgqkewzt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/godtsdgdm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gjanbmjrv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxwxvapiv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gajkowlup.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gelxttnrw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/ghgegmsln.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gimyecfso.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gexhmxjrc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gifsztiss.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gsvugikzb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gwmnexdow.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gtiiuadtb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdiozgoet.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gvssapjhg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gnftyxcqu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gqmzkctwa.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gfybokjbe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gceswvjma.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gvrgondox.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gfzzcgqit.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gsktujomo.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gosmikafd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gaktnpbcr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gfuxclhnv.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gfmddghcd.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/grrvflxkk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gsnlqmxmr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gvhloiotv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ghsbavvgz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gexougtkv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuxdamvb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gafvbwcrc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/geqqkyhhw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gnugtfvwc.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gqgfrispd.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gjgezipog.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gudmsdvuv.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gzzbasnpg.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gsujtrlyk.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gnmiokzdw.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gaextlnni.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gucigsrci.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkkbsxxej.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gffytmaqb.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gulfauvtb.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gbypklifh.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gzalqztjm.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gdjzmyfap.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/ggaorzglf.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gcfyoiugr.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gphwxzibm.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/giajxusnd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gchswagsm.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gbdsvtdtx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gybhnhntm.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gpjmrkkna.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gevtmcqrt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gdnkzzvfk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gadfghrql.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gjfxyeywn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gtrgnkynl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gdmtaosnt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gauegrcgc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gukcphwfo.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghpvgssog.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gozfyjpuq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gmtzchpir.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gpkxpgkcj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guupwywth.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gmvlhrhlz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gzemnpmtl.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/geuwkcsqi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gouuezism.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gqajxbbvf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gfaovhhuc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/ghohiswlm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gdgvlhjzf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gysqwpvmw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkpeirwwk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gdcocokln.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gjdvvefcu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gegmaimeq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gonkefyzd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gsjhgnqit.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gtebipkmo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gbsacmvha.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gheqeesmy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gkzzyvxrp.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gvtcpgvub.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gklpfqkat.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gccxulgvb.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gxbkzbfmi.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/guchdsxwf.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/giwhyrnhx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gadusxics.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gujqmkygw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gitbwyjzj.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gknbduclq.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/grxkemlhn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gyxceuwzn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/ghsdogjpt.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gyyaruekr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gcnfrowqt.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gvpcsyrsw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gmxphbjpv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/guoxjsomy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gcvidfxqu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gfuvssjha.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gbljbjrap.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gjnehnidz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gzfsbhwsx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxafeleyy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gadqvtayl.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gumzzejnw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/grlvlkypj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gdxxdqfqr.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gzafjugiz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/ggruojfeb.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gnuxsnzcd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gpcugfdok.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gythftziw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gugjreegq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/guvqbcpda.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gnphymvdz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gqtadjfpz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gmvxjgswl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gmpwsyazr.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gfeykfxxk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gkhiyipen.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmxupytdr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gzeewewos.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gkmmshcuh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gcpaygrwg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/guvuexogf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/goijeehuo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gqesbwwhp.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gcccjrhhk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gnwfepuso.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gvshndspk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/goczdbeak.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gmhptyodm.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gjsklonww.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/ginysqneh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gshlcjmde.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/ginhwxnat.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gqcnwsvmi.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/goqiqweca.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gicbokpan.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gclkhyyiv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gqgteuhgh.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/glczdoixx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gyiukgmhw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gweyhbbxd.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gifzloscl.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gzlhiesjw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwgakfdp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/genhtazuh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/ghkitwtku.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gachslaln.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gulzwkcgs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/ggflwkobb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gzckqhpot.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gswugxddr.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gqctqzlwv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gifbwpqtn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gbvhporjm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gpgwlbbvj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gmdarshrz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gfoonhomt.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gcbbtlhrb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/glaqccmpx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/giafcyeqd.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gbcuyamkf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gmcizjtus.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gnkazzlfc.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gybpmqtbi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gwucuwnce.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/ggplydajx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gjjaajlgb.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gnwpwbznv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gyxgfbehw.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gniyjoide.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/ganbagltv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gnwufkyww.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gpayayxtv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gatvzgwjy.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gxixptjux.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gamdxsfud.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gwtgxpzcq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gjnsvxtln.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gamjefaaf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gjlkfmedp.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gkftkcvky.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/ghozieclp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gligifdet.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gzewmriwq.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/grasvnrdg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/glrljfzzj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gjttydlha.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guhbyjiqn.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/glixpnwxw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbcbgdvlb.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gyuprudam.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gsgmgepvv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gepyjkmyf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/glntmvgwi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gdfauzhof.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gzyihyzlo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gdzbshhib.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gxantrexn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gvgrdspin.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gxonpxgzu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/grcaqdoln.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gknrxgtwl.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gazozzusr.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gupjvhgkk.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gezljsioa.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gabclownj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/geipmrhjq.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/griltzjjf.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gjdtdajwu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gpixcnvks.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gsevsrovx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gwypsllsm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gvstlmbal.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gmvnzwsjq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gegymeccd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gctwlavxd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gvobsydnr.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gycrtojxm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/garjfvqfv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gxonhvdmw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gzhkhvnbz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gfdokpdpy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gymwpaupn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gvfnasaej.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gmvfoenil.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gkimttjgl.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/golbjabwc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gzlqfnpjy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gyepuwvat.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gciwqxemh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gniwxoyju.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gwjjhfszs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gehkmuzna.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gmkrpwuvx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfwuvlelb.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gxfhkfrpd.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gcgfruqiw.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gdqzmkhfa.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gccqndrca.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/ghlfvlqou.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/glacfjjss.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gffgqigpw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gwiiqmnzf.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gksxiioxf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gpvrhkhkp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/grsdknreu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/glcqgmtux.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/geazlmihu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gtcbiokiv.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gfrufktjj.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gbmcpatzz.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gpseqnqss.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/ggyomwxtx.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gnaicflmt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmlansdz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gwzhcixbx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gdnbdkxna.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gvvjjbxid.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/glhchfsip.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gaywbgzma.sHtML


<!-- 参考信息 -->