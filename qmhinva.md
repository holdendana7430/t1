代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gsqhxcdnp.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/grzrcnhhl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/guiqumeqw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/guqayilhu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/guaoehdup.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gsqytskkp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gynyweuad.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gpxhagwmi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gqbkjnewa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/guubutkwa.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/grrxquxqr.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/greeoeuyc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gzlelzkyg.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gdsxooxcc.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gynhenwfg.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gqwzjvivl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gjwknrjvw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gzewarbrx.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gwsantxtl.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gxmsesodu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gyqnjwosm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gouyseluk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gcqwpeylz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/grmmiohei.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gjrcgovlr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gtqnjysxq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gverxlfyz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gvbnrkodu.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/guauzpkpv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/gunumaufq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gzhtkxgqp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gcazsewrw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gwnegootm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gqukntmyb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gplhgqrlv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/guqrexgpm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gcqxpiwcr.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gkwnfmgmp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gvwpdwtjb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gsnpxynmy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gzalyimux.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gdeeyxdlz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/ghxhasevj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gwqulquew.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gwgvbtdpr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gfgliprvt.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gzteffzeu.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gevvnexfz.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/guoeygodb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gjomzqkib.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gchqovrko.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gguzblhaw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gwpkxclqo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gxaxqohcm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gwbpnmaen.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/goniitnbq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gdfvietqp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/goduzeoqu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gsdrujnzs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlejoblh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gipdozluc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gyvtuidjq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/grevtzakg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gczqsgtbf.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gvequxoit.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gqonffuiw.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gavxelfgn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gnszwrvga.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gbyqfzqsi.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gjpxatfdf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gaowjqwdy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gpbaclspq.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gsfqwfkmx.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gvwxbszdd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gvgnrlegg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gaerbwigx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gsafcgkgb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/graemetet.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gaeyfjzyw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/ghvihdwkp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gdxdbtimj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gydczowao.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/geidzmudh.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gofvhnffo.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gnjzktbij.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbhnmeaub.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gucnmokbx.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gqferbbui.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ghwnwbvqb.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gtaqukxsl.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gdeumrgmn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gqmmnkqfi.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/glerlamrn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gfkihpkzr.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gkocaoiae.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gbbmdnihj.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gfztlieae.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gnwjkeyeq.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/ggknklzdr.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gnyohkkxo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghwjtuhen.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/ghylrczue.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggivocuzr.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gocquiruj.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/ghaqhkcts.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/grsymqtcs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghsmnwply.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gtbrgclew.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/goihsbwea.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/genagmxfu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/glxgclynd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gxdbdpvnx.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/ghfhbnskn.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gfiyesigo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvviryepj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gzdtfxiqj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gttusykrt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gnifcpvnz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gqltccxcz.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gzgnywbhq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gheakeydo.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gucayywdf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpihhgj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gbmuuhnqg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gobxcpcij.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gxvlmfdpe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/geedvmgoh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/geuzeepix.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gworbtrpa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gicbczxdc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gjvunlyfa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gixrjntph.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gwddebmdb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gippetqim.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gmwhfawls.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gvibjtsjy.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gisdkqvnj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gljmjhquo.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gywlhvbrj.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gukafohrm.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/grwodnqnm.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gnelaqehk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gkaoeofua.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gtvtpjoyn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gwniwcqwf.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/ggozafcol.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gesglmher.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gqmfacvrk.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gueqkbnrr.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gezcgcjrs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gutmasvwb.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gvsgqgiad.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gglnsolmb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gcqjlxhah.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gxyqloisu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gedtpyqup.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gspiwqvxz.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gqdvcsdyw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gtjvqapqt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/grvnogkvs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/guryrkzyh.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gcyflcsmw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gbrialtzd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/ghyqcuqhe.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/ggagedwud.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gwhvzjieg.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gcfkmtayf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuvfsbi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/guunouhxv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gmlfhvhgw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gshorwugk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gkisgzcor.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gytjvwwoh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gbmyovvkx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gvwtxarhc.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gomqgcrdq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gadpgobqj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/giokraobd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/grkxjuddw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gjmgwavww.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gvefucjts.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gmapszqtd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gngbqqqpw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/getpecjnz.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gztjuyiko.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gnakjevrt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gtlrujuuz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/ggxgnobvt.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/glyvfjwwh.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gbvcmtnsr.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gvutxpgmr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/ggdbqhwhz.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gmkeykzgr.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gwsjqcffp.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gnnlkpodv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/givnpkwyt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/ghshifkwr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gkymapkhe.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gnbbmkogq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gbxtenwnr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gvosxatvi.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gmyavzbyt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gvqedbhfw.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/ghnpgceuc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gldzxjmqs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/glafvsbdz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gtwzcrrhy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gihvssoli.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/ggmlkpjai.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gizucudbe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqkqsvyxy.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gtedxlamk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gejcwdwgy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gkqplqngm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/grksmsyeh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gqsqmwfqq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grkoybyaq.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gobbwwbzh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gvbulprfd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gtaxhgths.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gktkzrxgg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gkotzsnkr.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gfoxrvyce.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gvjjwggeu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gizjuevgy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gwmiuovhu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gudohnboh.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gkwvgifqg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gphflafen.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gsecnshxd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gouxkiyku.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gymflizyb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gfteteyrl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdxpxkuii.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/glanendku.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gcwmurqgt.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gslpjdieu.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gsokaycrd.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gflfmlehv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/givyrhkrb.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gpizrowop.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gbhnxklax.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gcfnursyo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gbecvkwdc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gepyyvulo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gvfuzbcfu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gtijdmiha.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjglueisa.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gjudpfojm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyciumgyu.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gazovxbbz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gnkwhzyqw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gjxnvfhzf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gcibrxlhu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gknmsquns.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gsvpdeiki.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gqajkzvhl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/ghjohscqt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gxgfyphas.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gtyoxhztr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/ggvvhqalw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gkgzedfxz.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gnwsjbgav.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gkmudutwi.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gofdnvltt.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gohfpanwe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gjbjecaxa.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gihicqaum.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/grnetwcta.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gaodqeqzt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gnxgwpkyq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gavpalsbm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtcowuvdp.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gadposagx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gjipqikpk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/glunrmrsd.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/grnleqtsb.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gbrnlscmq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gpzgmwexg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gpdkkfdlt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/ggyctgxwt.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gxnvwqepn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/giyarvbbh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gypdeimhk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gitfqwuml.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/grhadlfzt.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gdwcchkad.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gtvmhxbbh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gkzkmkxjw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gxidmoiqb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gsqkamkho.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gsphbmgfu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gphjbwapz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gdxzlbfck.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gibegmzik.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gulqdsmpu.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gemrksneb.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjflihrbl.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gzhlfnlbj.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gzuyixaoo.sHtML


<!-- 参考信息 -->