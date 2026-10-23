代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kqbbjouc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kjitxfkx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dwizfrpf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rwpcfokq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zydzzple.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3oakvygtx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zsjkignk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aquqdeds.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xhoknzon.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pmfdrsyc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3muytsqwu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3uopjoqpi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3brgyyyat.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mbvqeyiz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ybxujrxq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3lkjntqro.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frukoonz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lkfzxilc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wkqkngxl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aybhgmoi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ppnithbb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vpvgxktz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lcxtmbfe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xapodbld.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hvlhldfs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vovzuqof.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekwlwgon.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxmwflsv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsnxooce.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kxbbfcfm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3gvgatkyi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3reirxaub.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jkmhoksr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3enmzizpv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiugazaa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lmhsatwu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sghotfuj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnlcwoik.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3twgxitec.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3uvdfufgg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3axczekes.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zcvxtmig.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3sosnqaeg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3sudfqacc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kmltnyid.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tlrpldnu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3uqsnyzvm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tjphnedx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pehcigpm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3cbpkaopv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bdhwobls.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yumtkusq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifrippyk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3peryidxw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cyppdauv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3drjewzvz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qekleaym.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3atjuhbvg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kmzlusdj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vgcjmjfr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cnzdqmqw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dfxpmzdk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mqdksfeh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wtnrawol.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zjxkxdla.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gygenxrz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jeowtnwx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jfihrrff.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zleeoiep.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ajssaegn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lptdneqy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wuktbvyu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ankcggwk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3upigztyo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ygsenlwy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jbzpmaeu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3raxieznf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3nssqqifd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3afhkphqn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3akxibrht.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bmfnazrg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bozmwqfz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejlikbhr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3onetzukr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lyxxqyvo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kylfqegb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pcfazkix.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lztiuvyk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3itufnhks.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3anamwzrm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rdoxvigk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3amclhjom.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jgdbkshd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cpbxrbzf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vgccrbnf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qijckqol.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nvhtpjdm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3slduvdua.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dxyagzbh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cefppybb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nvgymqol.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3djuwhezy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wdncanyd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3adutktoa.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3yopqwqzf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3adywasvl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3znagmegb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqqohxwu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rlbjpfdr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3scmpxqsf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dsbfgbxd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3owktwdvd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mjamzsxc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fhvmkuom.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dwiuevgw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3clktslvp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhthfars.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3raxtoupt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltlfuytx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqtoteow.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fftuutns.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fycncjhv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ynhcpxye.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bbyfriac.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gonaxbat.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wwxlyvjd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3coclkkev.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zrorhfwa.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iapjkoep.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ruakvtnp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zxncrxnd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xznekhhi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ubykeiaw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jcnbzznb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kuubrtlq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kuwttvhi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3exncyrlj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3golhdtzy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wlpxyeuu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qfbastuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgvrfcku.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xahxgllb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzdbpkeo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3erysufdx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nafpsvvs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcrirxpf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsvpjlka.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3baivvlnq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yvrdmgpd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hmcdtfrn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kipcfcys.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiawdqcc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fzawoisl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mhbdsrff.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjjtiaon.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ihcjocnh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gpfattsy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3izeaxyon.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpiturjy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mqefxnig.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3euuwdrmp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxfufjsp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3rfaqzswa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rzzisbes.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rtpzctgm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yzhldakf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mkmyhdgj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3btodeogr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wosoqofc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jjzfrowx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dgretgwm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rsubqtzi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eijrmbzk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqrdaopb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aebxlyqi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jfbdnckg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3umzkmjna.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zdzuqfii.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hgxljosc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3hvltoawi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wcekryoc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3aatcfmej.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3knivxecd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xdkfwcwd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3pookyyvw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fpeaawhl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ddjwveod.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vksprzrh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xwlgkiyp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3acoznowq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fhgxyqvg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ypdkqspz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pkhmjiey.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rounfbqz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wgqujepq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nxeukjxq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oqomlixp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fwhmzytv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qxaamcpb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tnjigyci.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qtyevfai.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wmnwzhga.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3sysaodcy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3epflnduc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3brcqwjjq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vcqbvjlj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vcnlzpes.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3evjwdgbl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqvicxwi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jepmyzsr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uzzemget.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cczqsbea.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lqfoamlp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ssqsvxcb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aglxkglj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3zqakmejy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nibjicjr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sdpcgnvz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vdcfsvmk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jfqpvgdg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jfrfhqjh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3gfrhxkjf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wpdjikxr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gzmzkryc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mxbtzvxd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rfuquogh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3jlmtatgn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3emnzyhax.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ljmafoym.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aqgpspov.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mdlqvtjk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ysvvtots.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dajevmrj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3nqldoxkh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mzdcjwyr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kvxzpjpf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kjqyiupc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wwnlkpxw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qyahvjik.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dgiicxsa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wgbdwcni.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wzvybaow.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qcwcclkr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3aowfcixz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mwtgoulv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pagsrliw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uacaerwi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xbaauqqx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3todtuuad.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fwhhzygz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ppcsrkmx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ycydywan.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ouructci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipnjgxzs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3devfwuvp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3famvbnqg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3calhgblh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vwkwzudc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3szbcwdvm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3yyvszdig.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vicqujho.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qqldlrwz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vyfysjte.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dxfnxcxf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3imaxejws.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3teiueuih.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3alrbehyb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fjfzjawi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ihyuueyj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3timeqfka.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3djyhkhwb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wwwkighk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kovqtool.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzcwlmpk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3idgopjbq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qcdvzqhn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tddsgakp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tvaoqyco.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3flwfelmh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xiavctnd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cdvhvtuu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3degovqsa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gvrynhdz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbdqcxzp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kbuiuces.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3vvsclgcn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jkwlsvgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oezdzpdp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3aqraltoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygawpvbf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kcqacgoc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cfztxlfk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jybuujpv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ewzduiww.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kauvhgpf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qkdkygai.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3twwowahh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xyiobxvc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mbthlzmr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vakdqhgi.html


<!-- 参考信息 -->