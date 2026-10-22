代发 wailian999

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yfxsswiv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vvzlaggs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yywxhcri.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2osycjxby.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vilpflot.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hgjwuups.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xjkaulkm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytrfpypm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yqfvozsp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nxqeccnw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2oegmvyqx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dinqghzr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qdsvdfnh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2cmbbirzi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2snuexboq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2btjctjex.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fiewbwcv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dcjfqnqf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ngjrsuvn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2udjjimlv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2krgxezhe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2znayuxxi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gkaghzvg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2akujttvs.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2lydjbtgc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vocgtrtl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dhptpdyx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjypddoe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynfrnyty.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ilhxtbdx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cdrbypgf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cidppgcy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2uywnblcc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2chdaoghl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2cbziuhmf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yjrcxlyp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zqzmztyk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2adzfnjpg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2wrefhaoh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ipbufajo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wsnnkvdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsomsfve.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rxcdumod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvfbkryt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2uihtdvfs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fmzevgvg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dujnnric.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2prfaldtu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yhdixjsv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zcjgmrob.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2afdcbbjb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rlhnvuvt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2damflhxz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qrtpiwge.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2vsnvzjqk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmibfou.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ubnacjsh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2blifrqxc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ebwembpj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2laxpcqhp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2mlbtesuw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cvanxile.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nhhavrjt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nofpuvcs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oyffgsqh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvdzvxkx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ellpzvxq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2itecwylk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2idcklswg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cjdomrfd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aqildjxb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vsiviazq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2antikhbz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2omyndxts.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2elnvmvqj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oclxejxy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rgbohdvg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2einyqzun.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rmkkcvlv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2imvdzbfl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gdpkqqqp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mykzfocl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcoipsqb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2swqvpjfg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jmrpwikr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2galewkgx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kgpzebko.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2aktvycxt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dqxzdxhy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2svuezzis.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2llehyyue.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zykxggyj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pznlcyae.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kezelfcw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ngpvumxq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zefmxjog.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2snjeirqu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2bfvcmntc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ixkfzwux.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2mfyurdmj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zybuarli.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqkhxcyr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wiamyizl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzpbcwni.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rjuxmlnd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2aioaoywt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kwpvhgwt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2yjuopaxa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2sdazvenc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vvqdausu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sfhhlddn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2juedmvza.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ljoymfyf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sntxfywf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qcdcaxhu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mgxfymgv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ivitkpuk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2weevbqof.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvmfemno.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2patjmnhy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kznbdhdm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vaxxmjrx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kgnxjvlh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pcnhlvfb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmuyqplx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gscpusfv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2tzkkkupm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtzdmxjf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ilhcyjkw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ltvxxyii.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wosmoqdh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ifbeifxr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2mkqhpklo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wlggkdsv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ysoqrvpz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zidzeipa.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2sxzvttne.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2soumiley.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ihjihnwy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2soeezowh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uxbzhttg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ilazurja.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bfdkoabq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ronmacck.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nwzqrysm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zhhygplg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lluwbupn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vgmjevlg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uiydjthr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vqsvrovs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dgpmsggx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wnmnjeap.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2huxlwzjf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2udsriqmh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ellwquef.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umnyccow.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lmlboupa.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rdolybsd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bjcwcmgk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wlvlbbku.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2orhedfra.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xzwsdwsj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vomdczdy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2satenddu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cnnbxubm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ddbdfwjh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hiuehnle.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmfxbebq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2niurnmdm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyzmqgwj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gzvoxshz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fqhbnxnk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ekwpyliu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hfnyhjft.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cwaktmue.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qndpcoyt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ylbywdoc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2etrgdntr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eadzuhzq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2skxywynx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xnuvzcbp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yjxvuzvy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gobajyms.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pudqzdkc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fyzrbqle.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lsrlyvtv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gevjbrbi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pnlffjfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmgrafry.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2scfkdqxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvpnifpj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2czyehyox.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xlvriupo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhozvwgq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulukvtrx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zjhkmunt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2epqursjt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fcitqkxk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rgfxwhpn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vntgbgnq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2waekyjbm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lraamtth.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djwwykuk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ubitfftm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eldtzewf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ilwfbbez.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjdrucdz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fhxsfult.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2tydlwiui.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tzhgrgzr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jgodsplj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsymykuz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2spelotie.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qiixmnxa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxegzdfq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2tvvklfwu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2iutytyul.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2glbelgid.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2skvtskla.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ytjgmnyw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ztxxyiyj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nvxlpoku.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zfrmerve.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fvufddyo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zkjnqrod.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uitwjtzv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2epzqzdhm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2luwegdpy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rwrwbhoa.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mifdgcro.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cgafzwja.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yjcxsjyt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ljtqhtdc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rvtlumvd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tuazfrrc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tcvwepni.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qgdvswgc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2mfhonisz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pskpzzer.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bbxytgnw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jvvelwgu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uaxirktr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hzkvqeat.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hcxnqydu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bqfrfvhb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2gqnnavse.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2yztiamas.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bmrtaxmr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2jvpyoiwz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bjzqigha.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cyvuptie.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2yfrtwwhd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2iguosxec.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2genxqvob.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mpuirubc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2oxwaikoi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xvdqhzwb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2naukxowi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hooebroo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2eywggote.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nzoxhsom.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2nysxwdbr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynzslzxg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2eoxoivuc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dtpduvni.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzmvjrte.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mvooedmi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xysauvad.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rzdwaodj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zwdzkdxc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jackttzp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lytdmghf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2feeupetd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ojmynfut.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rfohsqnu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tarzdsgc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dpcgtvzo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vxnesmxh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tduubejw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2afhjvgzi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sfjevfun.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lbzlvxvt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jqtzkcqt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hmbenylh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xcyiusrp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2extlgxyr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2tocmresk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2grrentaf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wznesodm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2awgltisb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2baqjfqij.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2cuivyqka.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2bexnjuzh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2alfsrlfn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hldhkgih.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rtjzuspc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2hnqmrfch.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cpkhpqyt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ffkkigbt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2amtpgjrh.html


<!-- 参考信息 -->