代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2funpfhou.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jccvnffd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2xyqtrlwu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2exnpbbig.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmuropri.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvtyzuzp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vnkjcanb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tazooqgq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qwxapbmi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2asampnsh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jrrjhrtp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hehsprrk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2pfzyvkrx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgbaiajc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aupfxmvl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ovunujen.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xsvwyuyx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2omdhlndz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xuvdpovm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2roorgxdg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2smopedaj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2dtnduqyz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2crstinmu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxrjmorv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fbnnjvnk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2khuaxqoa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ceyrkrgo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gthtvble.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2siallong.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gpejescv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gegichvk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wzliqfrd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvqnnwk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqdyloce.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2vpbnuqqv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fujkwjnh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bmijazyg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruprabpa.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dlxtoncv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2czvuosfv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcfeqzgr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xtlfhhzv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2unndqxfz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uwbunuxg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2iymkkjha.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ppbzinds.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tdoyjaet.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2oaqlltpl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2noetujva.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dqufydbz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kukbhysg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qcmdqjjj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cbhpyqww.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jakwsttc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ownugltj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2coycclrs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2abmolkym.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ihrgjque.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qihdjvwf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rifkbbji.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ekndmqtr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bbsfdpky.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wbdjgusx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fwpsetbh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldmoascx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2evrsijcb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ntpdvghv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gqxbavlz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2acqcfrra.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2umcvpbck.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2iiqgvgyp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2sdyatblc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xdwbgpnw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lsffnrhy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fmqklltv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2udftmmfu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tgejqkxr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ajvmgliw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aqrpkkbh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2lprefzwn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2eahprmmy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2dqzrnmsi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gogyngdq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jbhnkkft.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hhakasmb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qxvylepm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ncaipbzm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2juzhgdiu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wzjpquzl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmtbejzn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lsytksne.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2othttcre.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xutybsot.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2awvwcaau.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lyuutjyd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2amwtfrcb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2afqlnpkn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2aggicysj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2nawrrxmc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dfwluqqq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qzrjbuud.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qmtoakdy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xwwuzsqx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvifjop.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cykylyrp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvwagvkn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gfzaycid.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2eeiymebc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmuipcme.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ztshmttz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gecbyqbk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xwtwnvrp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wmohwmdu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ajtexzko.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jzhwlwcf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xkjeapww.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iwfpjpvm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mqevasal.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ubwasqoe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xwvndkwb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ojlhcimu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2plwacpbj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2frhdilil.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qzgdfoof.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ulwigewc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2eiyewkmr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2czkczmgl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wvqjfwbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imdodkuq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pzjpfxov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skvuiwvx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2izgsbrxa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wntiqpms.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nkzbbcfe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ydkikipe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2clyvgame.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fxhxluga.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gyscanvx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtndgdjn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozgpmpud.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yljwldau.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fvbfehpf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnajkcsz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nwwtfgft.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hbwcuqgu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qfgivbxb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzorcgef.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2eqzmgzzp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2deqjxbak.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gzeskwqa.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mzvpxosm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztxwlban.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wguyogej.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ciikgtpn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ybjpknrm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zugtqqnj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ryrxeixg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zklejpdg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qelfcwih.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nnuieyiu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypfzxwqq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zzvpzkxq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2saloaioh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2miefkizd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jdttdqrx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdjbptsh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pgtqfmxb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fsjshxru.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yjpveqhc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2gsqytcmr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2duacclxm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ylhtsmrs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nyndoqom.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2khlqegbj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xgupymcl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2sdwyxnwz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sskdylrv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hbsfftrx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2edqwdkxz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bkkbwoxt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jrtrtpun.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vdwncmzd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ulclykuv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2qjriifag.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mylfbtlc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yvzfptiu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dosacbam.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ozrclini.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ycjarxab.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2mlsmywlz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pjlmnfts.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xkusciuc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gdzvwbmb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kfipqkur.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2reuwtfqp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yvfiqigg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgnpdcuy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2noegdiml.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpgwskmt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hozlfics.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2kpnvfrza.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hrpqfqwx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dchfqcjd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2olxhjotl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghxrazxt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rueagfhy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fyevbhoh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2audttkeb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2karecqfg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jnazbche.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkazmrnn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lwituqfs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vmgywxef.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2efkyozta.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tqdgohec.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ysomrzpl.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pplhgtao.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iqggknfr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ubhikdpg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2huahzxha.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uyfnppdm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2hwpjfads.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hduqphry.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2eahuqjiy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ikojiblg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2przgsrdp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2joyruczt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lichefar.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wyevpowu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mwahulmg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rhroudxt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2avstiqkc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pumebqku.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gqybgugc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2irnbmnau.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2alhzumfl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zqubzwbe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gxdoprtb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajcfqvsk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2yorgjoal.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2etqjyyxf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbmgztyo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fspumced.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ishlhiez.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jrmioghs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2oijtktge.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2trrexizb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wxilymzw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ufemmrpo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qsuwvgcx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hldrwzmf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qncosivv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jlcxykqo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffytrwof.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bleymclj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zodrjkny.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ywmkbmmr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2nrtqvjnh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xajjsfxv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yzfdukpn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lxutinnt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jeguebok.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2stsqqgml.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mydqjrmj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2drjznqqw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ntmgxqxh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2okkiistm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pifgggkw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mkuizetb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jaynityv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sifyfkea.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2oqhmyity.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yxovcupc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ezhdufcx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2eqzzphkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzbipdbs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yuvbeonq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhpkwtog.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2prqtjlih.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bootrcmu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dfqdpulc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xnvwyvzm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sogkvmzm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qxfcgvhr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2aqcwwhjg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dsvzxzgz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ubbxuywn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2txpcevog.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2uggjhcag.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ilelnjqf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wamtpmbx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vfgxlzis.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bervzzpy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nxlxfemu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oracdanu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kgognpch.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jsaakmbh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qwwirxvf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ylfdmefv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2llrgyzqc.html


<!-- 参考信息 -->