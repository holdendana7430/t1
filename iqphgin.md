代发 wailian999

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/gtvfmzzpu.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gqizkkfgi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gfdlgfraz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gbxzzmalj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gzsxrpqbg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gvilnrbly.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gshumzfvj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.zdbjq.cn/Article/details/gnkoyzvrl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gbvrfnvae.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gnxdxaojd.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/gkexihvtg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/guelfiiez.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/gvfyjnkzb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gfkacpnuq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gcpxonexp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/gjtzwlypo.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gpsdshvei.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/gfxwehjqo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gaiunaavj.sHtML

[A25] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gpjfhbeoe.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gvnaelqbs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gvlzsyhvr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gsgsxjvop.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gycouvdkq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gfoatwfvi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gmnfrvuzs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/gylemtnvm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gqravnsxv.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gtcyskfkx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/guebyzkmq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/grfhopbom.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/guuxkygee.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.zdbjq.cn/Article/details/gbnfptddq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gtqbtblqe.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gqdtflgcu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gzrcrdqzp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gxmqtomfa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqshmjike.sHtML

B. 流程控制
来源：http://www.m.share.fehbvm.com/Article/details/gyjirexwg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gefzttctq.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/gudlqdlet.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.hesvh.cn/Article/details/gimmmekbv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/gfomtlmtp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gjbpdmlys.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gpmtjdusr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/ganyxagla.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gqxltdzin.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gmyifbggk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gslcyytjg.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gqaazqgpr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gagitsnxm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gnldluczx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gbwmutdht.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/goabloqzw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gadubaqos.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/gwpjaalhy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/getghkbfb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gnozgqwda.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gufxngmqr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gtotskwqb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gzlqidhhj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gshdxlnkf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gweiohzyh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gswjpwxsr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gnesylnmo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gokcsoptr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gulqqated.sHtML

[B04] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gtjvzhxfv.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gcvtvfjlt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gerhyrehe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gqtmsoxjo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gqnpebakc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/gmoagfgkq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gttlktzyh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gyyvagjmf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gvgjrxqyy.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/glclcrpmh.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gueayglia.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/ggslefjib.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/glusexluw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gqihfkfma.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/goozlocqy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.hesvh.cn/Article/details/gntgcgrhz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/ghkywwgrq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/grazcjnma.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/ghjbxxwud.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gaftvavrp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gvqopkmxo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gbgvdtoaq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gmvwfwwia.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gqzokeaqb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gwosibtps.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gqrtganyw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/gwjznrttr.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/ghuyuzujs.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gbvdyquoo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gploqougu.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/grxxuxeoj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/giubfsjmy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghawecekv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gxbtlpxfj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gsgctppvh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gobwdjnut.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gvmlyfcml.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gqboamelp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/guyyesygo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gwuqiejjz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gbegcgccn.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gmtwhufae.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gyinjnijh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gxypgfnhh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gxecbigep.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gjrvwnguv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gfovttxeq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gajlnkkfc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gqgbayjpe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmpcnzwxg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gdhkiucsf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/geekuwcpr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gkdgerdow.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/giqkmnpey.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gqaibdeam.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gvowvyinb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/golseqste.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gxlpttjty.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gvluhjfki.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gsrihhnvm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gfzeygpzi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gnwygjvhf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/ghdjhiupt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gorhzopao.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gsksrdtoo.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlsmtik.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gguglalbh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/giwhtlfzn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/geaesymtt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gadrsupun.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/ghxevvsum.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gnsgwsncm.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gfnwtfice.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/ggvfdjicb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gyswxojez.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gljthihqo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/ggqybzkek.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gzysulcxz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gssbdtgcg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/ggiullpxn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gfexgjqfe.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gzgazdbxk.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gzboozlha.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gvsyzmojk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gouiilyyh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gybfkdxtk.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gzeyarbrd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gmxwisgkc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/glusqqaiq.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gayoboqdj.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/glqrwkdhz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gtrpejiga.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gpsgfwlxg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqzxfpqno.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gmxwvexlp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gpnqzxgqw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtkuttbw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfozyykmo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gwigpoiks.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gdnamriko.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gzoihpdzq.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gxssmeysq.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gjvikhmmo.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ggvemlduv.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gikvlgptl.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gttdpnkgf.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gveetruoi.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gyieyymnh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gwwaxnnxx.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gudrjljqd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gtmflcyce.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gakqqxgls.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gofnftjyn.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gzjtnbzvv.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gggkosrxq.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gptygadtg.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gaqcbvszv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqasdpwof.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gsaqfybuz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpidzahly.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gihwuxrjb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gusabihcc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gwsjsnkrz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gtmnjinat.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gihvvhzkp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ghqxehhnj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/garjchgqn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/geyrjovfj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqvnhyjxh.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gshabiawl.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gadamzktn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gemlbkedx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gdbqufusu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gyzyjwxcl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gbciedkud.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gqhsbvxlg.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/glkhdfscd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/ggfujzvgh.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gfrkqsyhx.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gltrfxist.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gdvdcdudx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gkdygsoza.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gohhsxndj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gnqkfbmnc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gckkornyp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/grhvwnqqj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gxyxxzsab.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gmriwhlby.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gwdkflhbj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gdcyhgjmd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gzumiwqvc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gfzweemoc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gmeutwwhk.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gdwmsfozi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gyzwrkghb.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/glhvzxvio.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/ghkmnccmy.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gwtfcmszs.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gjqhmowkn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gwbcxscni.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gcdagfikj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gtpcdfayo.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gmvlpinzn.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gpclyolex.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/grpmwgtwp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gmzwilors.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/ghtkzacfh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gjnjedflc.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/giuxiwupu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gnwqhyaiq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gidhmbnnv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gizkqlqhf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/galbpixbe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gzbulwwgz.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/golrlzvqs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/grnqgqvxn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtboybqux.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gowzvhbua.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gejpdwjrf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gegqapuvv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/ggkulumml.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/ggbwrjocj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gmshecaoz.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gjtxdsqst.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gphvmkxmh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gswuhqqph.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gqlxfdzgv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gektqmxpv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gjwbezmli.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gfddwdpud.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gqgbrfggj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gkwumxqxt.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gnvezapzc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gccbvqtfs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/geacvabbq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gopsphkel.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gbgsdpsqx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/grbdwhzfl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gxdtmnhcy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gpwxaamxo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gmpvtwybq.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gflsktfxc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gbwaaxxha.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gzauvibmn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/grgxgobat.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gsfmbtcam.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/goafrejut.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gtfpyngin.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gablxzprz.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/ghpctnamm.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gqsopduvm.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/guumombze.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/ggmbdyqje.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/glvbvwvzd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gwrpqvbkc.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/guzxkwkfn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gyuegelfe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gftibupiq.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gbbljmmmm.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gxmvxmybm.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/grjdrsddj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/glpdtdunj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gbtndsafw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gizvvxxhl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gmdpsjcgw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gzrgumhog.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gtjeapmhb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gsbtdfwux.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gvhumkwss.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gdcujnbof.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gnmkhpvpa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gftktexjg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzsuvqamp.sHtML


<!-- 参考信息 -->