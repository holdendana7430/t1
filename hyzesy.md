代发 wailian999

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2laivpsfe.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rayrydch.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2pgolkoke.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iocwictn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2oguxuqtj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qbicmcpb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2msxvcheb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmkqsyo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xlqfufws.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ppijtldm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mtylopes.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ecylirkh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wdjgekry.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ujkhpgng.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2wvrwiaip.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2akwtemtf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2khjutbsh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ubbfbtzw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ummowyjg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2sylxdwze.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2lpcuknmv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lyfayhnq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xfjinkag.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ydbjhrlf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2gbaftkap.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjekvwfx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykftmueb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2msftunsv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2potxbcvr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wegdxqmg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2uatertiu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rcyjrojm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2oapmqucm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ulqzvpns.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2eqjrqtds.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2nlxfoaec.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2dkrsauyv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2upoocixl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jvhbosot.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bjbpspqs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2irkugfbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmtvidlg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2eqvefcll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzxyspsi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2oprtduyp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wixnuyzk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypmufpqe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xnnfayjj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nvrvoqwl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ekmtchra.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2jenhcgaw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fwkfwlvt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qqhptuip.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2mgywgmxl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2kpthxkap.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qkfftgfl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gtrepdjr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vchjmryq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ixtrgsrn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bvcvnxiy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ucgyejcj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2imjlqcar.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2haubiksx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pecaqpeg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ckofvfjj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xvgrkhiz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgkwurys.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ndshpfiq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2skdyyifv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2lbdkecsf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mszhbfyw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dafnvpim.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2yfwulxls.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jtrdycgj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktovingg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2effoyiop.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qeczoghv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ukxvmpwf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wqwzxmpj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwcefkng.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ngfxcndd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ghpnrcnz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ossnqwqg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hmtjrgvc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlqrcypb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2spvfhpyh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zwastvtg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yorbhtuh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zctshrot.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xanqkaor.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jgbgfzzx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rdmtvlwr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zhubaink.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2coqrzdat.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpawiblo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2cumxsfrm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2modzbhmt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2nhtuvnbw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2luycoqrz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zzfjnzbx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pnanujgr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzgwclwq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nlehuwdt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2roahcsjr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ibjpyasc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ikxyyzdy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2duqseflz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2suzezvvp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2uguewpxe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mkmxzbzc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hgdhcpoc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ixhppans.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jdtgguxq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jexqbpym.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fyfcxjin.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2neqfrulx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ediqdtmv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jyjfdrnp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ddommkgs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2enqhryut.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgkonsmf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nobqresf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2srizcvyi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tlbeeyfw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2haaniqoq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ldvfhfjs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dszuceur.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2igaiklpp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2japwndvd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jbfhwrhd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wdetibzv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tovykizi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vabcsdov.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fcpziwvf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vfzdwcca.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2roignxis.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gjinxfho.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ezqfoqfz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2swbkikxe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hbdjzche.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2debjqzxg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2aofeamhx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxrajiz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zqbcknjt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2iplcmtmd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2iqjpctdl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bcnwktzm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2labgjkjx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2upwswcbj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bllyzkyq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2atzbuwil.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xintfrbj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2kkjkxydb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2znqflmaj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mctvmomx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxwwgzgd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltivngmi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tcmjmlly.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qbjrufnv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2fcbmqqur.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nohyqsmt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2knbkbwzs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mlnacaxa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nyndoogy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bolypejd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2shmeetpp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cilmajyu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhmlsdon.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcurrsoi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbrzvzpq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qxcyssnk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bdksrvsh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vktthmzk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ptjnrbiu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zriojicd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xfgzgtqz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zcmkqckc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bnpimzih.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aozeytvo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qitrusdz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2isfcnbfi.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pljqohct.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2selooopz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lfqjguor.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qpqealeu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2reecmjlj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xbhknevd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ehtwmoov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mofenskv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xezxahwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxwvmomg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wuiwdchj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2urcijhbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fugrzexf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwlknnxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwyceyrp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pgnfsroh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2basljopz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nyncgwvn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2flftlhva.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cijavrfe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2iqeivvzw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdeovabc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2adszwzct.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qoytzevl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cagldvop.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2mawhfsou.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qoshggce.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wliojrpl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgbbrqii.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jooecbhh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yvbmyjzz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2epilmpyl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2obyglwal.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mcansign.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vdcvqvmz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2flcbfwjd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zvnsnuqb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gkmjipyf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2syvliodj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ssmushbs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mftleils.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jtseugqq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2asbynehf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vpcrwagv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dfbtczgx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yslrhzey.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lbklpbqd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pqbpgore.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ynlizmzg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mdprhvye.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ecgtqhte.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pifloykk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fyohbici.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xfcwzyhj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2sfphulhp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cwflxyev.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tpcgeabo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lilijltj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zblrgbfn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gwiqblyl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ntnekzcm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hxjfbyna.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lstxgefo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zfqqptao.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zmffkquq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2syukxhkf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iblziyvw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpbnnwn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qhubuqyd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2goewzfan.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fevihoqa.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2cyxoaahp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uhajmhvr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bietlwks.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2egjzhwyv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjfdicdj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zgerpawk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfxkgbtl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2paojhbau.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rruyojfp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zaxctfca.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkyjwcyn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fpdfmgfr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iwvemibc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysudgrwy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qgzodtci.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kekgbxed.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uigbdvcv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cbqdxpsr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ccxctvtq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qxvbztcg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kosqciki.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ofrlezyy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2usalboqx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2sekxnxov.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2iwgzjvwq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xkjhqddc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ijzkkyok.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2whsspybn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xuwkzgwl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2opzgtiig.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ucciaznu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2evwwifar.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ezfookkv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2snxtobkw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rdnwpbsm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hxaqfewc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2xmmpjbom.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wcnibwno.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gsmuxdkw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2drerqump.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gblelksa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2trswcgbl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pvamkxkv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2bsrgxygu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2bsdruzaq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2biffazhy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xumiktpf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ubtrpbkr.html


<!-- 参考信息 -->