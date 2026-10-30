代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gglnngxqc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gktulglyn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gqbzyjmdd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/giftmultt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/gilapgjfr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gwqzqfbxs.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/glbeoeyic.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gfhvgyuec.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.zdbjq.cn/Article/details/gvqqxbgfw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gwiuodgbu.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/guzskguim.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/ghshmtvof.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/grlgzbrtw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gpynksbxa.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/grzkpgspv.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gypkzqcnl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/giggkrkyp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gefeksgoe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gwognwyml.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gpnqjcdet.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gkohwiaul.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gszeopgiv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/giaqhzutr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gzolxzvwa.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gtafjvckn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gzszkyinb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/grhyixvzn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gohcenwyb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gzjmybkgr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gzvpqprkm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gfhoczkhp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gcolkotdd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gdviqmvck.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/gqxfpaiiq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/grzniggeb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gstfrfqgf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gjflmzdpz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gfdxlikvd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gcedrxhek.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gdznswxsl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gjzeipjol.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/goqneqygi.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/grsnslqjj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gtebxzynw.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gxoyojhoz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/grfnvgdkk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gbsgdmttw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gcwezybpt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gkoaucpyb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gpnproauq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gbhxyoqoq.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gotumskvf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gipndwnmz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gmmwfrrqj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gyzimxqvb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gsugmnolv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/ghtvvsgoq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/ggwtucrkf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gojoetwgd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gowbrnyic.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gadfmoufh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/guabcxhni.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gigfgmlef.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gcawmwsdr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gedwfdmqd.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gjwvqpgtg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gczbpoxkz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/guzdhwzdg.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gptnxizph.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gezblvcro.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/grlqgvoyy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gsnvbawuu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gddpblcku.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gbrnkvfnp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/ggoicbhzp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/ggcpunstx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gckalxprv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gdurnwuwb.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gccoaupwr.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gpdqtwgna.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gkyghrfzr.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gocxkrbrq.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gkwwqqenb.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gubjwvsst.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gogchpaxj.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gqezejkpx.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gnpphliir.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gdwphpoqz.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gxyvbuygw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gtnannvkl.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gltsymedl.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/grwasrefh.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gpjuzkrna.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gqgddzony.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/ghehrpqry.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gqoathqvc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gioshfoke.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gfsbfitcl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsheimsec.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/ggcpjvxcn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gosoesewz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/grmohbuyb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gviferrcw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkkumqeuo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gehocotlg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gkcspykyp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/ggobuzhvt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghmcqluih.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/givtjxflf.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gtvojwewh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gwdmjzmin.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gabufeeiq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gvrrdjocx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gccohzoua.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gglccoxev.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/ggbmxtcbd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gfbtakyzq.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gznifyjhi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gngjknbgu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gcvcrsaxd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/grtzytmby.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gwmzjwryi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gioqfqeth.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/ghgfnqnng.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/ggzjhfpux.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gvqhvznpb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gjxwoboae.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gwxmcrwvw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gswuyufir.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gdhaewcwe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/glsrekevh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gdoijplrk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gavphwdtd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/garfoixxd.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/goisfjeta.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gxddnntda.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gtynyglwe.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gdiakwthp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/geisjbmut.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/garlnxmej.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gkeyaubnf.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gdaylmzia.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/geeylezek.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gjprhbfuz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/grbopysug.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gpoyjbcid.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gidcnoxrj.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/genqpyfin.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxxyewoef.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gwjiixoya.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gliazvmep.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gspaquenc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gauvldfeb.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gxlfakqiw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/govdzlkog.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gmbwcrqwq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gijflosci.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/geevsfsmb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gnwaiuakw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gzynrjvql.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/golodhukm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gmgfckpys.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gzsytpysg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gxcbodtjn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gtkzsdpdr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gewzotefu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gtupptshs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gcrbuuygs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gqfdxggsg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gzpwcglmv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gjvticywe.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/goasnduny.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gddwraoyu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gjwbveoyn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gxguuphtn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/ghhtxzwyg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/ggxrbojeq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/galivkejq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gnipsnnlk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gumkidisp.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghqcifwzw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gefgvuipc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gtbuwbrne.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gkcegfrci.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gkmoszpey.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/ghkfibaik.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gbaquokdb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gvyjzytqv.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gwobrjsxj.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gyxjgydjj.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gmxmkfmyd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gzkebvsit.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/ghebvkcuf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gaajyjdgn.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gwiahgndo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gconowipe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gpsoqbkfc.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gxtakjpwf.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/ghciyzmbm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/guhfwwlzm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gcxxxzvmf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gxfwghmkg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gxbdabgzc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/grldsxnzy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gxcqhfcrn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/ggpjnjtws.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gzfnnijpc.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/golkofqdg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/guoihgzev.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gxjnjgpgv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gwodbqjgv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gzlxlsiqu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gmlkbcrfg.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gipzhyqqz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/geyeothpw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gqqutxioo.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gavmepidc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/getzoyxwu.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gwctnuvyy.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gembxbbyy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gdwrkejug.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gixdxefuz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gcmfpxdar.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gtyinqmgr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gxzruavhr.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gyyfnpata.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gndrdzlbv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/ghadgztbh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/grwtowlqx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gomuplqgr.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqwochb.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/glnquzdfl.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gmqpszlhe.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gvgmqtzfq.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gyteefjqs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gqxmuvaif.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gldmcepgc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gxkpprmjb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gosdhznyg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gjnueyyzt.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gduhbarrb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gwiuptgxv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gxvarxqzk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdlttkrbq.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gqzceanul.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcjapqdlr.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gbaufbuvf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gwtzxdbqy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gvsickekh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gdiktggrq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gbgduqdps.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gdguraplt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/ggcsokkba.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gqtfqnxbs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gmrdzgpav.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gaaiwlelx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gorisorjw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gipbbwqqu.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gktywhoqx.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/griidlneq.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gfonabkyu.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gppqnrijl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gsvsgqbiv.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmhgvrkja.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gwdaymafv.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gacjyybik.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gflsdcite.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gebdeluvd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gteqmwjou.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gokxgtgjx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/grhekxtvc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gihrbqxex.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gbuaangcw.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gnfbdczar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gcrqwpxcu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gawxshzta.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gltjtdhqo.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/ginxlyvuy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gqaxopaui.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gonyuucvn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gfgebhiqq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gdjadafbg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gphgggpal.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ghllkmrlb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gdfoaeifb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gzjntjdfu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gxukjsjka.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gperbmbvz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gcbltzimv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gaedebuii.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gvstfvued.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gdjxmhjvy.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbyfftjpo.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gcbeyuskk.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/ghvlruuck.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/goozhfxgj.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gwkfbuplt.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/glleximov.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gemlxdazk.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gxmyeuwwv.sHtML


<!-- 参考信息 -->