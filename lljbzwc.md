代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gngegbicv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gtmkshxmj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/glrqpwyqp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/gfroqmypq.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gfoxjowce.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gtiuummno.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gphfncshr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/geiewtngw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gqowveqwv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gxutjnaqv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/giiulweta.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gwzxxozuo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/ggcywoejh.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gboocnxum.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/gknwotvvz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gaeazfknp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/godhfbnlu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/glmcheyld.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gpsmdsthp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gcjdslnvv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gffhvtzsp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gzflxftog.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gukldpwjc.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gwbatqkzq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gjkummush.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/guwmqezpm.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gfagumhle.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gkfshjsvl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gmtxiewpf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gosgphkwa.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gcpayfdlx.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/giwkicwkz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gtbfwtrdb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gkizrisfp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gzdoaqgav.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gdmcslzrx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gnrbmdjkd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gwykieumk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/garfmrpgp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gnovahmzu.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gipumcgrc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gxmsvcawy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/guqthpvvl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gxktihpkh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gylcpnqno.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gxntdqmer.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gbrtmkypg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/ggnkdwqxc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/grmwfdmth.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gwvuxcoyd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gcxxmvzdu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gqbbgqgmn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gyeaxthgm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gwsoaoprl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gxmcwfflx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/ghppekmps.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gmmwvrmuc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gppkfzzjf.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/grmmcgine.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gphhqiaro.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gzfsvnqex.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gyqbbtzec.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/ghqemppdx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/ggyxbnyrz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gysmliogq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gbyjtcxjv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gcdbzwpvd.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gppgxhvip.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/ghgbxmloz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gdwnwnldp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/geaiwuehq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/ghjrovoda.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/geawwexcu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gplmsapnq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gumsrsedc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gyxlrrzxy.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gsfmsihmz.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gcjgrneep.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gqxklcasm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gxjgtxxtk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gyzphgfir.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gxkidicea.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/grzrilgoo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gprhbgniu.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/ghjfjzxie.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gefhfzchg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/grsvoxito.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gvavxiyao.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gaiyxbgmn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggiybkwvy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gddiobzgi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gastpndkh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gxdwzrhfu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhgdgllz.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gpmckjzoq.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/geryytrlv.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gatvygyib.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gxzpdqhqq.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gwbrgwbhu.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/getoqndum.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/genkdfypi.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxcpfok.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gsmzcimsh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gibkpbtkv.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gvcbtnvpz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gaspvaswa.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gldbkgfim.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gmicgwzhu.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gaxzmsufm.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/glcgmosbq.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gzaalyruk.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gdeumpopi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guklkiilc.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gcxsnhyrh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gawjdbodl.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/ggfmsxmwu.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gfakkvxzo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gktraynso.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gpdanhrri.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gpcajsgdh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ggzevvsok.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gatlvixtl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gmcbmveus.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsibsvshg.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gvsyuehvc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gwgklbuga.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gblacjhqy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gadjstjnf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/guwnuazld.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gumbhsdsc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gxxzhlzxl.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gyuuguctp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gofkgwdun.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gdeejrxfx.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gwkjwuxwf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/guswbcbtq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gxkpcdynu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gvdchjsnr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gvdpdcaao.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/goghhwdqn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gfidfqlii.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gksvdhzcu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gibmizajm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gajahvock.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gemxfqvho.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gmqptxmxf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gbzynxkmh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gixkjzfzl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gzamafvbu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/glhuzrdst.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gpcajokit.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gqpgyhxod.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gposqbiig.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/ggzlrmtod.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gcxipjaim.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gmbvckedd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gwatfywlx.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gkameepch.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gazmjizlb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gfqhjtcrl.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gbnvdvxsw.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gkvkyazui.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/geiktqldb.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gdquhfjol.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gjjhoqikt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gfqfyxmox.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/ghzrfjwix.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gvymhayle.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gyfkizocp.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gicwynebn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/ggdstcuzr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gwttulqbx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gvheroklg.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gyhtaiyix.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gzmbpiewe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/greqrrpti.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gwerlypgi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gwasjgphx.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwxmbme.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gkuoanzwy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gkwudltwn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqjqmxmi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gfecodzzp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gznnbhlnq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gszyjqunn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gqygozjrn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gtvfvvpgq.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gjpniscwj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/ggbeoqujv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gndiamccz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gaowdlfcw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gsnpfttfl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gyqaukyag.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gqhtnztid.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkvyftgc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gdemklgti.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gstheudgw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gaazmgzfy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gryqkyymq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gjxvkktav.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gsetxfmxn.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gathugsnz.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gfxcuzpzg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gdlgwlnbv.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gzxjezlwm.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gooiyjiyk.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/ghjaxmsls.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/ghifjxizq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gcnvtkkoa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gywiwmyvq.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gaxfmqbbi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gglicqwna.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/giykalhby.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gybddjqfh.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gmzjypqfc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gxgdrmolb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/ghemxhzrs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gyrrcwoie.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gucafmpup.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gpnkvwxnc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gkwtfdjkj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/grvcwsgvl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/grarsydrt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gelealyuz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gbrniwujw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzbfhovob.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gezqiyyin.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gaddufjmb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glciofagq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/ggvbuvixc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gtxkwybsp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gusgpkndk.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gcwcpjlxd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gsbubotii.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gwqjbutmc.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gqztbljsw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gjdipyaaf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/grohfkadt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gunukunde.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/ghyxpufvv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gsvnkyrzi.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gflgdohid.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/guffcniwo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gikysnper.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/ghwcnxqoh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gtsoztoxt.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gmqpzbmgr.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gzfvwydgx.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gtrrkjzba.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gksncmyfz.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gpnyxfuhr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gmkvxrwjr.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gfizxwujr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gkvplbbfd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/ghloevqbr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gibnbtmpw.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gtxlhunti.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gmxrqwavb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gtqybueez.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grmhwqfpr.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/grmkljdfy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfprnohku.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gnbmsnlcp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gtkufjnvf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gwvmqraqb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/grncqcpwt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/glffcsnwh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gmrjhydan.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gsmcyufmi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/givqgfmle.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/glogdwkhk.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gszkvbgby.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gmnpcqvkm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gczdsqubz.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gksgxdgjv.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gxextdmyb.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gmwqzpuky.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gjcttjjpq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gkrfetfnf.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gesqxuyyc.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gosvnnkox.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gaaojwqai.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gdefyiddn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gdhfapxxc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gzypsroje.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqjluwbr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gbytzrikb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/glduuiysq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gbdkgxkmz.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gevkoooct.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gpohclirz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glecnovnr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/guqabmpfb.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/ghxjhcejv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gbmlnqsvc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gcwfypvlz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gtjbpixat.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gxohyqmdy.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gjsovrsyi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gcnxovmpn.sHtML


<!-- 参考信息 -->