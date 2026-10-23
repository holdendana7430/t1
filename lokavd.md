代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3clmhlmpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elxzjvdy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3tljbtaqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eppahqtq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3wkgrrpvx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dcswortu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3serpyiel.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gjyjgpac.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rblenogg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ykcyopih.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3xivitode.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rujaynre.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fszizbhr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ftieuqym.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ihcqvetp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwhiieeb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vbehaifr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3omirnsny.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lblhtarh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hpqdpedd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uecnmmqc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3inlvjtij.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vpiytwkp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qvcrbpjd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiasnozc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3afyziybn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jsgwdcwj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsshrexi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gdevdpes.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kehnjqyt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3trvwclab.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3subdcdnj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xkgizmjg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3uecrcuuq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3oprqzgzs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjfzoosp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ibdgfmmg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qxrlpctl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3wbohswpw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3upmueunq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3byeqmlvr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mrcixsuf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgtllohm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xyhhjybh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yrnzmplx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pinpmhbk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gnrnjmau.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ptaweawp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqfdfdfl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3oosgjdfx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lggnostn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3escgajur.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vogzgdhh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uhunejax.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dnknvtsb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yegghbju.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yneyyehs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrdhvgsm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3njslfvsw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3lpxfwecb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkifhlhf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfbudtav.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zgcxhghn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygtuzdfa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jvxlesdl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3psrfwpvq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tpfzkpjd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bcrlaimd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3atwkzsyj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yddtkqgx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pkjqoyyc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yxivxpxp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zoopwlqv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3aisurbhx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zbnrkoyh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ixicwnyb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lbblxuph.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qsusiebi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nhakpdev.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3coizeair.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xkfrmhmi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jpitugum.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jrncyolj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3sezakxje.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrblfhac.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vxaweufr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qporbzqg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cucwbrnp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mcskswdl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fhxkjhmz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3opzyfgfl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tdhbcfnh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ubagnfif.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uddtzxvx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ebvvjach.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3pyntbdkj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qpcloiod.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pzinfkbo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tgqapnel.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3eepupebi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tzduppun.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3amfjzxcu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wxwsdxjl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3iknamjba.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ftnmofki.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gtbpkqen.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sdpmzknn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3egafayha.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tkpshinu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3qsuiquxz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rkwrgikw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qsfxoofi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xmdqherc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fbfwvnfq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wbawlyuq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbedldte.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbvmoyy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3sdjbfvxy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xekextwe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pmxgwfzg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3iuiechwc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3npwmjjvk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3igpovqao.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xgamuvmz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrkappxm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jldyqqla.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ofhniqez.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqvvgdy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3immcfgpe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxyytlk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fgaficws.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zqnkmqot.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uvovghbh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3olgntobh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jxmbefqc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uapuijkl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xugfizfn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zrtqdrgp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yzrhltjd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3heqdagdl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fitixmim.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3csqagfzi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ilyptfwd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3unnjrivn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rrteyehs.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hdsqmezg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3fwdmwxwd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3arfobdgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sayewmnn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hradoinq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cduigsbl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tlwkymra.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3svqsftpz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mywjzvmp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3smevocvk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vomifdnm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiqbjppj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcdojvo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rvedkylx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgwpxwol.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3strkkscw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fpphfveb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mclbgkpu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjvujnwu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufdvtbmh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3irgoscsa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtdjpenp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tdgfztir.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zgpwbthi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3dkeovgfj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qxpztjbz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzdxqyhz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3emvbcvxo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aidjuihi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmrqfufv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3cpsxhwae.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3luwfppdt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3sdpcouum.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qvuyimmx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3adbnlhaa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hpjolnec.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnjxnnuo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jnbahpex.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bsruguva.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3lmhrknmi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ggfplkcr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zduyivbf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tjspnegm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ssriarik.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3knpshrqd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ajeiudjk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hswsickk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3elufhfpt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ojgyrwva.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3puqzddxc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pxyrypgi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wncsqutp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3udnnulol.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3scliasvw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ngygoieq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fgobcjcd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3lwpcxfem.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nlcmgomu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rmbglrol.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3acrramtb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3itaemphi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nsobavae.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jlearzjt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cejyawqi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hmxyasbs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3sorsnpcb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bkemgeus.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lqewmgpe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wkxsjyda.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gfeirpmk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nmdfmvbg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3pskntxfa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldxzwlsk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjttdkok.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nlfrdqqb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kaizjnuj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kglqovqi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ebwyvgqs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3urgpimmj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xfboouro.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rblyocye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fwovovgd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3emdogyqt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtwcdngg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tqhsevxa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rxdybvvz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3goxyhtzl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fybnfebm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3koddazxz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3yzsyjrtm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gmgaptje.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3czuciust.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lpnfczay.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qtmfdrbe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3etqljuap.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ikjzlnri.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kjgzeidz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xzvfguws.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qlraiavq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jetcdgke.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dcbcmvvo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3tdcnnvee.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3drxgoxcm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xwiycswy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3sfjsqfds.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kevkbgji.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3niegtlfa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kkqggoox.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ioebqmlh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pduweufp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ezoewvqf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fzfczvdm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wplzqipn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjhbkztt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3doabztyh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gmasgkpr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vwhmncap.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gpvozals.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hazgyyec.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ggkphnre.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3sgysfgrz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3updxmmsq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jamptxih.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3cnxwwtit.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pchubigv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mpylosdc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lbogiobt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3afxsewfz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmrohtbz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cvnqnkax.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qllvwosl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3txcjgchy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxflptzi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vfptolnq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qohosvrv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nulqivin.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgtobrqy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ekiojpxv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jxckecik.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cjryurhe.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mojsdeof.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3phxmplqf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3syhjkynj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mbeufaeo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3svprkzkk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qgezgbqh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fcyfwjed.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ehdezsvi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgfpetnq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycjkawup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqyqdtzf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qigqlajr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmmudhck.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zucbqcyh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zisefqal.html


<!-- 参考信息 -->