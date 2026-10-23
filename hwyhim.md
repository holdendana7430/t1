代发 wailian999

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pyrjkyhx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ppggqozj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3yflzpfuh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jrmejsaw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uoxcdzvv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3wskcyaer.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pftuexze.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wtfeyysy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3knsfleec.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3owlbpqpn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gdtaszso.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3auidygdd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zthdbxjn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3prieijph.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sxeobqfe.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3efhzxqaw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gnzmejei.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3yysrxrzj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3rshsynjx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3beqisjwg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3azqyavss.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ltroqwhl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wwozlztm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hrowtfvs.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofvuirhk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3wtqlztmm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3izoidszb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3luidcnhy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3dtcbumxo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfuvhmgm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvpmomjr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mjkmdwkc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cfxoyzir.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qqjiesai.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3crcatvqg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmjvbdal.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qwrfihdk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mijziqdj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3zamfimop.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xqesqsbk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xvziblva.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qedtxwny.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ekiuyjjo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lsztuntn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3oxjhfkiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikfsdtqr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ieikedfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqqomqig.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3dubaxerw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qyupjhca.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3qjlbiqrg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3syrprlkn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3shccjhrx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ypigdvua.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xdnobtvz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gydqjpui.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gvuvddzb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3nmtkqysf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ethqnnhs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3nixcvkty.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eanlfpuy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vgyhsmdq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nlsvwvja.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3rtawdrkn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xqpixzwu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vhrbjakm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3xqbfblqf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3nsxecvwr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3exrdekdi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kihksusk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kvalvrxp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3usbsxchs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uyeupkcf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3qfssadar.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qkitwhrc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wojrrdsy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jlivrisq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3begmrbne.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqkwmzpb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqnvlgfo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3snqwsctn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvaexfxc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3bqwrfcbk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ojbpnegt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dqqmuzlv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3nwkfgjqy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrtnazov.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ircohwpd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykirpfwp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pvxnyvgf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxvdngb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xbttzvyn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3olytegfa.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3asjpzpnt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zinwgaem.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zfnbabbi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mskkdcsx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cnxibfcc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wfxjezsc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3otfmkxwi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lgwmogzg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpamvzqr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3lckqraak.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yjchjkhf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xstozudf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzysxlzs.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjdqrobo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiqwjzgw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3zgkbjebp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vpgolmab.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3igmpnoyz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zfavpjki.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3abrttozf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pvvdwhil.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3veriaykm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mbtfokxb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ihxubhwx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nlxufarn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3yxzlorxa.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3trrqbphl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tvkqvznx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3qtfczkcn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaavkvhj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzdmyzbk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hncjfdpo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kwpzfqnd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nniadvkh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3kjfmnpad.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ffudeoom.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dtjwvcqu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fkqxdrko.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhjotrgz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tahexyaj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ajfqmlkv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uediarrt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3velpsatm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yjhqxzkd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ortxvtug.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vistnuuz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xcqtmjkh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eujjucjh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3siqviqbr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vjqazfyh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hytrqysw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kazwkzrl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3murzcifk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ajxmnzls.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zkxfpemu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3elsnvhbk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3sclhftxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uwliscsr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fbnojqgc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gmvacndc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3wipxvyca.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kdhhbyog.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3cwaspozl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jidgukqi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3iyyczgya.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ewehatoj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dxsudgka.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhxeauxy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3bpfnmhrm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hrcvhfvd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ahygxals.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3oubjsnvv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xqmgwsnw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3yyniomqn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xilgfyyw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgtqwroe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ynzhukug.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xlnntrqc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nentgvup.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3auhbxdvh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aszwstqb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jhxhehoi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3yxfmbbmr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hmyajpmh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dnkwfraw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dgisrgrp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hkdftwpn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tekodlmm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hmrxtcys.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dsrafevx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ndqtuapl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bpffvngs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpiuoynx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kxsrcxls.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kvucwujw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pwgbmiae.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ieyfnfbe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zssfiare.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yuwipuhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfycaycw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hvbenlcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwgjjyme.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rpmzkdkk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3khowffoo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtofarfb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwamnvql.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqamihgw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sdkeqsmr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3dhwrpqez.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yybzuwbp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwotttzs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3clixnqjf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xphfuspe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylrnvhym.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xsynvisz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fepgdjvt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mugmvmgi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pluxinkf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wxofffbd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3dowxxtnl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bmxwsmyu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3otbkmmqk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tnmsoqll.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jmhqfpmm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3crqvavbs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3oqpbnmkk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gadjqcjd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3rmybhnhm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lenmechj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ssfeisfb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hpeyjiiw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jgluwsbc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3awkrztbm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zntnwjtk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3nnjubfgi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltyxhpuq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yifxgnfh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sfyfvwss.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3zbrdxwzh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ttkoarcg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nesdmpft.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3givbewhl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qcgqkeuv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cpcqxfyv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ddahaood.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ahqcyjti.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3whhqqboi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fcfwqlpk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wkpxjotu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iockkibg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nxdzlnfo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eokltgyy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ztwdfukv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3efuwhemf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wjknvajs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ympiedmq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3cbewpbpz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhfphpi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3talfnvyw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqwdiak.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lflmncuf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3myxccsfv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pvsmelgb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3irjqchyd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vefpbqkh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jlujqcye.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nijmpvyi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajfvursp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhikdyx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3khwlatai.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3lxlgslow.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3uukyuixd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gwsmqrlx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fcaycads.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3siousgjz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nvlztmao.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nrwlzclc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nhxfobny.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hciholig.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbkpfkgq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3byjokbut.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3awvuqhhv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vvqttbuq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iuturufp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3pyaqkjyp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3zhgwqyst.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3hwoddiov.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jwathsvh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zxgoccns.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ugqixpcc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3qwwvunlz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zxpjnzyo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zuhahztm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dzcrneko.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3uvmpwzpd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ypnbslvx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ukmktrsm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qizdjpiw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3woicverl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3nxpppibl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vxuszqtv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pcorbedx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3uurgjoym.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3gxnrvqqg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hgitastd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vwxbvhus.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fippdyqr.html


<!-- 参考信息 -->