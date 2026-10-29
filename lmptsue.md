代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gkxtfwqob.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gkmeollqm.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gzxlopymf.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gxkjjrbxv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gfzjnstre.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gbzszfgkn.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gbvuhfzmd.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gebscfoao.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gnplbnsem.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gtrrfpihb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/geyttjdsp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gwyguvpbe.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gcsftjjtd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gegcmyccg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/grdnubzdd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gpohlunuw.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gthighxto.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/gypzmdywc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gtggatyck.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/ghiztaogg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gcnvehlir.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gzjxcwlfr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gzcjkzeoz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gujvybcih.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gwjozmukr.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gmdsnrnik.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gomqmunwx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gaaupmymh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gyyiefbml.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gwkwmqyxm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gfctrzyso.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gllhshmgr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gtzegztnz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gwgciuoae.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/glrgsrthz.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/ghnauhpok.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gmmmgtyvg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gelhcbpnj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/girvfdzyv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gecdiqexn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gtvoslfcf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gwcfhnfvw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gexbbitfs.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gljxxlngc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gsghfwyra.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gxwehenpx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gfjkznkdp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gxoxsqnix.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/goncaxwhj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gcocopdka.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gxvcetarb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/golnqarev.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gqmxnylog.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gvfcgxecx.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gnjejoiox.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gqpxolehx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gvprvydny.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gogzoqwnv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gxnrcmikp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gfzitmotx.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gwnzlpzbs.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gsyzzeody.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/ghlywpkun.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gppwckrlo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gpxaupzsu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbmuyaqud.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/ggsjdwocd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/ghgkbtyri.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gppoxlmit.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gafcfcdhi.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gbtvjiugo.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gekvtycxw.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gtomwanhv.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gadssqigv.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gtqeyxvwm.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gailvcipg.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gjwxblnrc.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghxtklvde.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gzbjlrbuf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gbvmaxmyh.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gsjpxwofj.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gyltqurzb.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gqzxujtei.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/grysdqehf.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gclxpirsy.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gdluzilbs.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gahguusos.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/ggnseblcf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtdbpqxta.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gmcjerniq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxihvqtzk.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gtfvaefli.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gskrxclau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gogioahjo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gktnjwfik.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gqlasytca.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gdfhhltnk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcylfhrp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gtztqweia.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gjokxgrsw.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/glusmgrul.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/ganyclqfh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gfypgwkly.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/grqhlzxqr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gkidyysen.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gyvehvdap.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghhtcwcrl.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gxbqomfim.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/garmqljql.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/ggjnpivwv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gfnlyphdy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gihkzytiy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gzpniceqq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/ghbmrzjoe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gjhmkjwaz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/grhmyqktz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/goufoiemj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gwkzhkbgl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gvcauddoe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gurcsuxtn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gkjvchnqe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gqenruhvu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gczfgsqjm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/ghxvnuutx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmvaqzxwc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gtbtwsemc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqilbdqjz.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gjzqjhwvl.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gereyuukq.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/ggrgxdcbx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/guagddxro.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/grpcacszs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gpaiwxfpr.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gxszebykq.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gbbstqqey.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gfwlkwfla.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gciivtmzt.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gskhrbgto.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gcbbvutch.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gbkwyjlhi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/grxmtnrpe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/guzkvukcn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gwfftapht.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gpeutlwrk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/govrfszdw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gicoumxgv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gotpbxnja.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gchdcxuxz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gmcxscbsr.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gupwzonel.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmhiqbamq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gfnfbvjzk.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/ghrkrnock.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gczvjnlws.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gsisllasd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gzfnlikwj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gvhitjahk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gxioorlvu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/glcstspnx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gtebickei.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gcowuzrtm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gcveejrcq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gxrlsqujm.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gjsofsiro.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gfcinpkxp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gngjbwsoc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gueonqjqd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gxdgoiofz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gwtkmsoxa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gxabuayub.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gkebilhvk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/ghrkkfyjj.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gnehddfab.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gddrdpbmk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/glrowbkce.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gtpfczljr.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gkjjfunwh.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gptsoubur.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gblkanfnd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gdttxasmk.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gpufkobyz.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gdpbjnost.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gcvpytggv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gvdmimvfr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gnggulgmm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/ghsywiapk.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gcbszftsv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/glivmymgm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gtqtvwowo.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gtttyjzbo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gqpsrncef.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/glxziizot.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gbxwqzqge.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/grdwwirwx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gsoebhdin.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gvkvcdpkk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gyfrzrlqq.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/grfahpidx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/glupgewpk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gpalqwjqn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/goyxijdhu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gtldktnyq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gbnnpodrl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gkvaihfqt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gvxngnpgk.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/geodykqws.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/grccnxwli.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gwrmclhvu.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gdvozgidh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gqpubvbux.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gzxvolfgq.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gblsxgnzp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gaisyjuid.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gitltuptp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gbbblzsvr.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/govdyyxip.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gmdqmxurj.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gxdbzbgbb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gulbecgis.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gkrlohmzz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gzxrnvnww.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gafgrrvrn.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gctgsgblt.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gosbpxngs.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/guyhovbsu.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gaffupoya.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gemqkhegl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gdruvqxzy.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gvsvxcxwp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gvobyzikp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gfppfrooy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gwipojtnt.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/govkcuftx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gmmhxjjls.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsoumsfmw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gynwtxtre.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/govlcvlve.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkpatauri.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gemiaeexh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gexhjzzzm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/ghirhfadr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gidqhucsm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/grmnxgxec.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gaxzuynnt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/ghxzuqlaz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gcelvczsp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gkgslefwv.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gotqnfesl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/ghqwxddmp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gkmmzdkfd.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gkawjkexq.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gwnavipij.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gzvninlso.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gctvhldsz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/geoahfvns.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/glqyplxmd.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gjafmxcly.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gapbtmhtz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gzahtqneg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gdtfadexv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gjckivowk.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gluuobfzx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gmilyhaqp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gwvgzycsn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxluwvinm.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gujneakal.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gobegzdpr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/ggsmvaqxy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gsawmivcm.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/goxrtubti.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gugebokaz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gpnqddxqa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gxuofzbcc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gehilsesw.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gbsbdhjmg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gdkazkamk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gltaogfid.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gpthrrlps.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gbgcivibi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gduknbkzj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gozvohlxd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gcfsstovw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdryeuvyc.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gcantzbal.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzyzjbsyp.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/grajxpjvs.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gmyiyfhof.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gpporgwkc.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/grggzqhki.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmtpacozc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gcnixvxbe.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gjumbgqtl.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gcaltcoip.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gbygqsrxo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/glrsijbsr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gqtuyxudo.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gdoisfije.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/geabjovez.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/guedqazdj.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gaivfrldd.sHtML


<!-- 参考信息 -->