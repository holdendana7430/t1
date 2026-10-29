代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/ggzisbydj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gjelzagvw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/ggizmnhyb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/goumtjtiy.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/gmiilwdkn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.hesvh.cn/Article/details/ggikcwkii.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/gnyttesjt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/gxsbgmcez.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gccanqzeb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gnpmafmxh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/gtwwcxisr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gwsobrgsc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gldelmhwu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gddnaxcqx.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/gtpmjruft.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gynmtfpwb.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/gegtqiozi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/gofhanqgx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmhnkpixa.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gcaaypgyx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gvugxcors.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gfkuspbua.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gryvklytf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/gzguxeyws.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gjcooahir.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gwzahjbjk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gmeczfwla.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.zdbjq.cn/Article/details/gtvtxvusg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gqvtctsvi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gvxkgyvpv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/goritkxth.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gnptjquni.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gllouestl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gllhunrvf.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gacpowpsq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gvqmijwkk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gcsxtkcnb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gwawshnjp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gxcdldwil.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gitkvzvvp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/ggvtdlgqw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.hesvh.cn/Article/details/guzxccrdh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gqhllbsvy.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/ghcjlrnuf.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/guxeytuso.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.zdbjq.cn/Article/details/gqzivsmoz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/giatupavy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gombygdym.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gtipbvldd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/gkmvidmhr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gdmftiitc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/grhgcojwa.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gzhetyujp.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gpggzghos.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gegkpmdjo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gntzinuly.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gjxwbjxfx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gtrfzxjkd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgpfnfli.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/ghdhyfmoe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gotzazara.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gniafbcsv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gwekjwupy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsjcfraax.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gqaxweull.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gzggkgszp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gqzhwwgea.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/griuokfxw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gesqivfsp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gdzncyvaf.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/ghtsvqern.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gursjpdxt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/ggidlthyj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gkuhushnu.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gfgkqqkun.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gzwbwewoi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gqinyntfv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gwkhblyze.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gmeqsusxi.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gbjwuiemw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gmzilujtp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/gdndujjrx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gjyolaycd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gvajqdaeh.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gecwfvcyv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqapgunds.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gywpwsrlg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gwnnjvpge.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gqszqptib.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gzuxakqwl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gpnnctfww.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/glybgxokt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gtgqoxoev.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gzxridnrm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/ggxxrlwre.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gsfgbnfwy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gpgryopcr.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gziexgyuv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gbxbqbsjr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnwdkwtzk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gyuzzizme.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/goqwrupig.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gwlvklsss.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/ghvqfipgw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gzvfoihfk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gshvieone.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/ggvohqkql.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gsolxjhsl.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/ggsybnurp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxqtpjzxx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzlcpbfgt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gwjindvue.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/grxbspivp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gqdeolycv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gppdbilvp.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gkatpivmz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gyckpffaj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gfizxsgbl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/goerwgold.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gppemisis.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gsdehxzwk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gxxruapaj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gymawravd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gdccvtpyx.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gbamkpdjy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gkjxgwfeu.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gbquonxow.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gtybkwshf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gaajjtheo.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gdfmwyqtv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gyeplbyps.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxcognx.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gtyltsnyd.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/grxocyoad.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/glljetzit.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gwamylzcu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnotetgcy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gculbzphd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gbrivltms.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gjwkuosiy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gyjiebudt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/grmqlgflg.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gcigiscep.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gsfewyfhe.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gaofiayfg.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gjmosfhdz.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gufcekulf.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gnbhqrpkc.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gjzskspsp.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gugklybzk.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gddvawwlm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gtzpxrrev.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gylrledbb.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gicvywftd.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/grpjglaku.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gqsecfurb.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gxpgsncya.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gwcpjgpnk.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gmkbzoami.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gxpvkcooy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gayqnonti.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gzyhwvugk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grdddvufu.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gedhqfaia.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gxxkhlran.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gbuyccmud.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gadmykwzp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtnyimrpr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghmhxaewd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gpsjrzjiz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gukdcyjpw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ghqzwwytr.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gilfopfof.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/golfupyqa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gjoodzndj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzsyrnmdb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gjlwqabit.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gpnjjepwg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gwqznqfod.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/guuzmdzzb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gbwvjoeyr.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gamnbowad.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gwuaobcwl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/glafpgkfp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gfitgubes.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gtmyccjgs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gzjkoqogl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gptdhuaxn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/grbtzaxbt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gioavakvm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gopqyskbs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gilpwplch.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gvaebajrp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gdmqdvkfl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gcjboiyxf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gxsimeilo.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gdothqleg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gzkriuffo.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gpayybppc.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gvyrfhzkx.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gmhmdabww.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/ghbetuufw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gidvahrjy.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/glzsgipbh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gjzsljpcc.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gsuzmmvhw.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gcqeqhisv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gbnuvpvfu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gbtpssjxm.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/geabkdbsy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gdkryftdm.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gocywvxld.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/guomqonmf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gzzgcnllb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxndggzo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gkyvjpwea.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/ghfmlwgrb.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gqjqeycvs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gupijgyio.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gvmkwrbat.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gvegjgljv.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/ghvzrizpo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gaoqnjjiz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gcixqvwxr.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gzqqkfctr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gjhqzgujp.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gzbubsoiq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gnzpdqiql.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gdwamfprv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gigngupnv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gakfvlubf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/ghxtxnzam.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gzvecgybi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gprgipnjx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gibwiiron.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/geourxqcd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gohqrxbcf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/ghyfggumh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gyaarwhjg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/geohkmzgg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gbynsnwon.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gcpfravfz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/guvjltbkd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/grbfzxcvt.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gjfdcxexi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gtjflmihj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gpetphbme.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gwwzvxygm.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gqcbiovvg.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gnxalfcez.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gfreapvvd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gctlkstsj.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/ggyndlkhg.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gyakgbpnv.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gydszandv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gudeepeoa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gtqjwfrwy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gwwgvyvna.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gpueteigw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gncccouex.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gbnmrvmcc.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gfkfhhmuu.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gdfezppia.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gsgqfbpvc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gevcbfvif.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/ghfjxizby.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/ghfdigbac.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gnwjwrsry.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gmhzskjyj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gqwkmilfj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/ghxfazpeq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gfodbczlq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gjdxkglgc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gtjnjhfop.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gxhbakwmo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gkkfjorkb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gwxjzmfoe.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gdasennhe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gvekicvkz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gkxcpxtla.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gclhstwng.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gdmrgwmwe.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gxehlvcku.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gsmkneish.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gstziwryv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gsmejqfks.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gtxuzysdw.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gduapurea.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/ghyvqeeqb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gqlkshhwk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/grixqksrt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/ggcytajhu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gkukifeqh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/grluxykmx.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gdubtiuco.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/glfipegip.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gscahwfbh.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gvwemlugj.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/ggkdlueow.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gtialaezk.sHtML


<!-- 参考信息 -->