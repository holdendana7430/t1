代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ahzrigwy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fnlbrbxs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3teymryvc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3vjlmdddg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3unkdudzm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3nontcprt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dbpzrfvk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3pdykldbp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jigubqzf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3sslaptdm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3naamrouf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ywrviglm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3devdakrf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gzzeihtn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3moiveiuy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ngedqeoh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cuocusgu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jjhmdmwn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hwowkwqy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gsuvyzmm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rznwfxpi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3hxkxuvaj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tybitruy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3uwwnwbzo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxpwobap.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vwvnvwbv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3btfuouwb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3prhulhuk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3iufiukxq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3fqnmtzwo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ynfrhuin.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pikejqco.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3llisukup.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zfdgxnrb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvdhkiwh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mnxmmjax.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcyswmrh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydswdama.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3appjykjz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ibbihbnj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xfovfilr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3gdvbphzb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bjrjsxmx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3kunkrtzg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3tjioghtx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yrgwksje.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3smekvlev.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3coawfdnu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3glnnsfja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqbxurdv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bwrghjgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfrjallx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gvenehng.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tznkdgzu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fydvkmch.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qdxtawko.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3umwlvnju.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ixhhutbh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xsiepubu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3blnvhpts.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uavectvw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yvtkrwud.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3rbhgjfhd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3qyznpddc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kxwmszfv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3csmlolhg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hkuksgzc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tcguvskd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3owxluhqr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rpnpexyr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3bksewamv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fczmpnvb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzhqeenj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjpucihr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffjwlliy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivajmars.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bsglvabx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3hnkxsdke.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qxzlxlwm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lqsnynku.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hxooigvt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3azepsgvd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3njniqobn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pkkflugh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3mxcsqosy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3gnqlirvb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qyphxkbf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwdvtftn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wivsktat.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3bzlbxwqj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3slckkjsv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3htnbnhfl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mouzxkgp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fzxrgxjt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yylaoiaj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lyboacdh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmdbwrjr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sznaxkls.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3clmkdokb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jtrjxbvl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qcfiadsq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fjtfyeqh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ioakitbg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lgfviafb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wfbetrai.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3chazgzvi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jhdtbwyz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3lhniryvd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3bgssuzqo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gtqabdnb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3onxmfyvl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xutaazho.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kxwwzftl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikoziitp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3drlqcszt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3rcxbnsra.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zvchylix.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jhekukme.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vjlcuwoe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yjqsaqau.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3crkmonri.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uncvgvzm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qvonugki.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oihqilrp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xlxbbeco.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3stsridlb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pwgkgsqu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqcvknpy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezqodzhr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nbsengio.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bobmoept.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3firkydoi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovkuwtvo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zdlntrnx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cutdolso.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wmtxbhlg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3enygsctp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kusvqzgk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lospsraz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ruvuzulj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lvnhasru.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3excnmcrd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pwmpbqyu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pnpewexj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tnlmfpma.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ldvlrrwo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xsszvqas.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fkdgqdaw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rvezjrhj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3cukqkzrm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uzksfcnt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zvjmvwli.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ufzjmfhk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3twiqumrq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ixkszgdp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yzkpnmyd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnurpeub.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3osyiclxw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3smfxqbny.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3drrxfpqu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3fwzirlgx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ybkyrlku.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfopmptn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ofxpipdc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cpclobag.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3nvtwbejw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3adueathn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3htjuylpz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gphmdwmc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3mthbvbnf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mggkczwp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3yexhnkyw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rltqnxte.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3trkamyqn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aerfcxfl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3woyipyhd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ezehbtys.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3llbkwmzj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lvrsvfvu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jvlclvyl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vpncyiyp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xmuuxsnn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ismnjdew.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mjudxezt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xtmsnelt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3avvdkuwn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3abuchnvz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3lybibbms.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3unhhwxdv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmaaxowx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mnlzzqik.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kvdigkvq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ckwbhkzc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3pbpnhqeu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kjkdvxvh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3akygexfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khymmkzg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eysklucx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcfzjyuv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ltcgknqj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kdqaeuzw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnkbfqet.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylofdzed.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hpjfecta.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuvsqece.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qesjquwh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jqlzzmui.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3butgofwh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3noprspau.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lvcedsjr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thgmyycg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rlgxtxut.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sgbroqrk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3owxdkjoy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3yhscpcpo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mbxsmzsi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3lbplkllq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nkowgman.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3smczpsgp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyteranx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gnizwzcj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hhtolgfz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttdoddzo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3cicdvejc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xioafpjo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bkrqqwav.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wawiyknp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3orqcqwmj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wujazmsk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gaaqgguu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ivuhycnh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ojgkjwfv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rronojkg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxxxhoqg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yhfslsuq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vshdkciz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uvfdmoqx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ywhgqjiy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3znvioxyi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kevfgrsh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lpqmuuqk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xjicosgw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dkrvioyd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wrksilqs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mwzuowsj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kagkkrcu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rjvbpbwp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tjxgtcjo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dnkgkjuv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xjizvbfu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ltolxehy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3koejroju.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yezjjqsv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lxzelrpz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pkiiucew.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fiyklxml.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxomtlj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xhlhweqa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3earosxbx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jahobgxk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vbmfzlqj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3daxwjryf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xuihpymx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gmaukymz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xygphxxl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lyglruva.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rydauxei.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3tdirlnhi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xrpdfrwt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3npcubctd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3spapfvrl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qsezchek.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fxonbymm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cgesdinf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3brvpnuvp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rxvhebfy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3swioutia.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qzvtvqct.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qubvxgwt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tgfsnrye.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rvrdokke.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zsdjczpq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hgtzzfyw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lkugbkvv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3shnfptse.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mnarcyez.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ulbmtfem.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vxaqicqv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pesqybbc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ogcqentm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zfhlogyb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mlguppss.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zreuxunv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lcfwtctq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gespqzju.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wdqkyzvx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3iomreldy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pyzkxktm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gjkpqdck.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bkvowfmp.html


<!-- 参考信息 -->