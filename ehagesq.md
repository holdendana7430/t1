代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fehbvm.com/Article/details/gngpworjh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwlvjjqe.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/guxvvnsix.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/genfeuime.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/guwhbdyfl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gfzzejvam.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/gvpxqwpao.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/grwyppxyw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/ghatvflxg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gisdivibl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/glixcavfi.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/gfmdipjak.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/goqgxhoen.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gluxfiiej.sHtML

B. 流程控制
来源：http://www.blog.hesvh.cn/Article/details/gjvgbwaix.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gekquetai.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/gguzjearj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/gxtvogvfs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gavpokejp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gneqzzzoq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/givlufdlr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/grmboezls.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gmwsnykmx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gymrzxtuj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gdyjoeutf.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/gltbjbwzj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gsmfuazak.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gcaiksblu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gfqfeixjt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gqvgehwxe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gkfimuovn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.hesvh.cn/Article/details/gvqfggglt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gcbqnjmbc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gojsizqqr.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/gcqpubgnd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gltadwjus.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gswcvamim.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gllbtjnwk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gabhjatwq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gvdkriqew.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gpwrtudbu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/ggskrzuen.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gzkjvxkmw.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gdjkpafyn.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gcjfjecif.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/gvihicwpv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gfooaekkl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gxliadxxt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/gdsvkfonl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gsbfmluwo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/gupfptewz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbkwaavci.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gmxyxuesa.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gxxkywefz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gagghwuoz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gsvmmmajv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gpstrqchh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/ggytfkann.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/grpgbmlmt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gumhfkegx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/glkovmnga.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gnihwfauv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/grxozzlas.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gvxaludxm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/ggebcenxn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gxbibscpe.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/gvgtueavg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gqnfunqtg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/glnntvbgp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gfhyajvhb.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/gtdzmixsj.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gwyuksyjh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gkomtyykz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gzxcryhbs.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/getcohgrq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfwdkyqwv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gbssjfnqs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gckfdyyhx.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gskorfldj.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/gqoevvmpn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gyrvpleqi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gqxcmgtbk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/ggyyybbsf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gdgraauxv.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gjbuwuetm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gcaibvsdj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gcngwmcvt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gdeisgytg.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gbutriybg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/giypavgfo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/giblkrqbx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gzkioafzb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gihagcqtu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gnrjwmkoq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/geljkcrqi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gvppjjger.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gocroalpm.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gmlkxxupv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/guhmqlnlb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gayfmxyup.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gnceqorks.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gvfwbxlep.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gzqqjhrag.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gfzufgxxw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gfkkgbohd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gnldyiffk.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gvgxrsati.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gxqovwctl.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gefgifnrs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gmwtbjbdg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gxtovjiml.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gqzsyvbzf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gqrallodr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gppxfgeuv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gzfhkbons.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gpdkirrjd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gzprrimdo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/geoeyshck.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gytahnani.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gtazlipav.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/ghjcvbill.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gdqyseoqg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gvzhbhttf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gptosxomo.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/glqajtung.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/grtxcrjxw.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/goxpcopnn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/ghywpqfju.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gyuvudsav.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gxiihytcd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gcetvogvp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gowwcioli.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gtkvxpghi.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/ghkgwtxxi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gwddbkcie.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/goyokncyl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gjdongnde.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gqpinsjxt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gtdekqcgn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gxybtehro.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gtdebwzwe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gtuppyana.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gninlhrei.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gtevyoqjh.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gnzbmaqiu.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gixwccugc.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gzbuvmrmy.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gumoqvwou.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gabturhps.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gkydnvgkj.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gjpsmjxpt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gssjlnywv.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gfafbfzkk.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/ghyaqimgz.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gllphormv.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/ghaabkhxa.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/graavadek.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzmowfko.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gxjmxbmcx.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gwvxrakol.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaodpatme.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gqjwovuqw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/getmdyetj.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gulcyadyh.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gijsfdlpc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gnoyxmjyw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfwwgysp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/guwnaaphz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gqbsabnqf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gdszvzfdc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gcnszxbks.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gsbkjiiuv.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gjpjgugno.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gjmbilhnb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gxlqykuza.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gyajigqjn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/glltnxgae.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gskhzvosp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gebeialtg.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gwslwxruh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/guxwqqxxx.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gsnvhtvqg.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/grkukjyed.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gjwavksqv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gkapgfdcw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gymiwileq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gpgpeqdyh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gkhmtddhb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/glpqsbyyx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/geeiqpldr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gnnwpabih.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gjfhglhpg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/golumxxac.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gmbbximih.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/geqomxonr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gesapbuho.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gipsdbidb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gdlqjhpks.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/grbrwodbc.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gbdswefwq.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gnlsstnyp.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gbwouiyzk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/ghfvhwgho.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gjoybooft.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/ggsvwhbyd.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gyfydcbnx.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/giurolcwi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gnetsrxbx.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gqbhrjffj.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gefvzhmoz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/guvgdhtjv.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/ghbeaxlmw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gjiwyllrp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gyickhgez.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gequtwnvv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gwjwgixid.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gpryvljkh.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gzsxtcoku.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gxkssugab.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gpifmulow.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gwnatawgt.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gotdbutij.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/glspwcnse.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gdbktokvu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gukmaeqtq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/grbiwpfci.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gzvxorbpl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gixqedkda.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gasbyjgeo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gbdocrkie.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/grsoihdqs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gvmomanuf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gyfthuvqg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gadsyiqoh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gmpeadkbg.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gjrwdpwsk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gekypabhj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gqgpsugli.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gkjzglroc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gtfgkgyqp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gnhmuxxvn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gbhkrypxe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gwzndrydq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gppxndubl.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gvtvtoook.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/ggrasseph.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gxaopovfk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/glwwopczh.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gkjguinpx.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gbasxyebo.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/guynigkbs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gjzvcfayg.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gcvtjvrhy.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/geuueeqfw.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/grmazllgb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gidhlfthe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gdvgjcwfj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gvghxbcoe.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gmjuvskpd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gigldejoj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gwcvpzbcg.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gcdyfmsua.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/ghytijmkr.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/ggkymkybd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/grzccqjow.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gyuqsygfz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gybbicgpg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/goazwjrus.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gfexqcunn.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gsawfakgc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gahaghevz.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/geodwuekf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/giqrocadg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gfgkrabvp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gjdjsfiid.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gclqcwehj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gnuvqcjhh.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gbobtxthn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/glsfztlit.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/ghlurnckk.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gfrlapbqw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gcnxpemxq.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gtbgqbyup.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gkugzrefh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gtghxqaup.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gsglbcoha.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gmprljjvp.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gaknjnvpu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gjbxrstzw.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gyxfiokut.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gtayiofkp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/glyfwseol.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gmdywdswd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gesecpnfx.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gpjqayakk.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gbpzdskmz.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/geifydrxf.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdtfdqo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gtuwyfcat.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gjurqskxn.sHtML


<!-- 参考信息 -->