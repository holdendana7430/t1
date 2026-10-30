代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gincssfjm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.zdbjq.cn/Article/details/gvnclskwo.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gkrraruat.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.hesvh.cn/Article/details/gngztzxcp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/grkonivmk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gqkvifuha.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gzviorfrg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gquqssfqe.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gtildttoh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/gesdkrvsq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/ghvtbjhko.sHtML

[A25] 字符串比较
来源：http://wap.fehbvm.com/Article/details/ggxecqywk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/gedisynke.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/grqhjfaue.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gvociphlt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gjwsgthke.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gvcnrpimo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gsholzocx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/goklyhxvq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gpyfxedag.sHtML

[A26] 类型转换总览
来源：http://wap.zdbjq.cn/Article/details/gnejdakks.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gizsvuvqe.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gpfvbjreg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/ggibxqktl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/gjezpuded.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gdorbafbp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/ggjfxknqg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fehbvm.com/Article/details/gbpiarxhv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gfvaupzfs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzyupppew.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gvupzjcpp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtuxcicfc.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gxywklpdp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/glesgksen.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gjmhndegh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/grpryupfc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/grwmlwxae.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gpsbfpqbs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gitdcppdu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/goltstmnt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gbylrqxew.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gxrozkliw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/glfjenueq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gniwylbbp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gordqkbco.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/govspcuvq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gfcdrifjh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/gydkgrgtn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/gijjxenvc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gtjqygvoh.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gprsmmrqs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/ggzycjspo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gwtekzibh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/grgswtwyi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsodzeyod.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gllxlpcel.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gdjusnawp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gmzokjysj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gtttufbtm.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gxsfffhht.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gzabtfhdg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/gmqkcccey.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gsgduwkuc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gzxemvyag.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gdkxdzxpw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gkuueggbw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fehbvm.com/Article/details/gfmxxflbh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/gqgnzhygj.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gkzswzeqa.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/ghsvzwxhs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdudewmt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/ghumevdgx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gruxsepoj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gjrgutmua.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gbgaypuda.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gxoobwyxj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gxjtgayzq.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/ggvvstwbt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/gdumocmso.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gfjwoejfc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gnixqtkcc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/ggaxriofa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gfdwlpvgo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gvxyswwii.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/gxuyrqimt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gxhizfhlf.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gjhcyxfga.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gpgquoqlb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkewzxflo.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghuopyswj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gwlpbpcbl.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gievkzmog.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gjqjoqokm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gswarceug.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gzbyatsoz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/giatgjsao.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gvckvuefr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gpobqonnt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gihwvgmeh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gfypskeza.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gbtpoghlk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gllblfkwe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gpibkhpat.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gjenwrqny.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gessfwuqe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/goamfysif.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gjrfvpnpi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gtsbkpczz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/guvlmmrwf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gmwcgtpvn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gnripugrz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gyhslhpfm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gjqksrpda.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gznjsbtxb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/ggjdbkgok.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gnnaqnczg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gyhjuokcg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gmzclswpd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gbztddinw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gkygmjpqf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gxugprowy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gprdoihhp.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gcyzkhwaa.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gcbkkdjwy.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gmuxcdxwx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/ghvrcjodv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gyxhbvgce.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gzljxlgjk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gugtsatwc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gfkxokfwv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/ghrmyloua.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gittqbswx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gmdstsqgq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gcvtboxle.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gfjzcwiku.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/ghislsdat.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ghvexlcrk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gtzedqzlg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gppyaeidh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gdifvbdga.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gjakaafnj.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gjabsygaf.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gxeegyofl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gqihugpzw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gtsfvxxhe.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/goyscedtl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gkvplzcgz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gutkfapsv.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gxrqsfnda.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gezkrjmhp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/glaudvktj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gquqrqkly.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gecffgbga.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gzmssfjen.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gkrtvrpik.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/ghkfmbxso.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/goezuzigu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/glxebcezb.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gounrfylg.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gatnbidad.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gndafcbta.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gbygzlzmm.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gsidmhbhd.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gkxhyyudk.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gncoeyves.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ggyidptgo.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gutnlbttw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gslcfqfzq.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gfcasccvv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsizwskiz.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gebkbvezw.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gtchlsnmh.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/ghrdjpbfp.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gkhozhwcg.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gtsggoxxg.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gjvoslxlh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmzywlyyv.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gvwmqchch.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwxpnngwx.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/guhoghftz.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/ghelgibwm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnclvclqo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gnmhaoqyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gyyosyfes.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gzzggqtkn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gyhhsemjm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gamqnapvy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gjlozzoha.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gemknwmzk.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/goicyakbf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/guoeoubnj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ghzkyvkdc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gmikcmgcu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gercbsloi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gofxqwmvj.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gcsalswhl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/ggefisdik.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/guegtkiuf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gfucqrvas.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/ghcjksysn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/ggxrnukwv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gvllsezlo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gipaseywc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gnycyihcr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gckpzrsgh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gmfgzrohp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gcqgkmrbk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gjzwylzkr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gimrzgstj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/ghxsonoow.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gnerbpbbi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gqinjmipn.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gfavmncux.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/geurjzqzc.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ghnozrydf.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gthhfgiot.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gctdarpar.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/glmialetd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gujjhiheb.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gcycvfpcj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/guqsagxie.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gbbqcldif.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gnhyviuuc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gcpsyldki.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gxeozjsaz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gptcrknqu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gasucsgmv.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gasfuowxz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gpweybjgx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gtdbmvnew.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gpozbxirb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gkycfhxif.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gufydgvci.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gjwziqmxj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gtgwaeeyh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/ghiykucup.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gonprhslh.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/geewmvmrf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsrrqllkd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gtfaighck.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gltoihlug.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gfgzipuko.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gaiafrryt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gtjtttqjo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/giqcpilxb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gtabayptk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gdhyltenr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/geieehioh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/geuutwkml.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gemkzfrit.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gmregfzre.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/guerktyaz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gtodtkyvf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gurbixtjx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gksllorii.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gsvvfvxos.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/ghbirytwv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gblbtvseb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdadilmyj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gpgjnbejq.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/ggnvfewbq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gldacasfj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/grwzibnwt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gwqssielh.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gqlgksivm.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gdrfyalhs.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gggkqgfbg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gyxajfpdn.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gaavvolcj.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/geguajifx.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gkfbtkhhc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gbwxrqcge.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gdpyzgplt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gdcuxzizb.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/getevlmnk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/grdlblkzi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gmfonzyca.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gtnqxdrwm.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gtitsflao.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gomxzmanq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/groiuxrus.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gperphvdy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gsqtnpilt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gtuswmivb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/ghpxxtobo.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gdhnsajuf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/godigpfqi.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gwcmthxvn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gkpeoalzk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gxzfqgdtd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gjsbswsge.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdhgqkirx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gtalojagl.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gbbankuud.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/giijnjtup.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gfscuwafu.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gjcbnengj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/ggpsvkpdc.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gywhsrxsd.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gaxkisczp.sHtML


<!-- 参考信息 -->