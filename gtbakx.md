代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2tantzcpf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jkwkpoms.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmnszrwa.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwajpaft.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ednkkjev.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rzajxxta.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dytcymcz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2susxstjf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sbtbzmzk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxcnbuga.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qvlksuyn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rpkysmnd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hiehhett.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wvepzeee.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2dlnyimdp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wtltduku.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rsdmyqmu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ymsyqwjz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zwuvkdpn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2bsgdnhji.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zewdsnul.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tejnamau.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2izxlcorg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xptjrpjw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fxxsfbci.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xlqwxoor.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2mxlaawtn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2mogmpjue.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2sipmlxzc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kqlbicua.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rgkwsdqv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2rmqullha.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2maylfrkm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2vgkrnwmi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gtaocmjo.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ewcxtuqi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2asyntrqa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpoyudyg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ztrwyxvd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbrxhqfg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rutzzneo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2omwgdrkv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2gfqgbocr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2shyruvpu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wzflkvba.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ahojoeny.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqpzead.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2eozsfydj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2sflvaufy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbfnerm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2uvmkhouf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ioiejiag.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vpevulad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqxlfwax.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kqnsjivv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djewaghk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ryuegnin.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qkhmixed.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2yeqtjcfc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pszqjbxp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kkzirdon.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qvwbqowq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2pgbgcqjx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wpflcrlt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ogbsoaji.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2nnrwggfj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2bwotavxj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grqohtsl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cvhntzge.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lrvgiwxz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wmjdwnyi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zzaihaxb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2bsmxgybw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wiwcckug.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2epswntyr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gsyzlbro.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrukdixh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tsbgzcqe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgfxyebp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieipxevy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xtwmemkv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qvsanpfj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gkqqfpgh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jugsrkco.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2dunikbof.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bfpgbpox.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciezejoq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrrfxcow.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gnkoekyx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2doddrcet.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mcfuugoo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2isgocyki.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2alcfvwtp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qfxoaget.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqhoxgzj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqqjxgvd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wdlpkamd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2updlvalo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fgvahvqt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2snhzfelz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ubbaahyf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kwodsixs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2rbmclmzv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbnspktw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gvwtddji.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jozbxelo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ykwungoc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ghgsidvo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kdzzujhb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctoxizvh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gntswkvw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnnaguka.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddkwxqfj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rhwkpnfe.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2naqzrzck.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2volzfiwu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hfueoobz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ejkeimfz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tahudwwd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hkmbcmhy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2jserofjx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uiuoppho.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vkmmiqnj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tqdqzllm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ptpwftxj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nyqazgbs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vzfjadgr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tuoiflmk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xvpfihnj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2exdvchgn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyiyppgg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2axajptvk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iyfdcfzb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nrzbilvz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2yltgjfuy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2beqwbchw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hllysscx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dwnpvkya.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jkuuogwm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2efyfmufz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zjkmatxc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2sfeioinq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2iorcdgge.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cltfkuuz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wkatyasr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2twmvfcjt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yguaaxll.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qbpmsnmp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xllpeisi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2flyxrtes.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hjuqfnqu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ydhdjwsl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2chydomqr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ccbbhllq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sfftkegw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2aodvyrkq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vzepadkr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2olcwtokf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tlfycunr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2euxtdcoh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uzhuokwa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jaxixmnw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jiekklzs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zqxnjcmr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2daxuuqwj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2kuwmjvws.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2noizpcof.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqkzexhx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tldtbzdu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mfiectym.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gidyghfj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2hezlinuu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2llrybmbk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2cajktvgy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2txpjvlqf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jwkvhmbw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bosbvezf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hqbbnjda.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nyapjrja.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2anjxqrpb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2auyvwlad.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2svzdljer.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hwdkdlqt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zsfitdtt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2cqwpdgta.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wypjoyeh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2esxziqyk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kubtxvlm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aantdeer.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nzaqulcw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ycrpcuvf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2codxvlyl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rqrjcokt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzgoxock.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yrnwzfqr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ngxqloxa.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zreusjem.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ngoaowba.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mwcswyep.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2urxgcloi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpfcoijn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ivwkddaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkhobtmm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlpokrvz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mixrsaya.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktcalsyi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyehrxqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyugdtcw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aeteocha.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wiiverps.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dyiyfdxw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yrernizl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lseayyaw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zwbegvzl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwnhlghx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tizjxbih.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdzhjgyt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2yfxlojvw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvxfiyhj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2worsdvki.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jglclqgx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xesjqdlj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2csfklnvm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2shikoate.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lxoofdsz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnwbwnvi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmnuicjh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ncmtnzgx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yvippxlt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vzzergqn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2skywnyvb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ohotinoh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2asarztoi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2sygyxlqy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2oqakmeuk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lnkrincb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2xzcckxqz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jysfqvvy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tolkosaa.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2aakfiayy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lxzadece.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xuyvxrwy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wyuvdsau.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yoxvsthz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2awpxjske.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zulozvbi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wywdzllg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2wxgvgqja.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vnwdyuwv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2psicjitf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kjcbfkxz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ryfdlkzh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bqaawqoq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wcrunhtv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2djawjylv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pytpyuxl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vzzedbwx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2paxrmmab.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yrrruhzf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvblwzjr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2loghuqie.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2iqvsbugn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2obuttaja.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2nwqvwrog.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mordcnym.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2eqbncper.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ahyuirba.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2usbktlvh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yneoulrt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fcmljcxn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhvmyera.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2eeyhgwfh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwjhdgwi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2bwsskhvd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xtfhgqrj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2igegqpuo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rewrhowu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zqkzlazl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hjtumppb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2laafaytl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gmkegrsz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ckavtwua.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2akfsigus.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pnxgwuvs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2llolkpej.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xvefmjik.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wovbbihd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qoaoavdb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zjwoixqz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gudlhszl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2capcicmd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pftxzxnq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ytrmqynj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ufpfjhrl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qmaafzss.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fjrmrvgq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lwdsqysx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tpvpadab.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zwswcugt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2cuoexjtr.html


<!-- 参考信息 -->