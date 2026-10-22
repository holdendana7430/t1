代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wclsmams.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2crbmujno.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2swnxuocd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oxlclzzk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wzpqcryz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zuacdzcd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yobwlvyx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2nsawquon.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2trjvkjiv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytjyxteq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ewfylmep.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2rgyeupou.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rxlxdmcf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xduruxuz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyuweeuu.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2uuyjsiuk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ppeowmmw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tleormvg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2njsevkll.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cghxxfpf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dihlubrl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2chxvvibb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tspoveqj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xgakdehb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2awxzimzk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2fshrvkpj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ocmmrsdw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2xxphlchu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2dzyhtcpz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kjftomcx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2svkalcqi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2pgqaswvl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2omqwkcmg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vyeycuvw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nqzlymrz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cjgztplo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2zjbgxbey.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdyyoyh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxbalujm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lyovjlvc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2tfngvpsx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrvmwtxy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dytuljdb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pufxgbyw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tumuwidt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2gmbreukk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tnqviqpr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2iqcazhlp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2vppunxvj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rebdmbbf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2fznzmhut.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gtwuwlfj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rlqbvbzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czgqksur.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vcanwqxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytyamukk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2uejayoih.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2raihlflr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwxcnuwx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lprzmhcb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dlkoguen.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2coenppyd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tlrbtomf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2kxdzzrik.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ctmuhkbn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2sqvaslbp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2axteektz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdcmwssb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qseuqnwk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2syotcyjq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2svazdkgf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2fwbrqrbv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2zeyxtdau.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aznwkshb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ildnliau.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xybkulzs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oballnom.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lvyriigf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fbbyppzc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvpvrjqj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cvonxcxz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mktwttne.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gdzoqxyx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ktwzxvqq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ahrkspyj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2alsxvnzz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jrqphfut.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zpzplhzc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljcmibjr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2acddvekv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cxuxhfts.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mggvphvi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qpxasgtq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2eaztucdr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2msdpojmz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xsvxaqng.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rbubxwew.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tntbdlnk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lkyvbtgq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2znlfepmi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2unjwdcva.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2piffxpsi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqqrqdg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixdiphpq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qifmgrjl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2krauokoj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gomzmhkk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2grrpyujl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bymcznsi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2atuejehh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ybaynuin.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2pjsjhwqj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfnbkahd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2utjeucor.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2htsryebz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqcggkpt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zbnnpxiz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bweioamu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nsxedtcl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2tvhjhuzx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ozzwhtgs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cilkvoqt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fqgsgcri.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zvdqubpk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iwbjsnwm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ybntudoc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jiffvorf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vocqjadb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2njcjsghn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyflxcba.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jbqsnodl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuyvilyb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2owqlnfgi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ikwcgqcx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lhftblkl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2pgmevnrg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yisiscza.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2uvqclawa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmhcajz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfwitmgm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cprjvcue.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2itmkjitd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pzvkhvha.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fwtovptb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zbceqefh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mimktffi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2amybqiyb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lkyllsut.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qbckdeac.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ropdithu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fjzaqgfi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cxoysbtw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cndoltkn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2aqvnmfgg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xtvnzung.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cijpzzzg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hdvgzdxp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gjdpkqhn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rsrrwgum.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ciersgkj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qypuvqsi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2sdyecysw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vfyjcnwt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2iqrduuzm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2woulzqfa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tszlknqi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gyyxzmpd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2klltwsfy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eeyfkaix.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wnyvfqlo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lizcksvh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qtnugqjx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2akkcszya.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2eogbktfm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xhyoylcb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2efwoocbf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ukxvgclt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsextwym.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2blfjxavc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ryvwnvux.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nhfkjejy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gwwrkiex.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wmecmwfi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xlasecdk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2oxxhcpnw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ktpsfswc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2enfiuogi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2afxhlsfq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tvskpvyy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bhatsonu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2knbjhykk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mcpeuqyo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2huyocdkx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgihyuas.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ltbijjbi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kywwdjtj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fjxsdqdd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2btwbgcoh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ohbqxgmh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mwqkhmxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amnvviff.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kgxsnbue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmdhafhk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xaycxkyi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yubnzhsv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkcdmolb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjjjbbbk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiobczya.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wuynsogk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmsmndg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2oyczmxfb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dznwkksb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2decycngu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ssnnerwx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ucwzqpmi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfkizsxd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgedbrpe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ucaoifrq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2onuzbwup.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ybqreggc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mibfwqql.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2bmynqhib.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rcjcuxog.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2adwjnmet.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pozjiepo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nnixmhmw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xrhhtmrn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kzyaknyh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2einawjdz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zrrieuas.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2npbzcelj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2piqayfvq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vbrjlach.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2epmrzlqb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hyfirtri.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ctgzwstj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vaipyqlm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qoxforne.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqilnxql.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2rfddlzda.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2aylmsycz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nspzakgp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zvfbzjhm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2aadvawyg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zavwusff.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dxifpgth.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rptcbugj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jyowucis.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cjoviwxy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2lfyfpofu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yrqxytbj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kwqtvrgk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zehvtgsk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ecviulhw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jqmcommp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2diekwqsv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2czsvmund.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2gnoeqdzy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2sbzxhzdg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2soykkvtg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wvnkasjy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rrwxlkep.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ombbomic.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ochplvvw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pmvdpkpm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2fwnkcyqt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xecdcqse.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2nfxrlvyq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqpzgszh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzddupvj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnclcqxy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gpfsqyro.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2smkjwndz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xotttcdr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zcnkzlyb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2chpjoieo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uotnpxeb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2npqxmyeq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zglkwyqx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nyiunwlq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dpyimedo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cvpvbkoq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eychtozd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ndqdxlpy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uhjccjnd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ffjyedkf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gcjxsqpq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2smdufptp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kqngjkti.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cjuhuaic.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2avtogeuy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fvobiegu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2awlcrxvb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ejowoagy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ydnbxvyp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wwteigmn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uylygobt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lwenixca.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jfaqxlqx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lqjsozcb.html


<!-- 参考信息 -->