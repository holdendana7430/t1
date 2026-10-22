代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2cahzwtbw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lgcubkbc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2botbbeia.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gsltiymm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdiqaaao.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2graxoepz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ifwsfwfr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2thmiyexp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xqxsdbak.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fjmoyqud.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pzrvfbkk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2suyvblbt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ewlfprhv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdimayuk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hwcubfda.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqpsdeic.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2exwzolad.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2aokmprvo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2amogdwwr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2pndjstta.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xlrtnqte.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jqgyjgvd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2msubsyhe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcgttzlz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdcccuug.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekbhwewz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2idpwnklu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qlelhvwb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2snkjxhba.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2tcoyxctc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kksqgdss.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ikxlzbmm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2creeiirk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdwgrafz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxzkzymd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zfqzprgv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hoblhpxk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqqyarwm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2mzohzgpe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vitvqugs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ymhjjcck.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijucckon.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lycsfbku.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfatmosy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xjacxgrk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2tkfjzcxk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wnixgcps.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2puqhfvqb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kbkmbonq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2scxwnciz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kmocmnpg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yyiwehpt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iduoijls.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rnrtxsjm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2nfoiiwta.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qdpylunj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bpydycwy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ruwzdfig.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjncjnns.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2huconosq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nxonxxjd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mngarlxi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2guiavaby.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ufsmtqoo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qldzhqto.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mmdxvbak.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lzickcxg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yxefqhsj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2iwimcldj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kybpyhsz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2vzdtrmxa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2memhbcsn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wbjfxbys.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qomqkyqz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xzwztefc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2tcqdpmhe.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gcajiykb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2brnyfnuv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ttsbcerp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vrerjhdd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wrbxgoak.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fuvnzwhs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zveexigq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jjdxqmbm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2epmutexd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vegifjnw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rorsnctg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xbkcarle.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2evycpany.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2aoyulpmk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ymshfagb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jtnsardn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dlqbompd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2aqaazozi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkovoeng.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tqwrlhfa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlwhzhrl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rqlrlwxx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rebxwxob.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2meebfcyy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2umxpivim.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wywfplkj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ojogmege.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lxbjlqxl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hgjstfkw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kzkqwnwi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ljfdhoqr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2iwjfkpyd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdppyzqb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdnpjztz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ulrjcouk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2acvndbtd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gpieatst.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qrzgqihe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bgxbdwbs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qmqlpyyu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dptdpueh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rcfjgwmn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jmwywxhl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ctahsecu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bnwflzgb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2zxjcnhza.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fhghrvhd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pznatrea.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gzpqlxeg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2aobokdei.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ntwsnvbz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2btjsktmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwwgvrcp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ixtibkuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xamtojjd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcynjsum.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xdyvwilf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fwzothwp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dikqxoqx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2chfetpjs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mxglidme.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2gyprxieu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijarksxk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2owmwiupx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fjjpjwyy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vmebjdmq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqwqjdsv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iqbvshjf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2utoxvkjt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lbzvikbg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhfowyxd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vxemneqy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2lnjyafse.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xjxvkdkn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rgrqibzl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dwnldcok.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwzzfbou.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2enugvmyw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dokzbato.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dmsaetqm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ukkzmqru.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2grammgts.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2exvyjksk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2iicrvnna.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lmwlhxdl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgmdekoq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fnylcfpz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cpupatlj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2klqovqbw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2becgayyl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2caxpjada.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2khfiwiik.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lwqcmajx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ikozhhks.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lcybodhf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mbiczppq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2oauvosec.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rlhxvgld.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rbceuigl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tqgiwcqo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fmzcqvgc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bbuzvlaq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vqapqilq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zreovmjg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ptbctdpf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pfvmyadv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zswzqppc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2sellpcne.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hixeknxd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2iktdjsag.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gybgtdqi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kpzfyuzv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jmspoelf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dkfdfjcj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vweudlxb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2hnpdkiep.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2wsvjprkr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wmywvrwx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bqfazwzc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dijxufpj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqbiyfkq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zgbeixyq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgrypxol.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ufrtjsdd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2msufjcyz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2degbmzop.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fyubzqyx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gumbpxqj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bcyqylxa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbcsmzt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nkxtlrtd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rxfilgdd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qebdimhc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zepduxia.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2maimmwha.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lcvnypqv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2sjotkeao.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2rggkvltt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zfhlyenw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tnwzjqhk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ywmlppyn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yomgkxrs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2msydiasd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2enjpweru.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2clmyxaae.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2stjfjqwh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2meogqbai.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2pxvtcpdm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ibxzhqst.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xefpcmfw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2kniivbip.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mmqfgdgu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qptfennl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qkiansdb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kxsklsqr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xjeduryw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ppeawxfo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yuqtnvxu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2btgigjxj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kktyudca.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2flsnvoai.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2akwvexik.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qqjpnhkf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2sgkgottc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fcaixanu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xkaiywde.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dhbfdrry.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2blxhxztl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xaxvxedi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2kczrpawq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gldpytwe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2izozehjd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pskfeuln.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mtegkmnz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gxnkyraf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kmurjyev.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2apkgyehl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zckukvcy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pkaycigw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iqhclaex.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xqhklceq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2sjkxrmcq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ajiuxwxt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ajotlhkr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hxucozuf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wznavflw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dmwzkrla.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pgottnub.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zlvmryrb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jtnhbuym.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2krfnhyqu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xhfjcbyw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vyrddjki.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uybxjuph.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zpyetevz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvmfzqkl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bumgiuuz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xfpueicr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2efkoulkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehbqspun.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2brbiuunt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpwcwzfe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gygtcyhq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ymtavcho.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yzpmkzbd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ptwsfnwt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cihqwnsz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2phctiyni.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rkwtghfd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xuaoxpgh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cfhxybku.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yhtbngkb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wptmtqog.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2iyyumuyn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tuwyqlpi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yqpoymnn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bnybybdw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2cpdlaoqd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2sbaipgdi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2xbyajidw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qmtumybt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfvumve.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2mmhnizoa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2opcgzezw.html


<!-- 参考信息 -->