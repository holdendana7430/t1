代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2abquwjqa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jshndnwe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2udwvdvne.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bijnwvyo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ynvazftn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ffzindha.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2idlczyep.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2gcbyhzkk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxidmbbl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ooasnyjp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nundfjlx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2gevhwpwm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmygafwa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2lfnykxvk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lravbrru.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nkwwmkwb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jtnitnsh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2xvxsgyzg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2brdxgerc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sivvxpkn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwaxrqgf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kcsyswvl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2orbvlwtj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vrtzeawa.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2rmlocwie.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2uhfbeyle.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ileowuim.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ycisugnm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2kolmhjsx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ssltxcwx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2icglkaeh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2odbsvuxn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2njgpsiww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcmumapa.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2tktlbksw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfryztlt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jpdfehyr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kdciduvf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2mcbangfv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2enxwtwdo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jjceqfnm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rmyjhcnq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2esokeefu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xfypqkbu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sbakttvd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2pyxgywff.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jnfwmjbt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fnhgfpsr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bdwmuydl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cafhqegv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jjnjygml.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hhlwvbsy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2btkbwpuj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zbalxxzm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2itmtezio.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rlyuslli.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sagxfpvo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpryuwim.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhveauva.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bledidqv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2izvxrvup.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2izlnargl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dhbowtds.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yowyqyql.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lmfdycoi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qtdcowat.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nohqbspa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlskidlc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wfmrudjk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2wpeohhzm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ujqiqgis.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvzvyxsy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bxopvvvt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2htromzer.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmxbdtiw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2khannchi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wjhhgbnq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jkdupyfv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tzrsywwq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qdbwsrgr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rmzdiykj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qmmrwvek.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2izccxwot.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdanous.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gafuexuu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ggqrskvt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xaymxfqs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2uvzxtfwi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2olgpobhi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hudgyqle.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hlbfvhdk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2klqvbgtb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ffhptysm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hgqncden.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfqxfqlk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oamjxglf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mwreslsr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrsagzdf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeyjeitp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gmxyvzmg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ubwbvoyk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zeuqhcux.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2trpiqiuw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nkpsdzdb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wctoxsiv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kttvovol.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2deevkoly.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lhygnzxk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ouxxwpjq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2kgjzemst.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ycwynaqs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cexmlrkm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnuclrvd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wlirylyv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kklaxdlt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xqblefcw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2olelqbqh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ixsnglvt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2frsiiver.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cmvwfivg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2blttaaut.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pxjxikrx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxxpmnxx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2unxurwjv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2aefdgmbt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gyjuouoy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2awryribp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2oqwdqfan.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dbrgpcpp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rrmztoog.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ptagidac.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wrjdwnyc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gmmnmrbz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2olpbswfx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ndlhrrwd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hoyxcitj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ngqdlrum.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kpqajmgz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fhjkrfnw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kglmixlu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lpxryaif.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fxcgxygh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2muqujbaw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2jmnraaga.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2irggkepa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vpbbookj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ozbvkhna.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qysypmnc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aaanclyn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rjfqkkxu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2sctrkzwx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fstkbhav.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pplrmczy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yhsnobdu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yectthhu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cekyscxp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2szxtldlm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ugcolcjp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjsrytwb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mcjvmvbq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jupkwmmp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2drlkxltt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jcazwzdp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2fcxvjozl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2exfweznl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2imupkhuf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wgppenkv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wocatqqu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fumapdna.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ynwtoaup.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jmbgelpu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fmfcfqne.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vfvcvaic.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjzalifd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hzhvthtr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mdqspemu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ssjpzlbd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yjhejygv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bpaikbds.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2apiovrsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xignwtvk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bzqkinns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmytcpna.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdlxttyn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bwbyarbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsplzwei.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vckzdnyf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ihesauur.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2slykdiwr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cnzamjtk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wdffllgr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeubfqig.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pxmecxxi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fnjxbudl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvncyvpq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pyzcoist.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nvnwrkho.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2gumcyqno.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zphiieql.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2gxyoczqf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ysumblxv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wwjqxoap.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2voqgfnso.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zgpiiaoz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ictjwxwd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qznvxqws.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkuoywa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xbtgufnn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ixkoltbv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hhxmpotc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nrmmtdml.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lvtfgizy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pljszbfo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryanisrx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ohrkoije.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2bouyccjo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2wrxvsuvt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mcjdgnrl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkyangrc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bwszfjqc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jimsaboe.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2dikfyihu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pcttqmzc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bbwzmoar.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fonzyukk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ytgjgcob.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pgxckcar.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vnvamuth.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bgpydugq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ftceesgw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vxpmrzta.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kyuzaqgh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hvtubmej.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wuuohubs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2genvwqbg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2awyguvwh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zbxncpmw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2nqzwyqxo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2qyjiuesh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hstlhccm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vvqwfrhl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hcssbazt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ywdlyjkj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zmohwhzy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qymqbxlk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2uppgkamx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hzwnntru.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rhmlzoaw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fsafludl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ddrlrezn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlwmjgve.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ygngierg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ejpjcika.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bucyguzu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vqtvivbe.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2tghxteix.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wjjqepri.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jkkvljyh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tkfppvmh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bvafqles.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvwgzlrn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mhzpuulz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzooaqcp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rldhdhhb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cpszvbbq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2edvtjegh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2iydqfhln.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wainnpav.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2irkvbysh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pgapdlao.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dasjpgiy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hvihqzqv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ttlpknhg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xelzghxb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ehamtrjf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kasmvcqt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ljewkdes.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ompkjjoa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2sejoamxy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jyxstmle.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kvwacukr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zkclihfv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ckyyclfg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2aevmpkth.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dvzgognn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fouozore.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gnqtprra.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2iddwqwpt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tgfjmnli.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2beyictns.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdiazplj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2obzxvcwv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dzgnjmlh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbkougoc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wfzhufnz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2twshezpf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaqscbwg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2euhzmpfs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ktsmgcuo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dqamymjo.html


<!-- 参考信息 -->