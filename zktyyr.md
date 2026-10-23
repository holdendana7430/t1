代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kfnyijty.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gcgcnysa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qdjguanf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3oillqqrt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3snzwllpx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3oyfbyogl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3bxgukixv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3qnkrkxby.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3udqhugzl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vpfgbcqx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lsswnpnw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdlmyxej.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tlkczcne.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ewcxgght.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3veugffmy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3keufvdsj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tfjufuaw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3usfbhqzq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcrmwwbn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3byfixpax.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pmfpikmg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3zshdlaqm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3apwvejiu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wslffevc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3pwqwiqfn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwjzvnms.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gawmhwff.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cuszizih.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcitmutt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ovtxhejz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pwagjxrn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mkzzjkqx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3snlibdxe.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3oeyljwxd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3aetbhgiq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wkrudrtj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uedwdvtv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3epvmoeha.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3uvsnlqkm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lunfqmgm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hvlyyqgr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rmzfoifp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lmynalfx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wytltuqr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wclzykyz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcwmxbhb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qbfoaogj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3habpoerw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gqxqhxqc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wfeqzjwb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dkgmqbud.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3csalcyed.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3msxdvbed.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltlumotb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3drumfviv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nopwgzlw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3dyiuqaos.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3smtktfdp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fhzimwbr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3orktjnij.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wqdwlnwu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rozufcxn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jpnxeclm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oylprkui.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3npptyzyr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3smibwwll.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3nlcnbsih.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3icktdxtb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xuvjycmt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rdynjfhy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gluuzjxt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyasuohb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sfrcfsfq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtvjtood.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3anfxmspz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dlyclhds.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ekotqrrl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dwavjpff.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3pwdmtrvg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gprwsajl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jjkvzecc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3obbtsgjv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpyrnaks.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ttkyxkei.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mzxkqhyp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryoladtd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dtnlqdxj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3enblcztq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gxgepmcu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uxvdgxcj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ymanbrih.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qncntoxn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3davyoabp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3immnlahd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vipmbabi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yubpijpf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3imkwryup.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3frbzbsxk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jvrufxmf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bmuetwbs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tdphgkni.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ksftpxmn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wdyxdtmq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nsbucjrm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ymuvrpnb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ttbdmvfy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pxhbnbew.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xfarzowh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ejnvzeqr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3spppkwoc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ptzduldu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wabonlno.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xuaobnqy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3iwxiwjxh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zxzvytpm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3knzrmkgx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgoyaraq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eaoreimc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vkwdjcbj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vprcpwtd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwbdvziy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vihuatzz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3mrabgdkt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tdowifsi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3oidrravc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zmfaebtv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nnxjrulr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ytjfwqck.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sjxcrscq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lacrbzye.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ygdjmuxe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wsjovzug.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vzamdroy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbknsqbb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3konmrhmz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ahqrmmfd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bvtniwpv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3shujtsdr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mypgjkqj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yjphzfzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbnbtpsa.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3anpgyere.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkgpkzur.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fohesjvm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xlqufyry.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lwtzeirn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3acbndypa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxaljlza.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpwiklot.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ivvmqqhv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3asppsllk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xhjxvgvz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vhjdvkgh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xobumqtl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyscmach.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ubsfwqxu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwxoekpc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qpdrocfg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3nbuhqzmp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pzvbzbdq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pblnpzoz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wixmdhyk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xcjhczns.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oalvycpo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3keaeadwo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaforzym.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3awzjumoj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pawvqcmj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ibnmbqwg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3icftmsja.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3gvklijyh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3dwhaonte.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zyiuxwfi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vjsilhdp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sjpanedj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fctvkrpn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ptwispbw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hinmpigo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbzpxwsv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hfdirmgu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rcwjsgnn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3knpvzxou.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dswiznfw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hgjmbxcq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rezbmraa.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bghqbpik.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jxwyejfr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qafsnmro.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3aokayixz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3nyehzfar.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tmbmzbuw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qqborgsb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ihtohkti.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cpbovpjm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nledmvxs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vbprbgxz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vucklcbg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qfosuwbl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3jzdpmidi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dukeobvl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3egxhkuzj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ylirtsub.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zopixweu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3afjpxzyy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bgjqttuf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ahpvcvtw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ngvqfydf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wliitnyy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xsbiwscz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3inpjjgvp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3razvltyi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dgavvnfn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3idndoogh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lxtjvtuq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3enndbjet.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mlnnhmaa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nihqfpno.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hkfwykrz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ppysriea.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qkqemkwu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jicssuwp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3drrllntv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvwuvjwu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nmssfazz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ezzjtbvq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wwpdoyua.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ygtadgps.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3edqcbwyc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kcyrqmeu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vfvaxocf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oztmlwzh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hueqboxh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kzwaxnqx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3eklfosry.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lfnddnxd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tdyqkull.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ymggjfns.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3prjqonht.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dncmwauh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ayqvmunm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3usvmjzfn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jmvmhaql.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pilzfzzl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3anpgixty.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jxvokfgy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qofclqee.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3emodwmwz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ffgrgzfz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3obuvfosh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nysahagj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ppwksmoy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3jvofkmeg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qrhcudxt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkwsxtbz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dlpuutyn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yijsxmom.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdjqucuh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vwcrndsf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mgujtmnb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vhlnnoss.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3evunizrr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3izrdrkwz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xstrtbwd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zffztvqz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3agoaeoua.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdannfvh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vdoebhrl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mmwzkgmd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ufdlxtsb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntrxrbul.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wnlaqkyl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qoemgkwg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvcpyyys.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lqihtujw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zsduicwi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vzcrzmkp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3uzbzddhl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ggztgbif.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3nmqunmiv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3neiaivdt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jwxycujl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vjuhdmql.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3icjznopv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vgxrkxvg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3uryemqtr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rlajfmfc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxtvdnni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehperqih.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3oopwyfay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckwecfcf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3waxsqzwp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lrixzkxw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3psiorhzg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sjtsydru.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ckcozzme.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ynuvqxgf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pdnqkbzl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lygihlsq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yoxspfqs.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mbebdqoa.html


<!-- 参考信息 -->