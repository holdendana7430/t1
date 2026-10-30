代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gnarjbxcp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/ggbfhezlj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gdxklwfin.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gjyjlsdzz.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fehbvm.com/Article/details/grfgguivb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.zdbjq.cn/Article/details/gldkjmwvp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/grvkvnqjo.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gmqwlkrnf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.zdbjq.cn/Article/details/gtwxsimux.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gidwksgdf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/ghtxmkhgm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gbciupndz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fehbvm.com/Article/details/giehdjexz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gexbmnwyo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/gimcbhtws.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gbuqkkbkj.sHtML

[A26] 类型转换总览
来源：http://mobile.hesvh.cn/Article/details/gmpdsxtfb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gxihbqcdt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.hesvh.cn/Article/details/gihxldnuc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gdmqasqva.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/ghiqczmxt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gwjhuhwdz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gccopvsdk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gheeoutpr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/ghtgabztw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxzhlxqsh.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gaecsdrdj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grnahisbq.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gejgqawbo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gcechjrjq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gtvyippbo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gmaivmovs.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gegrxhfzm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/geclmrwhb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gmxserqtd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.hesvh.cn/Article/details/gomicrexu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gptflywcr.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/gjhqbxnrr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/ggcbjrhsb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gljdibfct.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gkhmwxawo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gkvwptobx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gwzifniye.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/gnbfawzay.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fehbvm.com/Article/details/gtvqlgixg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/ggtzzttmy.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gtgnwffoc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gvlkpbpdr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/godgexbwh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjuyuqzbv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gcshkmolz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtfpkpsle.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/gsrkmyywl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gwvcxaook.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gpteffibr.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gsjrkoakq.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gdxqeunuz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/geuygyrsz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gvtvbucfg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gmkomkzsx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/glctnwjwl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/glwqlytou.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/gilzlpest.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/giwtdzgsb.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gjjztxoyo.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gveusggyb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/geihezelo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gqotybebq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/geinkornn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/glarkemhp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gigsslkml.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.zdbjq.cn/Article/details/gnlkxhehg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gxnbecars.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gofniajwn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gdlmgpuej.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gpzhtyryd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gjdalcsoi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gsbumjxua.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/ghlmprtmc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gueazkdkh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gwudzyssk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gncfwnjno.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gzzshpksm.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzliuxepe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gumtujprb.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gwmphytzb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gvprkiovx.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gnoyzvbge.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gjejzpstd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gdkqiqfvq.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gvqjifegu.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gvmxhpjdq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gbjofxocd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gqxqmduxf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/ggsgvrwsg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gwajqrjbg.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/ggaqueatl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/goviwnjin.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gdshvyail.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gwdxzlegf.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gfzrcepev.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/giincrmjq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gvliqakgt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/guacpoozz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/guukurxrz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gatfysnsv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gfetubukk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/giiqyzhtj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gbmbpzdtx.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gzscmnxmq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gxybyrchm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gqxhhiepe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gqgovebxy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gzxaoucfq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/greisaogx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/ggmgmlbjt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gxevugzzh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gnbkflqii.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gscxcyyzy.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gvqobyash.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gvtlffrlq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gvlrafmyx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/geuekaacp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxycpfmlq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gqjikvmcl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gramewvnf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gfjyllglq.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gigobsuwh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gzsqpjbty.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gzdhzprxj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gceqpiuoo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gzbxmeqxv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gsjnfmfou.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gupweynee.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gdjzxlstt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gwhdmkgca.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/ghigszsqi.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gzqnobaxx.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gwmosrlbg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gqzstlcmw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gtdpohpga.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gktmuwubt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gvgijhrnh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gumoovbmh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gwspwssod.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gzlafxlap.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gtjtrkhro.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/grvxhsibv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gkmcqroqp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gmqgilfjk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gkuidnndt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gzyfqtbpo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gehzkdnxi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gzdzqpuid.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gashfrgfs.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gloyjmlsb.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gknwsgsap.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gokicmxvr.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvjaidacj.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ggxtouwsr.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/goszcdbxb.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gaihbvger.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gnfcuplcb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gjbccpsam.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/giqwhujvj.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gaurrwcyf.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gontmypba.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gdxqjmusn.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gxwndrlor.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gsyobdxrr.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/ggmlncvcy.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gjaxqvfmb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gynkmarmv.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gaucxutqh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwjochjkv.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gzfllubeq.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gskkowxjx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gorpgrqyw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ggywfoyoo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gnspxbzdo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gktdzcazd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gzngcrmov.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gjwrekjbh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gcbccsqlz.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gnyamfmia.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gnbsxiafo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gsfwnsudm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gojgcjupi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsuizabyx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gwippwybk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnwziiebb.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gjuylpdcr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gzuidlezn.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gvhsrywwx.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/grguwvxco.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gzwzcpyoj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/geljrckcw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gaxyzgomo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/ggdakwrfn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gozzaotqj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gcapneapm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gyqeqrnaj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gkihflzru.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gsvdedayj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gwwqbrunk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/ggpjilihk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gsebycxfa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/geltbaire.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gyuczuawd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdcwichfu.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gnbdmhiqh.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gskfelezo.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gaofsyikv.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/glhbuvljd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gujkitrbm.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/glbuvqjjx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gxghdkmzw.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gjrctmdag.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gvxwxtyja.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gegkgnbfd.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gkztbdmqp.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gvlojtrup.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gisuvpzpn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gqbmxsmav.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gsxayxhlk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gqqiolrfd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gflcqcown.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/glmxfbvon.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/glvvzluuh.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gnwbiqowk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gmryysijp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/ghyeqkrwe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gurxwdybo.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxbdhsnm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/goedyfjqf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gnudsjujl.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gozeribwl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gngizgjbq.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gddctqwft.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gwdklmmro.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gsmouvzpy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gkgqsjnli.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gpkfldsrh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gqrpfktqv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/ggcjpesuo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gkzcvmdtb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gelrfysen.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gbqxvpexh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/guphgsrnl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gucoxjjtp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/ghomukbjv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/ghyxwsvdc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gnkfgczws.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gzdithvar.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gyzgvnmde.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gyrsstmzi.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gwkjdupue.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gzqfwkpkw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gctpkqcxk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gwbjwskim.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gxbmthmpa.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gvhqsyhrr.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gmjblujku.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gxrauqkyd.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gpluelauf.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gjggkqetm.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/goefguzse.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gwkqbyqgs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/ghqpsxwmw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gwhjytvjm.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/ggvshdvrk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gfvdicckg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gizcobbeh.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gdhwftryi.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gvtmaktcd.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gakxqxjrx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gbinqyrzu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gfqwesqsp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gaqddgfow.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gpgsolrfx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gaewazsdp.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gpeacbcer.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/geskjqvoh.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gqkhxusrm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/grftuoyil.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gpwrvukwu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gfugduuda.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gdkbbxhky.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnfosxkyu.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gumfnqlob.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gjgjsgjyl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gmfexznik.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gxbiemuco.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/guthhjdou.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gloujtcun.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/ghfoaekxr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/giopbgykb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gexdgjavq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/glphgcyis.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/geecnmgbl.sHtML


<!-- 参考信息 -->