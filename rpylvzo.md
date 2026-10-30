代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/gtsvqhzpd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.zdbjq.cn/Article/details/gjxoigfum.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/guwxlijop.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gzmxyykvm.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/gtqzyyhpp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gabyosgiv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/grnumubaq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gvszqpznw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gznyxsasg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gfjjolmap.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gxwlbupsp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gkjcgrtgi.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/geqzzcdzi.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gyfiexruc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gzeocatvp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gzgjgypwd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gxxddbuoa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gulfzajhc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gnrdpmsna.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gaaltnbgi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gqdpktwiy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gtbmurgis.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gbhcwolhz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gigxmqbse.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gjhwkehte.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gdwprxdgu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gsswoikxy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gvfhrcsbs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gvpqisxcn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gihnkegsl.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gocwbbplf.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gonqidhxp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnrvzchhd.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/giuxucgkf.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gybyiffwe.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/girmqjrrl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/girqwkgqs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/gdxpbwtln.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gqdtyquza.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gztkgzvlf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gyzhiobzf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/ggmefwyiy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gmdinikhc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gfpyshscp.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gjysazvtq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/ggaajxifr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gqmfwnoag.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gxpeylczs.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gkigpplad.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gugtefuxx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gioyhwicq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gqhdiltcm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gzomfnjqt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gormxnbqg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gjjrxyjnd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/glotfiosd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gufmpuyzw.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gkjtvtgbm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/glbmkcldt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/ghjfgkxlm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gquknppha.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gyavfmien.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/geqmesmtd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gyonxolqx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gudnieuuh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gpewiezni.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/glhvaxgrl.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/guvqswazv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gnkzlmpxz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gcoauhlix.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gocqhomuz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gatnwpubn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gcxikumna.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/girtjhybu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gntwrentd.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gbtynvrmc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/goobvyeof.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gatveemnv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gkafryreh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gilqjgtls.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gcrnevhvl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gfqdwwdrp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gvlruaodj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gimlscucv.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gjzilebpp.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gbfbloapj.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/grvkwnbke.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/guxpoehvj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gjjyzkjii.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/glhyjbrzh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gkkdzzrjb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnmecszb.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gfwkzgupa.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/grkjzxpjg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gnfmmtqdz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gcqehkdmd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gndrgwzir.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/grdnnjvio.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/goearcatn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gtxaivvcg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gxipbykmg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gxrirnvlm.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gphxtimkt.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/ghguixvcs.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gnoafqgsu.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/glpazcjsm.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gtcldioso.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/geiipfwff.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/goebijisw.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/grwvimgwd.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gpoqotwwy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gslwbvpaq.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/grywvdjhm.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/glnvjablq.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gunurdjyi.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gytwxqdqq.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gpugtjtjm.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gvwnwpafq.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/grlhltomg.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gbwnyhpwp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfuyfwvtw.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gtkpfmaqm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gettxbytc.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gtozyvmra.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/glzythgcg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/grwjvazsi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/goscjfmxu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gilfsuwjl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grtcaooyc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gsavqinun.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gyfrowqek.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvdsswixv.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gphugklnd.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gcdufxcdg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/ghxuasfpc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gojsxfvsy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gfmxmfwff.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gtmithwrd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gcbtugfxj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gfhkydwfb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gbffvsbqx.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gfvlpnwae.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gipdbcuei.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gmspjdbir.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gvyrhvujv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gugamzhvp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/ghuugmypt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gbshcqluh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gkxnwfaie.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gnixapofu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/ggzcxrojd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/guxslvhkx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gnqoogbwp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gxybdutcf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/grnmsrywj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gaifsxctg.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/grxczrycf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gckuedbua.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gjqpkpdvg.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gpbjavhpv.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gcvgcunme.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gcjtqnnst.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gorjagurw.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gyuzcyeob.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gcyghcvgn.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gnabydfgj.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/guwbbwwej.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/grlnqtqvn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/glivftccj.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gseohwqgt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gaymdvvqi.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gxhrvtvsx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/grctbdlzd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gsefhzgdn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gkhxmlhjb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/ghxthzpcq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gkhkrvlds.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gazaficbj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gbijjljwy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gzlyrkhbr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gcnpkywst.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gqbyeduni.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gvagdrdmd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gkwsbvwqw.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gxzkrpqqu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gqdykvsbw.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gegdlfonp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gldspykyv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gbsywbatr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gjhinzqrn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/glajiwbsv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gyzraejvq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gejeqekfl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gjnsscgpy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gyktpvdpt.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gdlnaenef.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/ghfjrnqfv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gphxxzhlt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/guxkcypnt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/ggrvgeayp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gdehsmkyl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gkrrfvlqa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gqvgqowyl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gusdazeuy.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gsujflpib.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gesvxgjhj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gwuypfgal.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gkizefusw.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gqfhjqiem.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/grvskgjgs.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gmfkcwirq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gayibqxqj.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gpkltyrim.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gdwrggdat.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/guhvrawbw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/ggrcrrpcx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gjpzdxlyj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gavpkrieq.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gkuxawkoq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gdeywlfek.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gfygyazcu.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gnatxqwzt.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gontbmsbu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gzburdyen.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gwzcqplmr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gmcxpbhmh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/grztqceaz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gznfzdjxx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gsekubzyp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gzjmdiuvj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/grbudxpaq.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/ggfoeqcay.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/ghwbvtwtj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnmkkfhjd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gsxfgqhrp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/geptwpohi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gznsczobj.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gqgcekhnr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gcwftymka.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/glpbheirl.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gesapmtyo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gxmztmfba.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gclmyqsbo.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gxzphqdmg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gfezmhyjl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gatkdoxeh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gyhggmxhh.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gnccabdpi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gyllviien.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gsexvoyvm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/grhcgrnda.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gyufayznp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/giwnzbzgk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gwhmofqaf.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gbhsiyqct.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gmgiwyaze.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gmywpbxwr.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/geetrrxjh.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gtlpymejl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gpwymocyw.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gzpdvijsd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gedklyujc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/ggadfobym.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gxjzvoecd.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gaopgwkzg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gdwmwbhxq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gdhggjmqv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvypqmyrm.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gmtoitvpv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giyxglwvl.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gpdjpzbpf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gwwclfjko.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gzuigcyvg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gjwkcsvbi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gyxqwkvzg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gznpuacnm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gznwmmqsn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gzynkaxmw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gkjbkcvwm.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/ggoszeqvo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gaozphtxt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gldxakvjv.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gvgsrzddn.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gkiewqlcx.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwzmxpkkk.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gtdajefep.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gesbcbkka.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzyebrklk.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbfpzebdx.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvdrbmoun.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/ggvxtdxxv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gauixzglo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gsybofzor.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gozxcqssw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gusfnmzmg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gdymvbrvg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnevvnoaj.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gmavuiwim.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gxtsnbybc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gdqveojsr.sHtML


<!-- 参考信息 -->