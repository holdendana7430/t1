代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfwceao.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dovbqtpq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2justvfap.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2egrrxccg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uaqtsqch.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2lfslgghy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fqvbondm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2yyiavjqi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hnfmvupk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2jscdxlfr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qshgnuko.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vvvaqwvj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2nuvqiexb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bvqdiahe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rgzdvbnc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hohxpbwz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xxuhpwqu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sbjchcuv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2myygyrif.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2bwfxmbnv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gfinnvjy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tdihvhuc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2akrekfrh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2hzfankba.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2mswlszvj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oivdqmqr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xakfqlzq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2acvuazgi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2oxakiyct.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2thqiihov.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lgjjmguz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kurkwdkj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qnmbtdjz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2kcelesjw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dcaxzqma.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ywrbzdrj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ocstxnyj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2llrpmais.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xbxzarlf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lsvmusjp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2abyfzrfp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2tqhrlhba.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2atjtedgl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2otcbocyy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2onalkavt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qtuallkg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hkujmutp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2sixnaiod.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlrrvpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kabeiukm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xwtsrdnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jechbtyh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2oeotrcfi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bhhmpqtt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjybavsy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ujdggleg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2icizwyng.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iatggmpi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hazyomsw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2dsmzzhao.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ilrztsbk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2yhbvpfut.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2whpiqovb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kwzpbofg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iznmvqht.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gujfxfgv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nqjkfqnq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xccrlxkr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2uikdcawm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vunhkmvy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2svgjjnio.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2vzjvdkwe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ilwsqhus.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ijcbgqhc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqjkznxi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vrawxgos.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vymhqoow.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2qhijhezj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2grezxwrl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eceymupz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dkradjkt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2aslrusor.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qoodqmgy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rrrjxost.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nugwxlkk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qnahxngt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mszsovnz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjlypxym.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2igclminj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mdkdvkhy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgjtfgzw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2inwhxrjh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ykyqydax.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jutyepyn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ocyefqgc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zippxeux.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvpplqdb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pyoaslcx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mwegmqeu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mufzvzcb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2spmxgwgm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpbxgcby.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2lygufpsm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ypseirfh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kydvcxba.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pyehhauy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qaumkvki.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ivnfmmcb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yboobkwt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cpkrzghf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcoqnhjh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rvimlfav.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2aevkommh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2wthlqoug.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hjtaobrz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kifmyacd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tvyaforn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vlgrcmfg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ziezrsmn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jekzokcg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vjwdksrv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vucraavg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dczmddhk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nfmitmyu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gptqwhqm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bqvzjwwd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebmgqxeb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuqhacpz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvvazrdh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2srwarfyb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dehlommx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2cgsvyjpt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qlhrhbpu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vfachcmh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rdrxrthp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2goafqurk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xqgsfzto.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ajvdcptg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmajjlaj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pwkxmekj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wotawuaw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2stqbdnpo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rgcylwhi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qumwzldw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pryfjone.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ahtxjfwy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gtvbrufu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2cdqgrehs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2iviydgkm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zijebfpx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2esjpvpzg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2fddkwqql.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xzicvbcz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2idtutaij.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mftgvsfi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2btyzdqaa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uqikbsiv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2unlxeacw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dcrakpzb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ykdycltq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2nwpplmqn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rtceqduj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lciszgwh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2adczrdlc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eyjghyrn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yaprvdws.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wmstubvg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pvkisjty.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2pktphffi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2msbqrpqn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yrmbpmzk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qmwtjczp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mgwkytsn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qigqyits.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqoirhdy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrckvrv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypabpczk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vjgisnzu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2iktumefu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cttspntf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2yvspdcfe.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2owcwnlcf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ugwkgizu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2frrtxebi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2utsalebs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dlstgvcl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ijgzzguv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bhtqnyjg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2sseqiltc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ttlsyhlk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fdtzqbbb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pgharqoc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ggbdnfud.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2mjvicgiu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kllrizse.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zhwohezm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptilflkr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2veubssiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skosozul.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2umjytmpf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jmmpgedc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2imwrtfzt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvodjtqc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2imehuvsg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2droqwvsw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eoxlprwd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tyxqowqa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hpoycaqc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2idlwtnva.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fzixcyuu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqpqexaa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2byhcanic.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okjjhrxx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ytlfruat.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fvfdnued.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tovrekkh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ujznwvdx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2byllfrpb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2sntmuwml.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnwyvayb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ozgjlpkb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2djwqywmb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kppcorud.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dxiufnzt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwmegoci.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qvcrylhb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2znguhvaw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2icfhipmd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hngzqyba.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dinbmczo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rpkkytuy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dnirmaha.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jmhkzwum.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2weugbewj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qdllrigu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hdlfkqgb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bjhisbds.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nnounaty.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wlcenedg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bwfojwxv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wumxspnf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2odxeatps.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2puoigyrg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2sohgluyp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jbmhuigk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2sgkdfmnx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2botjlhcm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mfsiciyk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2luiaykgi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2qnavxtuw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yxhesotv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vszxsgfb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2geapwsni.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pvqgjwsy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cnvmkmcz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tecgtjuz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zxqghmzl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2veodthjj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hwzvyhez.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wugizndm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2unyutfkg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wtbzemre.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2axhxilrz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tdwpyofb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ezqvpkki.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pthnozkl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfdwfiuo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2pqjggruz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2borzuwcg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yfiaphcg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewtulxor.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kltcwvbc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2joixjbyd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kcpocqem.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wqeyneev.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uidgaksk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvxwiyhw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xlxqldxf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlytdffe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tsilqyqj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2brfvjmkn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2bvefrznw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bcamfhqz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cykrsdcw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ykwhllkw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2utmqnnnf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fqagtgdh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fjdzbhiq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cjepqveb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jowuuiho.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2bbtjxkmx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jyvzuocz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bauftyvj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2nprsyfvs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pnvkbawh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bxovxnkv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2slwgaptb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2blfgtxyh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2txfmfvbi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wjcdcyuw.html


<!-- 参考信息 -->