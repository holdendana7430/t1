代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uyowmvks.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iztccsft.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rrjzxoft.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2kdcpxyrl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ahegdwkg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gdackzuf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2yvfbedyv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bnqabecb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nopzfuww.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgkpcccv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jtvojjrk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2brogyzqt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2djajwgbf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2nxbnyuia.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2znhjplru.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2owotbfxl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2kbowjcaw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2yrrouvwq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2khxygoay.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gegabord.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjpxwcge.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hvljxeso.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2vlgqkfrh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2riutpbls.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qrlqjcfz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nekahnji.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2txuurora.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2brygaoag.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2umudamzl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2evercvlo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vclpltpz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fpxmcmmp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwwbfskj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rchclnqe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdgukmw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqwifpql.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihchqdny.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzubshyx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzbrlsvb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gdbnxznb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wjkxkbns.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zeaqavcs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dqypwqwj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2aotgrora.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2piwagigg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxeeibra.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bncuukhu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfvikqhh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ptgdisku.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2awizoevx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhzsvugc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mdehbgut.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kahxjfwd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aytubyba.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uadlrjex.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wnkoilol.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rypihqzz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ycozokgy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2csycamhx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2idlgoosv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2aamethup.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2kemqafiz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkwbocdn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wpfrvovm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qvbwsscw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2enkgifgu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wrqvwtlk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2hzwcozpt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukmsndyi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kfugqmii.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2veguboan.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2embaszmx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dqhyrcnx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2afmprryx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rcygdyhg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2yqjzdbmx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2nhzzebwu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahdkuruw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yweeekuz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ktgdqvki.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2awyosftq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vcebvibp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2agszhzgp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jiqgjoyx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2iihbwcfx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2lgfjhamd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cslyqnlr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2pjqslbrf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jyaibkwn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2soquwvka.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kbtsxvji.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ltxflatx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2unasjjkj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgwzpxde.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mrbtzfli.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gkhohgsx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xvwcxmnt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2dlkbcajq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnbpjxxm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqealouq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wgpsdvam.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2arragcbw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mvasxtux.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nhiscqit.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2uxgeqlqn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2esmfddkx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ygthglbe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ehhsqtao.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xcjnixck.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xsekcfyx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dfqqlqni.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2zoabwavg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bitarfrk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lptgcocq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mzsmlrcp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ybqsjihb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rsxepjvk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gyibigji.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fylqroit.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dymielgz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jvywrhbl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2anezewof.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mfkmvyer.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kduaxpye.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yugmmfpw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2whkovfub.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sderymhx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bvyozzgb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hpabeyif.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vpkmdghz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2sjrshseb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rbznjref.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhiopbwd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mlrjaibb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqtjicqu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qvhwlixr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2cnwcoorv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2njyhgpsj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2irfgtczk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvnuklpq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqpwcmlz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dvngoeqa.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ybhpiggs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oivynuqq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2atjffjyk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ejasukjf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nnqlsvlt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxnfcupo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjebothl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lvwjlcwd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2holkkzuu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rhmxbecm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hqzpbdck.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kxczjpdi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2itcsstco.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwztexkx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kulqniaj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zvmeiwho.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2uhefxlxr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2biwknfvk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fyaxedad.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ozfnrgfk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2btoidqxt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lkayenyy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fdrbjbwj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdlpvrps.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vhmsvutz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2jykmpeoi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vnzmjlnh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ljimzaat.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cgtewkxv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ubdptjqk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2djybmmqi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mznbinim.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2obsqawad.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jbrlvzfd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tjuufjys.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sluteysa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2vnceikbl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mltgiqbv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2umvdxylq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fuomazjj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yoyzcbtr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rmobbvdx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qfajhsta.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2upprtemx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fvlzxqui.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hjnyvtxa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2utqojzyc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bxxqsdmu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zcmaueki.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2biidvxqw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pjoqpznx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2exiddbxa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2iwjmrwjl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fglollpd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2zsyfmkid.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2pivnzeva.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2glsmzgbh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xlmrgsao.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qimeoejp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2heipidor.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lomyshac.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ybzdrony.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2uqnkqxke.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fjhexexm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuwjowqc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zqokuzoh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fnjjlvns.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2googrmma.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hvegthcx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ybagrtou.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zafzrzxe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2nwhgmjst.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2niihzdwg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2icguoset.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ifwnfxht.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qtdcbfvi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2skxdgpcg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ffoubbyc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qvronlkx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jbevymkf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vxwjnklt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qfzoehqs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ukqjznob.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vcakbqqt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ixiljfmp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ozkpyglo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xggyjdnn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2naicqcnd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fdtcdyvj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zdimikhm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ssjmhzsu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jkxnfkng.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bvjqlcqv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tszcdqad.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ueqikdwl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vmhiialr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sqgjlnmh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ihxbsmpf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pljkkbbt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tisnufaw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxvfyjka.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jlfwcuvk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jrkdnvmw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qqgtyehz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jncecudn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntihdfna.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ohzwfhoj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2crwrlrss.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fygowphh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kyklpxls.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qtzoquzk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zngreuki.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lttclmxs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oxajirqq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qakvlmfg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tgikeyrd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vjakvzxh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tjczdovu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qceshyvd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2srvcgyie.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2areytesd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kbqkzrsa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pydvuaet.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2poevxhze.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kyhtylci.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2robcimxu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ziyxbicm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pzjmuipa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bkwgvmjv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nsdabway.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ynzuyryu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nxyysaoy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2uugyibsb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lzhemnmo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gxiasndy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qizuazbr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2utzdsuqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvverfba.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jbqltwns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqjnlhxo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wqhkcbab.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2eiwtbpgs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hgruaxqw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xxlzzpzw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zcwapcmg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2sopczzjm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2kldloydb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ekyckfvc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2otcrotei.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hzjtkfbm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jqkaxzvs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kxteeyku.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wqvoybsl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwtppmwo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cuslvell.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fmaetreg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wgjpxjmw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2pzxnoieq.html


<!-- 参考信息 -->