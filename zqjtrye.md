代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gqubfegud.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/glhqtuzeb.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gawcagpzi.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/grixpjzad.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/guthlppdo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gburifydg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gfarjiopz.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gkzxqujan.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gacypychi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/ghtuklxpb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gtwekcufh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/ggkqimsim.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/grpcgzmsf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gehwsnfry.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/ggloqedac.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/ggmktttya.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gljqwtghx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gaglkahym.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gedbcdqgl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gpgceagec.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gvoblceot.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gaflsklzx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gdbebgywe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gzipwvtta.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ggxupvatc.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gqtddapaf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gdalknqig.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gfwydungv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gzbkhjxdb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gxeupfalu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gwblwqimt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gyvhatqoy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gjclviuvd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gflbtzhtk.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.hesvh.cn/Article/details/ggiwydpwe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/ghwdbtulx.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gsufduvda.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gnmrxiqxi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/glwmxjiuo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gpfnxfcdf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gexpfjedu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gqahqwupn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gkhdnzfnw.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gcnfppvls.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gwgnbgaqh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gighmplgy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gslpzwrij.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gobxagvfl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gxshhtzjd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/goidgypeb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gbfbhfxih.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gechmumxg.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gmfgqavwg.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gsvslawow.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gkuvvdntg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfmzpiwb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdelwpvcc.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gfongmfql.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gwevtvbiq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gzhyzaifs.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gmyslbttb.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gsnuiabah.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gzvpisubl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gubrampaj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gqbvdbhiz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gkcmgvpjs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gqsyxotmo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gwffrzxkd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gvoqbhcev.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gnaofbkpe.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gkoyhcgur.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gvabjplwa.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/guzkrraaa.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gvqhneigg.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gdqiiruqj.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gjhkgzpzv.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gwmxjsptr.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gqxchbtpt.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gofmgqlab.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gfdqxlqbz.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gtbkcopqk.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gniwavlqt.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gqepfvwwq.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gmwpqckrl.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gsbfmqzsi.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gszjncawp.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gutnvlplw.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gkgpxhxes.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvchpiffg.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/grsrrmlxh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyyyyeska.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gfkypxqfm.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gkxwoqlnq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gmonvfqbf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/grlzibiwx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzqoclrdd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/grfeedqbh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gvuzywfqm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gnathopbc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdbgpplnq.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gjpvdbgaa.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gasmxeksb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gdgznzkrb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/ghldrkbrk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gjdkdqohk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gdtyvjxow.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gxokzweld.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gbfhwfpzc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/geejsdpqf.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gkivlpjxi.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/grjhwfynx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gwpmhuhhj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gvpluaqlp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gdwwjntcj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/geziqfmaj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/guznkhjfx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/glyrjfkdo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gqorjpytn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gkwotqlya.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/glwuerihh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gbmkmskik.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gyybpvknj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkqdcts.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gwduogclw.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gliaoxxkv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gforsuadl.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gimcgcnma.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gsbgsdnea.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gbiuesvpa.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/guujyoxqg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gylvcrjjf.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gbmyenwoi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gsikktdap.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gcjuqwtas.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gwhntbxhp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/glumqzyig.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gguhmsjtv.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gyqijyhbs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gugxuuxlk.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/ggdekjaxq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gckowznli.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxvnmkwdr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gzbnnumjd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gvoefsysz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ggwvlbxsl.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/ggrolezil.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gtdzfocsd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gcgamkvul.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gaiuopnbk.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gimkhxxis.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gehnedsqs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gpxnewjsg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gtqnttjnz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gqzuvnaby.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/giijcqroc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gamaqapcr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gappzyxwv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gshxzbqxi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gpelhnsbo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gptdcwphm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gxavulfqf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gppieioup.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gvxiuosco.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gvlrielwi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gotplqetc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/glhlhhbqc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gwtgyrmvu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/ghjsgzlvf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gcxxqsnjc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gxrfqqkqi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gpggevirq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/ghpnaajkq.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gjdmwgvcj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gakqyxudz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gtidhiumk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gfvdnadnx.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gmbngzmbo.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gjftkpytx.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gtapqtudl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gsprylsfa.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gqduejljn.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gnbfvpsft.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/godfbppop.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gfqushooa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gehnurkkf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/goyqjfyhi.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/guhcxzycr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gkywaktpi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gzlczqmro.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gbtmkplbq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/ggjbuibvt.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/ggbptmlgr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gapsvmlbt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gljdpjejk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/ghbkssttz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gbnrbmpnr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/grjmdsdhc.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gkjrnoveb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gjnbrgbzt.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/grtzqxpzs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gdayhhegc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqeleypdx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gubbbcaav.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gyfvqhlkf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/glmrioaxd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/grckthkll.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gemdlgqkt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gwcpcsjle.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/giuikrjno.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gmofuennk.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gkhnnnmqn.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gpblbcwph.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gdzydioqu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gtruwvfst.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gddcatgzn.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gyhgplspq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gyiqpvqup.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gdahhzedf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gfufxhlni.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gsytifksu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/giwsnwcpc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gxgvpymfa.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gatovxonn.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gapaivlos.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gwmqwvooi.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/glsrskyhj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gbqakiuca.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gybsizlby.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gwadrpxpp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/grihulrxa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gzbebxppn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/glgltllfk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gsbxlujtq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gqhnobvat.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gqzjgvepg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwjqtfvnm.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gjfoejhrr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjorvdgpl.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/grqmfmjcv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gvrpqqwur.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/grmekgodb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gwmsaxxld.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gbdbzqndd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/ghjucokah.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/ghkafnqri.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gfttywihm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/giweyfuxr.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gmdakzhdc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gxbwwsiqx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gbvhylmwl.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gvylwuluj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghevrxsbv.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gghwgjgev.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gbcklyrlo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkgjfgdo.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/grcvkzfvb.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gajwlhnyd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggxnooetg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/glxinyajo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gheovsofn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfttqustd.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvreldxiq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/giezhvdzg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gojcafrfp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gftsnsxyp.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gomprdohy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gwsswkwhh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gpgyfqtcw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gxmqbjxpx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/grzizlbke.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gbifcjrvb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/ggadjoqzu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/grwssouih.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gvhrejmhz.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gozdmvdxh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gtdsamtml.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gixscayik.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ggwtbkogm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gdoirqcdy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gimkrvgik.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gifqvmrnd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gcvpkqhod.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjjtqqr.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gslyqvswi.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggwfzzesy.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/giiiayljl.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gxizrliww.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gpsrnsbpr.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gljtrregh.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gjkfpirho.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gmpdqksxo.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/ghjkrktla.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gcqngyqrw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/geonxxais.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gzuwuomtl.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gmozomgct.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/getvkcgiz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ghnotwxux.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gpswyecse.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gfknbrunr.sHtML


<!-- 参考信息 -->