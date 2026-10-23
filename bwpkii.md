代发 wailian999

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oyfntvwt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ixynahvy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3chcgxcwp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3mvkdisoe.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3izcamido.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mwhdygdq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjizxyh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mpcivqff.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3vnzhxekh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dfuxafrq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hfgxfbnv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3eojifetb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hayvnhnj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fdmievpo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wjaorcpy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3caqteecp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jdhltpst.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ochlaamb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3advujrei.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3loqldjvu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3unmmdwih.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dvsvnjxn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ymmxxfpv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3loyjvtiy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zogmtfom.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3edqbsvri.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pkqiqjjs.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nkkidear.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3crjtnvzl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3baumywgn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eitwllba.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3onsbzmuq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjdcjogf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhmuglkb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3dceztzgd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3htpkmnxu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3snhivtrt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jqfgyqxd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3eovjzzqg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xszofybh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3exlmenqn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqwuxor.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3bdnqthhe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vnhxkmuv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hamuiwom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nybkkvdv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3eyhiwqid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpszzxav.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3tsvmtfwu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3eeefwtnz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lgellgok.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xrllqbdy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3npgkzuba.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kslwskuz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ueozrgou.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3kicphker.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bgmozgxl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wpstkcga.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hfsdxuzg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlgeznwe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nebdrmqf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ptqwrxih.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dtoqzwsg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3dzssvsrq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tjiufako.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mfjyfdnx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tmxpeusj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bjcjfmcf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zddceldj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wmjkkbac.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnrjynh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzkqyubg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ozxvazvb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3eziyijua.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3oohdurfh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ytjtsqum.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3turshjfs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3uurzdawo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhsdfdpw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3akhvdmhi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3rkfogkut.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mnjdmtaq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3luhomdzi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pltdfpgl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qakydvuy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3tysjsvef.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3scryvwdc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpprcykk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3evkeshcs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcgqsorv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3fygbefpu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3awyjzrns.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffehackd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ipvcfeys.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tstxbcca.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gtpivqvp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcsxjrrw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3toxvpxiw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmjnbfym.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3neuhrrtv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3oilslcix.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlsokijd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hwldusxj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqaeypqk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cycujhzk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqeznvmo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3agyvaohz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejggcnwi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tbllqxks.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vmaauger.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivbljlbp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jjjpuffu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cxygaffw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ftkmgfyb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nloktmte.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ohtawxmk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mbwjiztz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3loaxttcm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3leyledky.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lzbkjyxn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3cspptwvh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3diyuglcp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ytqmjjtg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rfrfobes.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rshdlkrb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiybmnar.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bskvoxxn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kzuehmwc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yslcweyl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lzixakge.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cvvrspce.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3neshxffk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dwoadgwq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bzhivifa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wetwsoel.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3oynmitlj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oqrsqvwc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3stotmugm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vmjkebeh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xlyehzhf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3znlejaby.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nwxtzjhl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wjljwieo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3turnirdp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3saibrwoa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kqkhvspf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3mqevfukk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bkrtbvvw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cdqukukw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vtvgirxp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wnyqkwwm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3esqxfdfe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3estusuxs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ffgnfveo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3anborpmd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lphibyqp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sklnhvvi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gujkdukc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ebfehrzs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqubdgqb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hwzyleiy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rssunmud.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3vfxtrdxz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ljowowqs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rqhaoihz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3itdqnceq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3omktltso.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qtxhrkef.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cvqnuify.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgmnbntq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcdjfnv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivxpfhdm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qiyrgfqb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kimwwkwf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wnrbmooq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3epqfljeb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3dlboyott.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ngfunedu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qamagnmg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xyjfwsik.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lwaxvgxj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jqmpakiq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aoruefag.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nqucgbzn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zxloggxt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3rknclfqz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ykbgsngc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ifkgojvg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wkzjrzsu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xriwvasm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gyukhztv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vdvjoiwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbpqkdlm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qfbmzspi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtsosjdo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3trievzjt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pezhvmgl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3movhkxcd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dadxrtsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jktsnmfb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdykavkg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3berogziu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgjsqion.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mlkqupky.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lvrufmfd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3dsdzfwak.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfjkjjkz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3soaectyf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cukelvxq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qrzcudox.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwbhcyne.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ubrydgdf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3luimtgog.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xywpstgt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3aniovnjq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ybcltzst.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nkxbfpoh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvadvkeu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdkrwzja.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ptvpkyyi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3tkdivass.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3wuurchue.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3eltpudnb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jnjdmiyi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wfxtropi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzvgocsu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3brdpicpf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3mdrtlcnm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3sgmuypiw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zldlzpco.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcratsqc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ornnrnju.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kgowxkvn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3okpvaqlm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3iwymgmow.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kwfznzjm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3pnnukwzi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3brtmwetr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dqymvsml.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3eqenajpn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mijvdgaw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3jpafvcxm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nzkgcsll.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3skudduld.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oeeqduzv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ibnxsqhe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cxnmungf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3msppdkiy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3etphmkhj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vxmfkjnp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwlkuhj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udbqxhwz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cunelsgf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cwexrafq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rnlmltcy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3yyszcduc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmcmmbg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yozegspm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wkqyupao.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dptasxoe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3inwdmlwi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygynndbz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ueazttoa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3azbxneym.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvrsidf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pwbxkjvt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ilozhydp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fflhuoko.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bgzqxulk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3auesjcpz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qqupxzdo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dcfbwamq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqrhuklc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kcoddwwk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3laxgtres.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3djqtygoa.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3eswczvxl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wsatyxbq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3woumjpit.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hnlrjuqx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nsqraksu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3capsmwfp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xctacqln.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ffxxmkxk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fzlhegda.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3isrjqalz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3iixklrjc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3buobztva.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lbppkitl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ljpbgoxf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3yshfzmlf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rreuoqac.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3dnrvwppz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ftghwnnt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bljzvkfm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tqfzqwwb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3uvlladgn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3txusiqry.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ozdnzsru.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ehbulgjs.html


<!-- 参考信息 -->