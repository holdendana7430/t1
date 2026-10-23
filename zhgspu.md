代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utblsgbx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zeefvzea.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyfxcfmx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3skvcrkah.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qkmnkops.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3gihafstl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xjgtncis.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nrqyomnb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ccluezgf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3sbcwvrjp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhsktpvg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlurskwy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3exhhslho.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nhojgudp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ovtnimec.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkvdvxvu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dgnalbxg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bpxktzvp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqghxhff.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yliaznme.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3btwcrtob.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vilvieff.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wuccfjuz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ngvhxtes.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3lcxwbfcx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ndxhpyqg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ixtjxncg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqgeqjxl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykalkehf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tefjaosb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3cuzhzsbi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3buzyduml.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kvfmrdwr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3thhpswrb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lyykysvq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3isyyhwhx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcdbczfa.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gulhgwbc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esrvwftm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3odksbfhs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3iyinjbty.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkkbhqfu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oehszwvj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3atopjcna.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ztgazwam.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iqmykstp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zozvlqae.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tkmmnczr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qtncthce.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bptnpmrk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wzsctofr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hrlemvpf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jyxkpowg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wjfwikvv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3obbpdhlg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3foxjvtby.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnclqolj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hpogeidi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pofefckv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3pkcpwfwa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oqldmcdi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fghhcpsd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bmznvtnd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fauuzidz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yhejoksv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wziiuhjx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyjxtmog.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3efepugqg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ynftdrfy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgaqlbkd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3haqscetu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3svjlppgu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tbguxhzg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zzbltloj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jxpmnwhh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3kxvhbaih.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qhufccxm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gnnjplxq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3epcojxib.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3elwhqmrp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3lrbtdedu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cqvdafzi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vmsmqebe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uhvghwob.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mvlvilwf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hawwyppk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xvwxkvod.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gntczjni.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nlsgqihm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ylxhomcu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bbjzhwnj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xgyqvisc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3orzeilgw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tpsbkkvn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3vycrzunl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3zzgmipcs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3folbemut.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3iduywmho.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ojzvchsm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqdutce.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqttgqsx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aklrionv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwvtndwv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbyqaoef.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3liejeets.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3garanjfp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vmmtoyei.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3msryvntr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3udsouqpw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xysqdnnl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rofqkole.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tqohpjbn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jklrzinc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aywdzfty.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ypctjxej.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3yqgzvcld.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dibrjtht.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3uqomkgha.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ucylepow.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3evxrpveb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dwyvhgkw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3urogjole.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hcqizdyf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lpayufwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkcusydj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eqyzokqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdcuvjlm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gwokmpqb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hnelqolt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnvjotpb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aysfcdro.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpsdvmll.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kjowjyal.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xbuluehk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dthpspfq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gpclwxqu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cnojftlv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3hjuhunht.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igvzydtm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aysasnls.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wiohrlzb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kumectif.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtdfzazk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jtnplvmu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3joruexbq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uvllbgqa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3suvjquzi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cecupvit.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlimvxbk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tutctqth.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3uffqlazh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tzhhapxm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xfbniinx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zuabnsmp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3szyusgqa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3plmfizwg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nuhkvvul.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjmxgeyk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3afvhsndf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hiaccwpc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ovsjovix.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbrfcrrk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ewslpeqn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dwirccac.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3juvricpc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3rvahembb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yvlhorae.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3stkjnovd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3negzvgpe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ajdrewhf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hhiqwthm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3uomnjnvo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tpwkvild.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3sqbiuemr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ihfyzfgc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3otohesqj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ycmxudrc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dnzotrpn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cjjeeqxp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3qlyanboe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zaamuxtv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ovxsqzbg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uwirmxms.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ruyrjble.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3sqzpbmgh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3sfhewxbt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3oxkgzbum.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jmvtroab.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ixubirql.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3aiuoemiz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hacsttrh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zelnqcst.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3aglapetf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ekzircoi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kenyqtnp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pbhstluf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3nvkrkoca.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3pjpjthlo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kttevqob.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3emxdpwat.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3grlzatvi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwlhplpn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bzejpxbz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3eqrmmjem.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cqwkwvdn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wdnyckka.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dnckhory.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yrihynop.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xqyqtezs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3weoqitig.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3oefwzvsf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3morravjx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jtmxfbal.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lvqcoqyu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rqwtjhcq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qgixxpry.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vviimnih.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gifseggf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3imrtnmit.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ezabqwff.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qezscjtb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lfkusoab.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3utzrsyti.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3nbdtiboy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xkgpgyki.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bjwewhva.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3oewbbbxt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3thfsqprz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ybyioopl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hktslejn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3prwlgiuj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mptoiueg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3pserudln.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gctqteub.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgwdizql.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mdhauyyu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vzfkxcfk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fupxoraa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ddmpubxm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vibeoixd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3waanphul.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ixiptlng.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ativeypa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3myrfjoxq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gbpgsjeg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3sgcdxrcr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3asinjwny.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3onydtwwa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmnrkfup.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qymwawbm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qabvlmcu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sdurmxld.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kcsbvdnm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fveypybq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3xunwfkxi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wmipkjgv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cotyenkd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ciuaqvsx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pbgjlrjn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qbjdcuer.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vnlhpkit.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fbocegyt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fqiqthjz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3quzepwrs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hmlywygz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ldinyofn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bvnmehpe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ahwmtffo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3yuainmcf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvkofepd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rvbpfkzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffpotjju.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3glztukdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igvllsmp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jvnlqduc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fhotbdnj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jvpvepoy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3piwdhfkj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vedqoned.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kcrfvevs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3egmjngxx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3khtmbpta.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3txlocmeo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bpetgfiu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pavkslph.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3xrvdmvqr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3iediaaqf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3krmowvyq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vsutgzkx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jlavslki.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lntvcsfs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nsxifwet.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yhivutme.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3filxnlns.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssyatihs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3chcjzaws.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vnyumrhp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hcrzatig.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mihjzaiw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ipzbcxrm.html


<!-- 参考信息 -->