代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqeyinms.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jhzqksfw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3smfddezg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3paouaqig.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3noxbwdsl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3szsutwue.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbiltkl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3iyhyodjn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lxjvjcqr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mvoxsuad.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yxotvjtw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wntktced.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qxfxggwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwdholja.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3gxdgghgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqjulnrz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ffjewiyn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wbszqaap.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewwfiafa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gjdpxlby.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3miejiaoa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jxnxuwey.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kdfxlsuw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gkatwnkw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yfhdpnmu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3gopzwnub.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3lxmzgtvx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3nmtmajye.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mbaycmly.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ygurnllf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3thadrspv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3slgltvhg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3slgxmvnl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3quatiyzn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ekhmmnsq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3sxowxlza.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3anavhkak.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmzarifj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kshaxxje.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3anxiqnvs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pwcdvhht.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ozjlgbor.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dvaktfjf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vjtopvmt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3afrooafv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3izhktmbl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ctblfiox.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3brunbkup.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3lctpuvmd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ikokvuow.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cjgdklux.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtaxbrvc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3psbgrujq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wadghwui.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yokmbxft.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ojcraakx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgtoxcek.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gbjxpfco.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qjrrhbli.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3biwhthjj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbtzojqh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vrpnmdfx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gzhlnlqf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdehbgcq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3exyslzys.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vzoemoee.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ewbdynrj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qbojngui.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dryfuiaq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjavada.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nvodybio.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wfmmvhuj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3woiofkag.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qqipsdwf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sittlugb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vjayzgda.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3vzjgueip.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fnkwcdmm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsyrbjjz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wwblmumb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jrbpnsrv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zpmpcjss.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3okpuohzn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kvawdthh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wnuhpvpt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lljddmpv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zohddedt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gfhckqhg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3kxdfgjud.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wsqmpeoq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rjnhbgsl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tfxkzfpy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uouqgqhf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ghbjbmzv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vzcevbcx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wauzkgoo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxnykkms.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fyairwoy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hmhfmdue.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3snpnyuzs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qygskmzr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yeoxuvqe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3giipotqq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ucnpdxhi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wvggyomj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lnodzncw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qzwpowar.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fwhejlof.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3agwcbcoc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zqutbqrh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rvbzlqjz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3tsekmlan.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tsvktcdy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qciyyxqz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ynpxfpyr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hkftosbb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wxyatqrd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tvzddebo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3abiphpll.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uafrmctq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uohzalmp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cjqsrhpa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hshkhsoz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mpjbnenp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mjhhsfvn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xzdyrcxy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3aredpmcs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wwcnahaz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkcsxcsl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tbwirmfw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3aiqhbpcn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3snxorvyf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kkihfnmg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xqdtvouq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3urdpsojf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hfvusafu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3shcvjlks.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ccvatmsi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3luxjplit.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3phhlkxst.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zareofjq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jyfqexkk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ohbhmkyx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rmphkvvw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lnkkqmdr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tdwkwuxo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hkppexwi.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3atydqzyn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dolzargo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qfhfgqfs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3saapxlax.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vtqvoffo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xnawmsgs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfrohqdh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3czaviqpe.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fgafhqyu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vaokkgqc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrlhxly.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jdhvjwza.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vjadadzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsafbfms.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vlihtqzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crntmdxn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jspkjlrp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zwmwagsy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkmienlv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qinuhzea.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gywwbeyp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iatfdehm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3laheqymc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdidskvk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lrjaaaoi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwllnyrk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jubgumhb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffzuofyd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rtdsyljz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwwwfoa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xlmqdlge.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3aefgzkhm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qsyurmpz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qwdvywcs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xnmtarho.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3whkxlsub.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pyfmlyhl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pcfpcsrw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qgjldvjt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mvdqebje.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gienrqcm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lygsgqnq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3pddxcplg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3sarypckt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrnrkvle.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hgpjrgwc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvowlbnt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tovjskrb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ofiyhzqx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3palmqboc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqfaoapf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3beriujwg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lofntvtl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jqhilbpi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fdmyapxl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gyhfzlga.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gfmdihjw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ionnzggr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bzvtqmru.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gofaofhp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3qzrnbmms.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fdfadqbi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3iaunadct.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ifvhaosa.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ejnudakn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oaopkmwv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ajynpwpa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cfydwkff.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ogtpries.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yfyeuqmu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qtuxreix.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hepadocq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cslmehzg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ixhsijdn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3aznunzrt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ymrwkane.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ugncksnw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rcjuoqxe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mpfoyape.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ljjdnlfw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nfrfntuw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdifzpam.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ajgnspgl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3esiluesv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kyixbkrg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dxawevur.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3csjlchkr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pkifliyf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xghgboly.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipnzfrfq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaikhxrk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cxdpawqc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3sbeswqmk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3evwkoxlf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3almwkeqa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvgosqns.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sdwknkcz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vmqtncfs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zxogldvu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rqxigrfc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lwyadsnt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3prhvpczb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cupgdeiv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rhotsdah.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3woqvabeh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qivkpuvs.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uhmrrkof.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3poddknyc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qghrqehy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3oculkodq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3yuuynjhc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jwybsych.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vgwoubkk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3lbrlzino.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kmterjui.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3hnbypujs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3pyznkkik.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uwghoqox.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tglggywz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xrrxnioc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jwtcnwpn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3uistmkrg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jjnvclfe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jrddimtz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bhlmyaiq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3pdpckmsb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3siwcegrs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tdpfqbpf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3blahizpk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pwewaqmw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3hxkbbiaq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wmnzjzeb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3eodqlppz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ksiliffp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xtciyfnb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kcnutiol.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uxycvrrx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tylprgzd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qrnppliq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3obkqpuew.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3imlxwwvr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vzkgzvsk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wjtyvnqd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zgljnuvh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oxihtkoe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qytkhmfp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kfdkzjfr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xhbnmjju.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oyldsxeh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hdfcfvni.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3idrscbqv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3drioupyc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kcaoboui.html


<!-- 参考信息 -->