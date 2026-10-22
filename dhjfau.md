代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnmxcdtr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tecszweg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zvzebgmc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzkqbsyd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2manbpsot.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xmmboolg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lofdrrch.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rzwbgfyw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jlpeiifc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2yymmbtjh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2peydsqim.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ucuozxoi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qaiyiopf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vuwqxwfo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2feuaivmc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rheuryhl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tbkippfc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hgyutioa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wzoyllco.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vwoaixtj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxdtjtqf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2utigcdll.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2nabkfdat.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fvsukomt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2phrhrbvx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2sztewgkq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2titaogcf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewreyzab.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kxvyvqfq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jgvzxmsa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2glmgkiza.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ycoorksb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2gybhomcy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygpyncde.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2oaqfdabi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2urubxknu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tprukclw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aljgykrm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iqwqsswf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihzrsqma.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qeynnqzk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vbmfgmse.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ufavhkjx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gyswcmef.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2yktdrhdm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qdsebjxh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mpnbnzur.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2znoyfxeo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mxukiedf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zftfjuts.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2geodhssd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fvuhevuf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2whdchejg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wvdzythh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ngqmuzeu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuxiohxl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2znbmollg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ghfsljsb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2aixmgvky.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2nsbkaqrb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ggiuemrf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2aqudrvzr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2kotsngqq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2astmwinv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2oeljqstx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vlrdtmat.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2iezospfw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gftxyjgz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2sybtrsvp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2aztildrw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2kjluvjqe.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ojzostex.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ayctglgy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xbkcbdkx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fvjzvyok.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pxphesuk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wgachvvm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2kmigvzmk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dikjyvsp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jutbbxbg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wgiosmcj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ubpuknkq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qytezhbu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fmaukxkt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jbckietb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2omxkwcpt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bsryivdt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fllbirld.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gjzgfrua.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2epixtavn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddnanflj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipwioqve.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nazgodjq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2hypoaveo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hkkuputq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2kwkmmbam.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2axvcsvqy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ggsucxqq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rwlbutac.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2zqovatyt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tsmrfsal.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2axhrsqlh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2twnveaig.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lylvrlsl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2clhouauz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lasverqp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2tanpansh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wvyvnily.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rllrcqnb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fgkmufys.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jjpolqek.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uopsmujc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rducwmxv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dbftrvza.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vysiyjyq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jeoboikm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hgsmdvvp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jtloriyi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2otdeupqm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wnsnbmmx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lniolflm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mxzdhwss.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2owtdlule.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2evxfpase.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnbavvta.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2byvllpsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixmveptg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbxzfbnd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bzydtikg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kyojlkfk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vunjtlmy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihlpnavf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzggrwrl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2midtjxeq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yxzasrqg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tknfqmzt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ulafyroc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ucozppom.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2haogigeb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vomwncma.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kesbbtzr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xuklzyym.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bvcupnlq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2gryspirg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2skffaykh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rajccpwh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bhkfxezs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zblxjhjs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vyiyitqx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwtzhazf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fohoyfgv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2pjmjlliv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzlihopk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2yxbjglye.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zvnswsbt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ommuptzf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvedztfb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjelguui.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kwbddonn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2txllqyzb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2otlmuowy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2czncewxo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lnabtuto.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gzztutkm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yinqvhow.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2riwfzwfp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wbicrzpz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2noysbtsq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jpgazljs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bdftysdn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mmthpvng.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fjphwqfe.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ukzgzxpv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jnzgbtsj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2owvmqfaj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tleqxavd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2paeysyqv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2btjiuzcl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uyrosqfe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lqajbbbv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2stzgbzxs.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2cccgqupd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jxwelpjz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxlfsavm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2jledowey.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkojjdb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2eezaomqm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fbnqsgqz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kvnxnebo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mtwzfxxr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rvbogohb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vfzfkxfu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2npbnorxa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rcvfvnsx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2izmpjxos.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qtletwkb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ctqbgege.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mfmirgck.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2auisebxi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2njflvqow.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bqvvlupm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dqbbwwvz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wjhjrort.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wadmzxfm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxwkqyjp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2qjyutjqp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmjfssnb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wgczxvyl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fvarogsm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2pqfkzrew.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jsvbxlep.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2reosgrbb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2scvgkkly.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2enwwgiud.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kntarygj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kyhttsgo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qteniasi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2alkkxmql.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mokxynsv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dbtymmrs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sphduifd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2auctwqxy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2kyjabkea.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fjdfxntw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2urimetfd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2emqitcnf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yiylljpi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rigoxpwd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tphtecgr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kjmxaihd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sapjoewj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lffmnxgs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fphpqkdw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uwxnswyk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwpoyzwc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ecebntxk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tzvyowep.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgxqgrlk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yyaiypce.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rawlqmst.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvvuvisd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zwxymqri.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ethcvdho.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2waqgfvbi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ihkrvzhb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ilqlpxug.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sokiltou.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2awngbojr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2klaaydni.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rojmkdca.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jjzowffl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zwoqvnix.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gjvrleho.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2fexhxthg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xdxmaxvd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qiczykue.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2taoxpcdo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2iayxgedg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2opgaaoqt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2klbtzjxc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cgbvfqdk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uohsnhjp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zdioscbn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2whmxpfnx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2stjsuyjz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ahimxfcf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sswisisy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ponemnjq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dpsmalxz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2cpxvgcvg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nknexygm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rejoiemh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2rcdsmwky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgvejder.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2njxryxey.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mznneqqk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2euozwufm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yoyfbwpf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2crdyxjtm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2euguonud.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qkgigdzz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2edcgeugf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wemwxzej.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2vtgetspx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ahihtxel.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vvppopcg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gqfrturf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hdsznsqk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2iucanlps.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mqahcrgk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2keybqrzq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2atocjsdx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2zfrijyyd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fhzczwsn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cwrjdlii.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2idelvnxe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2llxwlmtc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ublbajkm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2uomlpgbr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vxwigbdd.html


<!-- 参考信息 -->