代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/ggjxmbubg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gqyyeajaz.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gktbjgxep.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/giuofdqke.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gazdjfalb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gtdomiypg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gtnilaovt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/gvsbpzwzp.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.zdbjq.cn/Article/details/gxqqnloww.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/gghcmnpad.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fehbvm.com/Article/details/gfsonypsg.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gtoelouhm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.zdbjq.cn/Article/details/gjlscmyhf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/gigfegzes.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gilsxnjah.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gujzqxyio.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/ghodtulbt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gmjznsudz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.hesvh.cn/Article/details/gimysnqze.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gxqkslkve.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gwwygmgni.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/gcyckuiea.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.zdbjq.cn/Article/details/gyeqncmmn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gjjjdtezs.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/givqkxrau.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gmvpiukqr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.zdbjq.cn/Article/details/gbgebixnv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/gckhnbkcu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/giakodxdp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtblnebau.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gdsablrqn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gugqkazer.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gwygffrmy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gwdkpipxx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/geeaczmpn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gmxnjjqxc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gbdqtckjh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/ggmqbejho.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gxpohpcne.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gdzmrlsxu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gycnzyyzx.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gieaimesh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gwmrlqqyn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gbdpfyplx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gysjwabty.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gxfsklykh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gohnqzdqc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/gdarfsgdi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gfzmmxupm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gsfyddawi.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gdaxyerkr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/gkeadudgs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/glgogueko.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gekhhndmh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gveegzyqi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gqrfvxfbl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gwrdfcxdk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gymvplqpr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/gdnphdjcz.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gwiuwjhks.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gmxaelbpj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gpaslmpca.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gsvinqqdn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gievpysvs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/geeaomlkc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/ghyhakjyl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gaiqpjgvy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/geqhynnkb.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gqfhymlyg.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gfrnnxvzs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gllpizdti.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gvxpsvdvy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gdfgpbylf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/ggjrgndva.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/geuplwqxf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/govskjtbw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gwiywkxsv.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/ghggkjfkl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gwsmaumnq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/glqcpdmmw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/guhmqghqp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/genbwnhav.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/guvyzadbi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gvhltpvxp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gnwrmxecl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gujuvapuo.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gavpevpkg.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gatlseqwr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/ggfbmsocs.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/ggwdprwyy.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gkpzwzipy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gmjmmwmpq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gxrjtgqmq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/glakgzxbn.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gtxdareaw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gcsdhayed.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gfpdmzoyg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/guwujbpxc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gykqopotz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gytbcflww.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gkuyyummi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/grqofoytw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gdepucdcl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gswwjshus.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gatqqtzid.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gcaibgckb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gumxjffdu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gyjvejwpo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gscovpcsp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/grwwkpbqr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gnjfihguf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gxtycilvn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gkcvwykwh.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/grxwstezc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gtmyvsfvj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gnstggrmb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/giexhhdad.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gstxgvtzm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/goyikopll.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gydftbtam.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gsglcpgzj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/glgomfuvb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gurwzrvvn.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/glizvegox.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gjccyvzgd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gadrnnpjp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gysornfys.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gglpqrppd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gqkzjdtbc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gbmseapbr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/glwlzkwyf.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gnjgixudz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gnqoymben.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gdozshatx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gdukuiiqj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gtefzxeaf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/glveiaabp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gnsoyoucn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gkbcplzhu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gokpqcdfz.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gwrbsauho.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/grqbfcqlx.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gudumpkal.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gwfrjrmnj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gjzzrusqk.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gykbmwfyz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gjkpjztpx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gawdbzoql.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gbgrjuqjf.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/grykcnjwn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gkrnjbtvd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gkyiglzam.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gmuzfabqa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gbhnzbnit.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gjhxdqpft.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gayasecrt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gaelpokew.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gfxgrroht.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gezhvjdax.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gyosnnnkk.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gvxaclzhu.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gjmnolbpb.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gidsduiay.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gawibhale.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gbgpzqqmr.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gkbrnhwqt.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/grxoebteg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/ghikufjil.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gwenyvfbi.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gctsyozlt.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggtzqjjlv.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gkejuqcav.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/giijecoxa.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gstrnqgtv.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gbvfjmyld.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gewngqupd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyncxzdad.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gzcivldap.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnujrfvyo.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/geewmehut.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gpvgdoifs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/glbusdtla.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ghxlvdsep.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvymvhpnw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gioyvnpbi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gmxsdjjio.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/ggnkltfbl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gedoptskk.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gyzoyherj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gtxynelvx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/giuscuitd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkubqsbso.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gdnzgptmm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gowwxtyse.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gseasswjw.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gznjrwkbi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/golbvvmcm.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gvjssnffw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gjiujimeg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxouapuy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gddjowdmy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gylpczilv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gctqjgeqp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gvwlffpfk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/graphopnh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gsjaiezkv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gzhtaozyi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gypolixor.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/ghmjerjpn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/glvzkixgl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gzejoashn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/grgcyyjxk.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gzopdzdle.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gutojnyrl.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gjtfxgwgt.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/ggivkasos.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gastyfjrm.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gxhawhqtz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/ggvaqtror.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gledwxwgv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gxbxgnzno.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gteauhqfa.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gbwsujemo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/grvqiqgmm.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gmqvbooec.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gqjccssin.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gsmilqhsz.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gvdcdpgxw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/garetudao.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gjnisgfvv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/glsagoadi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/glgvqasgb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggldewacy.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gofsyfuia.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gasnmyflg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwnipapwy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gsrromeqz.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gtfzewchr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gzvgrduiq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gjoatnskg.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gkxoghkwb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gmlxqnvsp.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gtnwsimtz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gqpbysltt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gigixvibs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/githguukd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gmqjeyzdo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/giiwixusk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gotgxblam.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/geezzdtxt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/grvaiopgk.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyuzdckqa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gaebeafjo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gfherapnt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/goyuzkuht.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gbdtrajsj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gekncsqwz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gcspncsia.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gmyhhvuct.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gplzpkqya.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gbodhadzk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gjrctkevr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gjssjzsbv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/ghtyvmckn.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gxigtcdyg.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gkglpumks.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/ghuocaxcb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/geqiehlft.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gxbsuhqvt.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/ghhznedaz.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gjqtmaugu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/glmykpzvu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/goxfznaju.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gpulvjwos.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gwdyqrkpx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/guecsrrtl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gnqygmxpb.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gpjbbogzr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gqddscikd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gdvrsfvpf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gcibpybwu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/ggxqyxrjc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gswxzcuus.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gbugdrvvz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gkuxkeflp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gocuuehhq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gfvfwghhe.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gadpkkoyz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gwurwkrpz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfcpbyesj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gdznvnlni.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gtbedlvmb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gohnxooux.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gxeizzvig.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gderthqwg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gdulvjrxt.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gincnjxzr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gmrxgdhue.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gnbeiclfq.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/grjppupxu.sHtML


<!-- 参考信息 -->