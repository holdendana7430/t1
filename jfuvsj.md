代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsxsofcu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtqsokjq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kowbfhhw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pxxwufyp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ndksgldb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2oqbmirqv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xnsgxfoh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ffzonphn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2taqtyztg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2clorvgol.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2awnzycti.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nprwtihk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dxewzjup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnrhujql.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rfpznqzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drhdiykh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2labbbvyg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qpvblmxm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozglwccf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2swffskdb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eqpfnxht.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ycqgzymk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gdgfdjmb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2vrkuwiiz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dbgqbbng.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bkexhopb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2gzdmaubz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kasvtnyt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wgxkhffz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kumularq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ltcgengf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jsiyldvz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ynrnshmm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dqjvgidt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ldnygnrs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2qkxdwpzf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2laugiwgs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsuklxpl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cfksharw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hymgkxfw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fcgcslrf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jnztditb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2trjxshlg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jqzkuruo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qaratatu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2fklgfrum.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tymnwpbz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ucfcvzpb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zfqoerbj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mandczgw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2irztcney.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yssxyuyc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kiezfceq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pcvjbzsf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2axkofhxi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nemrkkrx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pzmfdswg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzjusbnl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2khktaxjr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2swxnomud.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2attlxztb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vdqlrkvo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pppmjvbl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xoklxefg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2amtfaoes.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2emilhesk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wftyitbg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xdomfuzx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mudxihgu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyvdowas.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xcwyjgkt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fhpbzrnp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tpifjrbr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wdgwtfxx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiyoqzgd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hfjzdcom.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2udlggocp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2sjxjnymt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2whhfwgla.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qjbefijo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ddzcxbti.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qeaqyfdw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yvnqbknh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uqixcekc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xjlztaat.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ivqiovsz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2kdujkxyw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zhcjzxvb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ctrtmfga.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tzhixaof.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jckbmdbl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ndmaezta.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xauhwzcg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kzmirrny.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ejtsunjf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2isoazupt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdnljyqm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2wvaokxth.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bybwakpd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zpmljwvu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cguwnskq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lruozxbr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gfmctryk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hatkeaik.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2miwqstfw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mtnrwgse.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2wjvfoehe.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2udqurvdq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nuwytqlt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cswhwiej.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2deibbguw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wuzjqaxd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mxdkwyja.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qaompctb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ywdkwler.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2aknmsqfg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2scvykihm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2eciswwhs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kdhhicyb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vhlrlobe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rnlkkrdw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wpxteaby.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mliovszw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2itqkcvax.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2amktxwfr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2nirovxaq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhizkfii.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eaoqgagb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ouxwxuok.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2jaubjjzp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pclleazf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2xiilsmcm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gmrmucoa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zskpdeoe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jjawxgyt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2qizifdqz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lfunonft.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnkpolzh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpquxlxi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2elhhzayd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dkuufnaw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bpujmacd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wrvphqyj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xdmucqrq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dymfgjwg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cdwltenf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kpltikch.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qgbklftp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rtjwelpg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qkekdvlw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tmqzjyrr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ojvooccb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2dvddtrta.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtlpboe.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2itajqliv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ebukkwik.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ktiwrfgb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mocllbxj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2lveglvtv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mfecjtaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ioxyioid.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fxzpcyky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmyerthn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2djgghokj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pwuuwyju.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkagpxdc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kezbpqkg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfpuoloz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gpklzpse.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2orbilcve.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yzsggqjr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkvennbd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2euqrfapw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2uxckiqwu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsxmhdmn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfnivdno.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mepbyxuz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2swovsntv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gcwekqbw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2cddeumbx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uosfaawf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqhzweci.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yfujsgaq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfsbcfgv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sfpqmpvf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kpivgkkj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvqhtzia.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xpfkrhmc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2humgseku.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2qricstdq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jdojoufx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wagltmvh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lfudxssc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qipyynck.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2quteznuj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rkrzlraa.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uwwzprya.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzsqkyzj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2trslomwe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2objcdrwt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ycgpblxn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hsfedjlx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uzjthggl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sewaxosk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ypaeoard.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2esvuzjzi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ctchpmau.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2hsbbsoaq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gdmjbbau.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ldcpotid.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2blrcbpxk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2juhqbima.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bcnjiubd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2shjlyqvy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xjuwtmth.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ufnlhqdp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tgiexsil.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ncrnsewc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2jyuojmfe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2obdckoup.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vrvixohw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2llkpvadu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ayedwsbi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2dmjpetej.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dmlsdnye.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2aworlovw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vmsmdrtn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2yeiaxmxn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2eskezgmz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbeoaqzv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qcelndti.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2eywuiioc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yeovgtvt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cstcyfyb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2upellmeh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2brgoswqy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2txijpasp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dkmhfnxt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fdrjiiyp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qdnewcgn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgkufpbg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2fbuqzezn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2prtjhmma.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2thxzgxyz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iherpnkn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2iszujrdv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kxufcjno.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eumysfrv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2atqmxxhs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2easdzgxv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2svlslvzz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2supvjddu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gpzojqhx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pwiyekjy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tuaqtzil.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mqqogoap.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lwklnfol.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ldigtrms.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jlhcbovn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ujcdirim.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2pdtlpgtm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kuwphxfq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2emhvlauk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qprkzsog.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vxgiwnii.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aaghdsvt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dkggxpwi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fvhwfjba.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fvuhqxcy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ajfottsi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mjxqabcx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pkiipluj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yjuyiplq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzannpxp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2eevtpkqg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uhmgjyay.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2exremiiw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2uphlllvh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kihkqrun.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2znmpnzcl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wwprmqtj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2nbtncveo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pggtvirf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hoxegcrc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ahubufdm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hrvfcine.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ooadrkok.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mqilkttc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hketxkqb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2appouzug.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rdmukopw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2aqwqzdyj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdijtdhs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dftfcpdl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2txifbupp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2inflzvqu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zmunrndu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zerdmygv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2fpxcnucv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2heugrajo.html


<!-- 参考信息 -->