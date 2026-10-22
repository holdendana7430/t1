代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2deoexbon.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kbufxclu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2cnlzlzpx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2kaiffgij.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mazxncqg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hbdekhql.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcuqexgb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhbjwkix.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2crecfpox.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kfocsvzq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mkphodxc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zgseidca.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qovfifen.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2royctjhm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nzrxfdmd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzhfslgi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnzclotp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uqriqgyc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2aflykpfm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2llqqubed.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2umhpzggs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2usoacjwp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2htdkcvac.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vuslgrhv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hhjekwfk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgxjyytz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ycwrzayr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xnyhdnui.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdefskvb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ccqvuebt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wehlgdgo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2bvmulwrs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rpavigap.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnhddzbv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cmaxuleu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mgfcbukg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dsohfery.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2eramojlz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ocodbxxt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqhwattq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2udybfkpl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2twlreekh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fkimltve.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzwvpyhy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2moyidega.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rbawmgub.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaejiwfv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nxxlrhtw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ismflrfv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yuogbudd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wbmbxwfs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hwuyemsl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cqcuqsmb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2icbnxqrx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qfduwysg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2evzunfre.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mhqebgid.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tumlaqus.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeftevfl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bijjgwga.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qpphbvex.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjqacbzf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ieuoltob.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fymhioqi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddzujyyr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2yhppbzvy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2tprcbnhz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2csfdauxp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dmbdjugc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dxbgkbhg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qqjfddio.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vqelvmtl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2phtfdwxo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eymgfwpy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2lxwjvcpi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gslvoqmd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rmzhgewe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gopxscev.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zsegnibs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2cpkhtqol.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jruzolij.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lgpjjovm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nwihhbmt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jonuvjph.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2iahzqeua.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ylkzmfxm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2potaigkn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eqnmeuwt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ehsvlmsl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ffulnrhb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ubyoyiyt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ltfhswyf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pvtorvtf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ztlfbcye.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2lvngklno.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hczlytng.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2chenyywl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2glbvesqv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2nccewjdj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mhbjzxox.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vcguhakv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jbdmrmno.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2czpbjdmg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pcdbkxwm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dxfozxxc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ztsbdaui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jxyhwhkf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2vkufnenu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zzdinlge.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jxfxcrgl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fpdwmyub.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2spmjzmun.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2lctqazql.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mafbyyzp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2blezsvod.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2akjhqtxe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xcimstfr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sxlavjlg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aosmrkda.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lzrtkxif.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qbsbgfxn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ttqsxydt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zmqvjzqa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2axyeuhla.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wopvltxg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kpgkraar.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dysmjwjx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uxrdxhtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2intojqzo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wpidogab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srioygke.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgkavpyl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zjynngjb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jktvucee.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzpkhrcx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2whfyslnd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ovykffbw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vllxdlra.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2lnwdyuty.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2buiceuud.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2efraeowd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bspmhggl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiadsjwe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rxfzptlq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bgnwxfak.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tulyivqc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ilmjlrwl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zaedauxx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2eszcncot.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2joczvpnn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rshkdvxg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rbyjmnaj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2srnqgcay.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2snszfasg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkpttxhg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2htyapxiv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2uqwllazi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2nlgvigaq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2flvpegpj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ooohhlbr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghlczkak.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zewygtkh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2rwsdqygp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bverzxux.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pijpfnry.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qlpwtwdx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vamlcplr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vrxttwog.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tmwipkqn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2negrguug.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cjqmfjam.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zqqqxzxi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2aopsvtoa.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bpfsnfgt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2eknexsav.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sgczdlzr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jcybeqxi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2advfcllg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gtblvnge.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gyjbodut.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bryiktfk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wctzqjwt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2eyybfagk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ldrmouhj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fjlkydtr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fhzwxnvh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hvixhcmt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mjoohsoo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ujwzncfu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yngqqkgg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2amjwvwpq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tlwqdobf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbdsnhf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qumupvgo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2oezrephu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jmggaavg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nalixrkn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2saxzynez.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2govlgchr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lvlibrzv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2psirsumo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yprjohcq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vvkpvent.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nonovujl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wqaljfky.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kxenuqqe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bgirzoyb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ewbvdwic.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ojyzlssw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lrimrfbw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oyhebjlp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ypoencek.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bhoojtjq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2rfoivbgm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2elwjempt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2dwblmlzz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2witzmudu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hvhkithz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zvelqurt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2randlovl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zsdoxaic.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xkwtfzba.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ajwlhnlo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hwendtie.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vzrlbqsg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xoqvgnfe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2twharwyb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zooefjbc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2elxhkmwg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jgnxcsgr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qctsmowe.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2uiwbklam.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2jfecwlnk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2axawgalq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yyedsuvp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2teukqcsv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2epbwpgee.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2krhatryy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xrdfmvnj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hvsgotiz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2oitvbykd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zjgpmyit.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pbxnnign.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eporudtk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouuwrbvc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gtjcwqwu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kvssqlpl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zehhiqoh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vsdcrlsx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qnurpegr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lxuwmrch.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sxpiucbv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgazehhw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tipkfhlw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kzdxmwiz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xwtcmhgq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vdhorgfi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rafxfhqg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2fvpybyck.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tcwvrqbg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gqffvgfg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rxzrqcxs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fklzknpm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wsmqiopr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nrirnwoi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gqouvsyr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wwntpbvp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tdwvglrt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2avrrixgi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vtqysmpw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hdmjcixz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pekrewen.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ylhvtigc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwstwqrr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylrvehhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npzovoyt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lcjvxmya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2julccgbm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ratrvnsi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jbzcvzpz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ejkwucqt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wixjuvde.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vhyyiheo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kehahkah.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2psucfhed.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eivrdmav.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gopcibtl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qjvsmhky.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lmoziqkn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qlpmsqyx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2omrcnkoe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvmmexwb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lkbzijpg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mewysoas.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2aehxrjtz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fstkwkyp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2kbteojyx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pxlskjhg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2guncdejw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2beaqvcbn.html


<!-- 参考信息 -->