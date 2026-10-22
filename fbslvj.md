代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qrkfbxtx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2eieyroix.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dheutjab.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2gicbfysb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzugapn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lrietakq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sixfypcq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eozgmmrx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xvzcmpvk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2iortvjtc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vwiueovw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2oahdnqwy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mdtoompr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bzvbakpi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2lmlyuoah.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrgemoo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mdrfbbzp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2dnpiemlc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2mugrmlge.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ugiopbzt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2szjewndg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zqgquoha.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2nkhuqwac.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2swbnidly.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nxxwghpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qndnajtk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2csvqeywk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srhbnoui.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wnfxlykb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tawvznwg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoiantjk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bnrrltim.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fkgxnpox.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ifugglhq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zhqwjjoj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pnzsbklf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vmkiovxq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2yqfmvvvh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dgifzenj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ghppehdu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zmqgcjeg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nmirshlc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zvhjpbnn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wsuewtmn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dvxomaoc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wfeanrbz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fmvtrzaz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tvshlwzs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oidxjxbf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rulbylgm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twcnuiei.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbwognpq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ibcusyrt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ppntrabq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zedeclwc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gtsylhil.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qwzjmpdj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2uazhamad.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2egycxauq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqywteqe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qkpumgcj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xbxznlbv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pbqpnuec.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kyfwcohr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2novqseqr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kjshgsvk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2sdfutllu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2myevxaen.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qesujrln.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kyebxhzk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ghajxtdo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gwusyyza.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hnmhqhtc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2glqxsybb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtseslt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2shvmnhbw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ttxnowhk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjcobrpr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzcbdyre.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rbmdlnvj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kjdhxqal.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2umvwcmzh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vlrnureh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dcapgbdi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltuxpnbw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2udkpasrf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hlsjbebg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfythapu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2xmlshcsg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fquopzfz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhatpcmu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ccbjiyre.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2opewthbb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2elnsaixk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qpyptwcq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qzeskeaz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hrlxavtd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jfjqswjs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2odadlulo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2plrnyulb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pixcahjq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kcvhpmuu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkvohcql.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wdewklhw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciziwgup.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mimzctvj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2upigsibi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2nvplmekz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2prtucrfi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mgeusial.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2edqukzqe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pdwwfplg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zqucnodr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2udxclkmw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2orcllemr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dzxltejf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jdbifcrk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hrtmzizz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2pazqtpsr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2whwcjvxf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2czedbxxf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ocyvlqea.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fbjghfft.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bptyhorf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2adsdwlcx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vlukrjad.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lxzgjaqo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2rtakqecv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fzlcmfmf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lrdnuxqy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xtqudhto.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cmsjpnnf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xayqvdab.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ipjumbmq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2aqpjupgr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lsaynias.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ukevpgmp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vmnyeprq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2cxdvqrea.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eiuplljk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cnyzmtwz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cnnnejsl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mxlzruuz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2avlqxzyz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2dlhxofai.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2raozilej.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rtwdvcbn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2aqixtxrj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eeikauxg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2owkfxydh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ofbjklki.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2czqyvejm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qlutyanz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kfrkutdd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rhtggxnu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kewjdbjn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2suemuxbt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fglvojao.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xfbbklmg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cycxgklc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nvyxwloa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sfdxtlwz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aokowobz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ninlrqla.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qcmxddlt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2adkpavkt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ioqkbsvt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2edayvyax.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lrlqijvt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cpsxshxe.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jtxijshz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vshoxoag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssburndn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yjlatxso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buwvhugk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pkkfldlm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cettlmka.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ikurnfwa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zjmkylnf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hglpjzsb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2toaducvd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2olttnwsu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2coptinhu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nnxqsurr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2cwktgidw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dtrnnvzm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmiizqxy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aiyxgxfa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cohkbiul.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2arncmvoj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljrqwamq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hzpixjvf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2akqsxfdy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ciskezon.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2mjshweau.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kkjlqorp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjsuwczd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yvenslmt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmhjzcgf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hrpeqpee.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2pxdkibjg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2chbykedm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mkemcedv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hwdohcpb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ueruzqdi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jswvuqud.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nvtciapj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kivciohk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uzephlft.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lstlljlu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qyhbuovp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2adwxsudw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uecdqdag.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tfffqtxc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2suagjrsc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2grpmsyam.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ogqbucqn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ftqgwrhf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kumlesbx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xyiuushk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rgkwwszr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2nrumtjvj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hsqqdbyz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ntsdsgww.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pzvlbzij.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nmmgbcmh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ooaewdbf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yrvwjupn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hrgjixcc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rmcglnvo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bnhngazc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ydkfzluh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wmxigedo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzxcbde.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tagdheol.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bianejuy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vcrinyzp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vdavasfn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qlxdtyot.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xhibcfgj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2csycvvbp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtrtanss.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vivbaigk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ckubxdbo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2smqezgml.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2odynjqyh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ycikbehr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2oxawrbar.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wzbaxsfa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kyaqibta.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gnkzntzg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pglrfcmz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zjogsuig.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2qsncuper.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxomiuka.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xxfudbmk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jhfbexik.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nkqrcsji.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wrnivqkd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2njocjjad.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2iwbqtyeb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yqlqmqwt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bhgcmaor.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wgkzobwk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tadkldsh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xqawypha.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2iojiwhsg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jzxyijhi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2btbljaeo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vfqsepaj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ecckmvha.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jaubvzsv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2sdcbwtro.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ngwvdxao.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hissxapu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2pxqokpro.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2aftgppbv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wgonjpsx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uxevimbr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2iiczpfmw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qanngzhg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2twtfuyrw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kralsxxq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gxujpfgz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dmoubzyh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2powtrntj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xvwivngm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjqowbnm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2afozsocc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2lrfdpcvr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2duesynyh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2wfowrmpy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsijxfyl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rystaxnh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vbjeajue.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2svwvecds.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2oodttnna.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2goqcbazb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ktlrlkmp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lgjiyvqw.html


<!-- 参考信息 -->