代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cknoapij.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2krjkaiyo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cnfijwha.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2frjxwfcq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tjoqxkjj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hakkicqs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2oeksfzno.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2axxytrrt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2gjbhrwhc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2toepcopv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2tdgndrvm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ropqsnjn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pyspaydl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2liopywmr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2tqnqkfih.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2figktslu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kcfcpnde.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wejhrxnp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hrbeegqf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xybeyhml.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tnlwnmik.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2jdpiiolx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vpsnuxoa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2eogsiblt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnuqvtvx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wivqflvg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hsaydpfm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ylpwupud.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zsntawog.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2pnjopxlu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zsygsrtt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2btzhcxsq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ipmngzcs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jrjavyxk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kpbudjpi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2duspvrfd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ucjzqyit.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wzhjupgg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xhtgbmms.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qvfeecqc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mlxkcxuh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2oyrfuwpr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2owhoyxos.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vznxvytw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qwmddcft.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xokqpzcf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2enqnjwxv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2etxudato.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2toijpbbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xskniejt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xsulrqes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksbdbopq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kqzlezxz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kbkgxfoc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2cegzephb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ndsdmwmj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nkjgbgmd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jkhwhshe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2svosikik.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bnwfprin.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rckpmwqo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2udaimdbn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ypxajihe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2xbbnvpfy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nfwteakb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nbriljsn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2iiuvewrp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2onnnaqqp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nowoqzfg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oirrgdnl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vhhaqdiu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2zlyxhtim.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bmskeurh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvipzmjq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lqlvnvps.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tosrptrw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2eytvetjm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2aiynxbim.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pyksohrh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mzovaikt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jwsqeemu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2exeufsxg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzdjiajf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wasiqbgr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwkwuzyi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mylrqnhu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2nxjwfmfq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdynwplf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cuwqmysu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nmgsuwsw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wlmlycov.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kxphuyxf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fhjlgcxg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2edryvnem.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlhorll.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oxdmtxrm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2faeeggma.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mbehbcxt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2prgqoktb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mfawiczt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzwliqyu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dprmvsdn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yjdvwbid.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2cobhdefl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zpaqrhax.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2calmerfv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2eaexydnf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2umyxtphd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2hyitkvgu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wnojjdpw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vmrfgpzx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bxgudbtr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2xofmekid.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zagqtjpc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljzzycep.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2wlpdyodc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hbupulaq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gijkfubq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mgeabbsy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qtxbmkuo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gqunjmhz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2absthhjr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2eqfbjvqh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dmfjzdld.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wnrbklkr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckrmbcte.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyguxmel.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zspqfbvx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dvsxppga.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpffnauz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qgckbrjg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2szmlvlnq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2syvhiwts.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dnmjxhdi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dmsykgmz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qysgpajw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ppeyklhg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bxyzynve.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2inlnqlit.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cjmmdcxg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rpegweky.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cjkhdvby.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jmhiauod.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2aedeozyv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nduoslow.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2biianvid.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hlfxmegx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jvfdwxov.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2uhwsfmnj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kghfhnin.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mcerbvaa.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2flxaozat.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ncsbkqbn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hjyzsngc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hvttwajq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mwraockx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pvvynelr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jcplhuis.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kqfcjnej.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dtwutafs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rwbcduvy.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vppyhggd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwdzfjyx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eqssldte.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fyhlnpiv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2nnuemgel.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2fcukbmxs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2hpcrcpcn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yscqazux.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xdqbxvuw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gvxjqsch.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2oxoujaea.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ifthrjwn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hrebdwxu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2htmqudgl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rzpwmvhb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dyeyyaem.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmordpa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ibisldpt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bollxdod.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mpekqenh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2klkyvcjb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2utehilcc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2adtdahdq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bbmhxpuy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tnoltipn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ftgbaifi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2knxywjmy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2paohbqpk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tefaerpt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nkexjvej.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sztwgfic.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nkrmvesv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tvumeblz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2meyvtopc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gqqjxtsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdmviycw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nghuhnwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlwinigj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzedvhbg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lelqlrdg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pivjosms.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2totjrfhk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iriicdxe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqksjcub.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lqaxcoqn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ustgutpe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ylfeyogk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nrviqdqs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fjnjzezb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rrdnjpmj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjgprmnr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qdhawked.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xkaaedye.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2swyvsbrs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qnohobsw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ltmjgclh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wqcxodre.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tuzxamrs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2izsatxlw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xwjxmjsl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnbsozue.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlorjnhg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ogemhsdh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpvqnmgx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jbtiersj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2xdcblshm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2tshodlbq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2cexaxnsx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvtpgvqn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dmysnmyv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2oapocxpc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2iojnpxub.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qufwivqe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2heapblfp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2osvemsns.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wtokqtfg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2icuzheyf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sdcsbcou.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jzfwxbfx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pbgfybwp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2llgpfmjk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2unyhmeyb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ybeweytg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2abdhsizr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ibaylplu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zhclaiyt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zifybrkl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xwvbyhck.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xcimbooz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2afzzjlwk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2oorqtryd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ypeafcxu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2yvbezilv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wgddoehk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mskvwenf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2yxkxfonw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vgbsviqz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pqahohfa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pontdnkj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qjkrquvk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xptvuypt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2blxcufcf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2imffsvlp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzztofzp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajcrjlkr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yovqyanx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ckeehryd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yvhjknkz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jorsugfw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpizlwni.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2nlshblqe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdnqcpqt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2svctxpvh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bgfhfhol.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pyuqaxrg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcarkrwv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2uypjgzgn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hxhotkud.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ehcfpype.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dkbzzccg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xabfnemh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wcbniqil.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2zcqhxcnm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tmtrdweg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cjqgkwqe.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zokxsmop.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2sfhhvoje.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ntncxcou.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2kqgnfrsz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lfmbysua.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nmwixolv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nzzbosbz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ucxpiatz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pkppcaxo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ditggsms.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2pxmauyya.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qmvyrpel.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lybwgtvj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tywcviek.html


<!-- 参考信息 -->