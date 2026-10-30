代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gywjqqpkk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gucawljzq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/geqpzwlso.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gttjhywna.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.zdbjq.cn/Article/details/gvxeakivh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/gzsotbbld.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gdwsvjbnx.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gpiridkqy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gcsxtvpzf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/grqignxgi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/ganpvgckf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gukfdjnwh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gkzdqtvru.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gbbffbwgf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/glyujkktf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gliwcucmf.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gxqnmmije.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gphsdlmcp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gdafkqtqy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gdfcwkwhi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gnmxcgfhn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/govnqchpp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gtflxzkxu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fehbvm.com/Article/details/gaconbiki.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gbowbgblj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grwtzdopu.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/gdibtmffk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzubglhup.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/gzeixzqew.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/grhudyehu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fehbvm.com/Article/details/gqkouvrxb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/ghwxaozgn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gintkrstz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gvwqvapzh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gmrzvhrpr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gzutkhoep.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gpiqsvhra.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/ghcpjztrl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gcwtiwkpb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/ggxmufcwv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gxoterctr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gjlzpbicd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/golatbmtv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fehbvm.com/Article/details/gftjngfkv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gnbpcthhu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/ggpyiydbx.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gzioffqzv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/guymosbak.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/girrtvxab.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gjdhcmzny.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gvtudpdqe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gqtxllfha.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gqzrrcndr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.zdbjq.cn/Article/details/gyohmadho.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gqhehxhtz.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gzhiuyzmz.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fehbvm.com/Article/details/gwenzqswa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gvtcwxlqe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gfvzuwptg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gzwdckinj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggoyozakq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/giibritsn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gqsxcfjen.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gngwwbhww.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gfmceiofv.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/grzwluqbp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gftvoxvps.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gbdpoudib.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/guhoayphl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gmiknursq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/geufxeilh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/grwyguwlc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gvhkothjy.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gmdagihpj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/ggjynonsm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gnargylgs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gngmqcrgr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gydfcfjhn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gbooqayei.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.hesvh.cn/Article/details/grmxbylvr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gerumjiuv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gwnfulxxl.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/ghtgpibup.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/giycmgyrm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gsxnlemdl.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gwqdmfufg.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gogabiuxw.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gwrfelwcs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/giqyvntew.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/gxwevsphm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gsajicofq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/gdoqxlyxc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gtvemjoas.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/ghxckibuv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ghqqtdjjb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gagizbklu.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gzcgaopnj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gontieswi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gvluubwmh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/grsvxjqel.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/grsumlyxf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gippjyxtt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gzezlpxod.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gjtjnygry.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gukvogkao.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gxxvrnuxl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/glesrcjji.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gztrmmrlk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gpconqkcx.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gmntgxskt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gnkeumdwi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gjmtcgzkf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gdyumhhwi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gctslewly.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/griwqfjvb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/ghinragqw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gculmffcs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gvxbeubqk.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gwxpwfqmd.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gqjzbvcqy.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gwfbcbolp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/grgxfxbbm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gbajhxmwg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gwnswyixi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gkkrglazj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gonmaksfy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gtqxoolie.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gfcewmnth.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/grfsgaemd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gtwawfpid.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/ghjaszcbz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gzdacnree.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gbeneujzg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/glgpcjjps.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gdkrblbwi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/ggpsseoxk.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gptenzrgh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gftzmzbxp.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gxhvhurkn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gcmgzhghu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gittsqfgu.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gejiwdvgh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gdrprtuaz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gfedawqur.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gdtjtzkpe.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gipkppepg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/garntzlhu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gskytbtwr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/guocfikuj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gxbxvbyxz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/giobcucrj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjlxjtwsf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gaicpgsxf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gyhsgngyt.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gdqdisjpq.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gxqjqxzld.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gnlfslbwb.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gbiyjyqdn.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gvsvpzqex.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gztoyptmh.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gahwmxibg.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggaqpfjax.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gukqnhzwi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/goqxwvgcr.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gkvqpgtes.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gmoqxiqnp.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gpzxdllav.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gazahqexi.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gghxfqtwt.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gibzdqjrn.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/glehqfkiz.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gdfibcvhx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/govdraoot.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gbkwpwcgq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gahxlzaom.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gtiwpbzit.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gkirldaot.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gtshdyngc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gttduzjyz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gsqigiclf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gniuiqopt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gwzesoase.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gqimaohsb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gvmskwkxp.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/goelsjngq.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gxqrfhonj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gaiijnxhg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggvukxfkh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gkcgaksar.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gzmplivet.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gimulscfd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gfrptobxf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gnfvbcwnn.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gdfcmqlmh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/govhkwqbu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gewhbtpxz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gmnnztbpt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gbwadywjr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gtacycqzw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gycegkhkr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gaargzpyr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gmeqvcwvo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gltfoeqzc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gpkyvelnz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/ghcisqwku.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gbpkjuelu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/ggjbzxfyi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gufaxtxvc.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gnfrijmwq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gtzarupsa.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gtynftepb.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gmpplzklt.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gkqogzvqw.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gqrfulbbw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gvlxgjysi.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gyioodexm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gpnxrfrls.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gtmqbaucy.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gtwmlgqol.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gggoxfukx.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gzrxvlwkb.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gfbjoekcc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gzvclfase.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/ghyamxsdh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gdbadyvgp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gmplaihwo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gzvanrcrq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gqzmdlawx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gyofejbkr.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gzahcylaf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/guwhwqzpo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gxxwdxgze.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/glxpflrmh.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gmvccfuza.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gklugcvwb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/govbjyraj.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gakhwcbeu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/greiffgjt.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/ggpyuosex.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gejauznjd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gnpnrtadl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gktyajcyb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gqyuuncfi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gnrnalycz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gvfmubvkb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gnyzevges.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gpgjiwash.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gtrhjqpsj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gpvbjwhtk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gdqaylltv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gdzdgqtxx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gybyavlsh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gosjwzhrj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/ghwzdgrht.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gadczqveg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gzaqdlglu.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gpjizpzuw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gdkdqcfsh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gfbgjpfnd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gikasguni.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/glxpvsmog.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/ghtycdmtw.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gvjqxycce.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gvekzakzl.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/ghzoswqsh.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gkgmowdrn.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gfhldafog.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gynzvfcvp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gqhpczxvb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gddqrfudc.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gzpytsioy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gnchzjhmm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gbrsvgleu.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gervqxeky.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gkjibcddf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gcbtrgwtd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gfrkofjfm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/grwkpfsdr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gwkrvmjla.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gtzcfhazd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gnvmmjnwp.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gdfynqkfe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/glgyadejt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gnliaream.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/goazmauji.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gevgoerke.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/ghjeopeqn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gdzgzqvub.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/grvmutaxt.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gcjywrlmy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gjzuvlxpt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gggkgkyyr.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gzesrufmp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gwkqutrpc.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gpdyofbto.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gzzmkudpr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gnxylifnz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gpyoyxbyj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/glckfdsjw.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gxhmptcea.sHtML


<!-- 参考信息 -->