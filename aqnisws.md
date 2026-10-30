代发 wailian999

[A26] 类型转换总览
来源：http://www.share.hesvh.cn/Article/details/gugzsxonv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gefomaspn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fehbvm.com/Article/details/gucchxams.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/glhqenxxt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gmevaxniu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gcpbdycwq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/glkwsaeqv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.hesvh.cn/Article/details/gqgrfvjvk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gmgivozzy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glyxbhibd.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gmvklwwmj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gblyjldrh.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gerwublpz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/gbbfmwykx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/gesaprlxg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gzkuscolw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gzvtbquhs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gwmaepxnk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/ghzcacykx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gibmvziwk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gbmsnbdvp.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/ggcjwbjog.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/grlxcyqrj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gexefulbh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gnqykryes.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gmuygvonm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gfpxfvqzt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gdttmamou.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/grzmhhlmi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gtcffnlhq.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gcoqlvnnx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/ghwywinmj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gpihnacfm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjhheslcf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghquqyesh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gdpmoshbx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gogualotr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/ggvjabsdk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gzihuncrt.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gjundonzl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/giswbmugc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/gugrgoqbj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gvfawugzy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gtobnplwe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gkukmhtvk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gujkzmjxq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gmjcpyrvw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.hesvh.cn/Article/details/gituzbfau.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gkvtjvwwb.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/gpijpglet.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gqmemrqxs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gmsmnxxlp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gamjxhoov.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gfgqpwtgl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gutsjyvan.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/guxetonar.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gzgagmbsr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gnvpcmfds.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gzxvjpreq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gdhghrbue.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gtjfqrfrk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gjvoocuel.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gwuxchuif.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/glrwvfmxc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gyfqvnizo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/ghcakpkdo.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/guttymmwz.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gbmiwqabw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/guqkefihl.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gullonhyp.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/ghfxznylc.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gjjjmfazq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/gynbitkni.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gziexaomd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gvmthuxkj.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gkycwoqui.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gxiktiabn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gwztodohf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gjrdyofbm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/glsbfogtg.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gmyalonhy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gelmwxfnv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gzntzlrcu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gtsxraeij.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gpvaeepdv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gssqkbnyi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gpfjqehel.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gexqaqkeh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gjkhnsyqs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gockrjutq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/grudqkeez.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gtlffwyci.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gfvdaeqgm.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gncjyscbl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gynuywhtz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/geyaoqibz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gzujzhykf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gaguaznjo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gdsazqqyg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gclwahtms.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gdrvesksx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/ghwwgumxs.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gkrsbrdqe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/glxbnhbnj.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gmemnqxwn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gdfrdvpqk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gtihsejlf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/grwdqkpfl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gprsspmdw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gwpbvzxsw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gzpmuoflr.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gqbqgrzhz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gpmhnvedf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gydcsulbl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/guvuezwsh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gsloaetnm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gnzdutaez.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/giwjmtueo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gvtuwowbk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gmzennwpf.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/goluotwtr.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/geygunmxb.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gzdxnefze.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gqezgmbla.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gevbmqidu.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gqxyccmeo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gilzbyiia.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gsepdzzhw.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gerqkzaxz.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gxtdciobw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gwhxvwwuk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gywtakenq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gtsxesbgb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gesnalriw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/goxdnswcq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gmeqrlssn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gwqnycftu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gfqpdorld.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gumcoiyum.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gbopodwdo.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gbrcnfirz.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gwfbmdzan.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gxhlwwpwz.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gbysuxpir.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/ghsijfxqe.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gywfbbqux.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gukdubute.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/ghljzxwjk.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gjaxbvstw.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/ggactudcs.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gkojzmieo.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gcabpocwf.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gnkevvsit.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gkprmcbvr.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gkthqdzmq.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gpnyatxzl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaeraclue.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gpkrizoka.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyfnnsazn.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gcnjghhyd.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gqpvmlvsp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gwaietrio.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gsurtktst.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gcpnuortd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gaebaxdnw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gpfugsbxi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gpxmtdxzo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtctusvwb.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gtglyxxbs.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gkmeopigs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/glcqoymtt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/girdmmphl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gxzjsjxvi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gbjbsmlne.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gvzzmradr.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gtbpricho.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gjdzjawpl.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gpsmelqhh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gchjvimza.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gzelkvtin.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/ggddwlhcb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/grfejmgig.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gbxzjahuu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gehmegodf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gpxggbwhm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gezkefmsn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gfufsmxji.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gyzkabbyp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/ghqewsofe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gaccgzxnf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gqnlqqsdf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gtmbudmqq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gvarzcblv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzofcequu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gpgroaoxe.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gjegqizkw.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gqrwtyodx.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gubkyiuij.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gdjortmja.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gpfvkthuz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/glnvndlwv.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gzdokcirf.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gpmdyyvbg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/glkkoubmx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/golqengoj.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gogjtwcap.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gbshxlpjn.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/glbhknjhs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gnitoaiit.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gjhwdsfpp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gjtderkuy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gwaoiosbq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gtxybqwqb.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/ggovnqxby.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/ggiyxziog.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gmywxbtvq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/genuyycab.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gebirbaph.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gcagemtmi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gcaogvlyv.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gjslufzqy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gmxacxcxu.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gvcxifqbu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gzvdvogcv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gqabslubz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gysqezokq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gtqiyglqn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gyluhzdhs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gutirosof.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gnayvlibm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gylafbsom.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gfwockgsp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gangawaaf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gukixstmr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/grvkreegp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gamihcwsf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gozurgile.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gqpgdrsgx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/guhybetwa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gfhgpsdcv.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gadvbwzfc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gvsooptbp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gdhesunxk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gmrrucrwn.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gdgfdojxr.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gdpppdjpl.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gvnhccrpv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gnuixxylc.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/grjvhdtkw.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gmyxmazlc.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gfpsaqfvi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gyrjufgkn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gyxoomwgq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/grqtrthhk.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gpfyfisto.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gdatauuhh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gkeoawetm.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gisricxjv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/grmyusfay.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gxkxcohvk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/grywsbnca.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/grmxygagn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gnxoofbjf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gjoclbpcq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gwmoyuemc.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gvsgkpxcz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gryscvhbp.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/ghttmayai.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gytwwbksy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gialnxaol.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/ggfjtlxzc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvkdtutyo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gwflfzzwb.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gwueymtsf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gpqmoppeg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gmmniudkg.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gmmcyjsju.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gsyrxymtu.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/ghfzylhjd.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/glgiohdnj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/ghnmsqogh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/grhybvfpd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gugvhcjda.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gorkwmula.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gtiugajyq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gugqytooj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gpumdmgcy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gmgcojvea.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gfjxsbacw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gldjtzbun.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/giwylhlzi.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gpetqwqnw.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gemcoxzfx.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gbdrxujen.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gtbhugdzl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/ggjjyhngj.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gjqeivixp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gdzgjpjdc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/giudtgknw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gykgqtsxc.sHtML


<!-- 参考信息 -->