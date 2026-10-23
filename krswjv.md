代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3shfatyji.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3swsuqyln.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3eejqchqm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3tiusvvhm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3bznsfbas.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dhtcqseq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wlbywnsh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3njxyrvip.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qqduqcjv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xqbtzxpc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ullvwtmz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3zzwshijx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rkibkjtl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxihqbro.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3updnfurj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ydgklcic.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3mjmpgkht.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3aljorgdg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgptafml.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dletshml.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yqpcdnuy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fqsbycai.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3vtewqsbf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3wrzgtptw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ussxlvee.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dqzmfolf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sdrwsadq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3wpnrxzdu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xcqoikwf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wwfzeoji.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pjruxwsb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3rghduyev.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3eyonogoh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pbvuelum.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lboiiuzg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fxnviruw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nremlnar.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jofsnuhc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nulzwmrf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xjvlfovf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zttgxiug.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxanqxja.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lmxkdphv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zpaxvbur.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zamhitkx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kccovrgj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fmxzouht.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rdpnznda.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bhiykppr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dbulplve.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3srqbmvsr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ubgojsta.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3bqpnawwk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ziqnhblx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jbnxuucd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3bxfggipb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cmosthny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zeymrcgk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lmlexauw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzcqajro.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mggzizld.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3phmcnuph.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3gnlygfpl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3epiejocb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gyepcmet.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gjecfkya.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ofrddpvh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hloabwfo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zhudelon.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3roopbced.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zwklbmie.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gizftvft.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hbarreuy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ypjcciwd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ubureyqw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3idikcbsg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3redlxvex.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pcelkmus.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qdlsjxre.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vnojdohi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3khgchffr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xcuitzlv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zqyoyrzu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ubyxurhe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3aypizvjq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3siiynvkt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ewymmulo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qmakhvog.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdqnugd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3tknfyawk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3suwimccy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pczlcbig.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fmlrxynr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3sezvqdft.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gsdzotbe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lifzkdna.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3egnjvnos.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3nlevxdzu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3veahwwob.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvfxbmys.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fszzawzl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ongnxmdb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gmdyhznc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3sxblyepq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3byuxwwfy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3naqdcwvj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rxcmsyfm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tflknbru.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iktgmege.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdsjizpx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqsogymz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ewyfcbyy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vikoyajm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3icmmwwcq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xbtgwyeh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ehqzylyq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3cmmxdzqz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbcrhbmj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kincjvbq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjdzopyo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3irdaetsp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fszpjqva.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3orqmpbaz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3jcggxlgm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3giektsxt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xyozjdmy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uovwtoiy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tmpqlsme.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ydlyfjeb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jjksmojd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zoapvoaq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wusxegmz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lsnhyzaw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hogjystv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zfvzkwty.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nqdmoahx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbysfnyf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xteejdnr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ttavucbu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bteytzri.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbujfiuu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3diccbqcp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vummludr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpkqvlzs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dzfrnzcd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vzvgvdws.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3juzgortk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvqdbgjo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ddzugupf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3npyvfmrb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dymmgtgz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3brorswpv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bczafdun.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ihcrriny.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rifsnpiu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ecittawv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wwddzuqk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xjyvjube.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rogtmprf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kkygvrax.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cntxjxmk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3lcdsaelz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fozwnvrg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zoqcewbx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ewwwwziv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mgnepmko.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rhuotjas.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gaurkdgh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ztvngzxj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gkjxafsm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zfbccjet.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wxuqxjfu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hxxdiduv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wnudycob.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fbthelds.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gqzilhzi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3egzkrjox.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mwfbcfbp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kchotzdx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3rqwgxjew.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsqcnaec.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wxzlwuni.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3biiasadb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3duieedxt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qovqijtl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3plahwgns.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kwkxibqg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3imllmocp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vknzeklf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wuuajoln.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yniammpo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kkpnvlrg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qmkwnyee.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wekvjjhb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tzuuldfe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3opxskoow.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3offeymnf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkxwuvcj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vtcqghqj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fqmvvxmz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wgwcszsg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fcgasknh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ksowyoqx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hwqxfidx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrtqiras.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xglgtmwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ooifrtgq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vcqqdcge.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ugobckhx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qjojanky.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkjpdgjm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tezxskgt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3twjgygvu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tjvsbrph.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3txgwdgbn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jhfekzya.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dfstdfku.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3aizwmivs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3munlnvhg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqybnqoi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3afoyyckc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xwbbnsfx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3krobszru.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ksdwjvwr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3lzomjldu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bomjrmmc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kgssxzig.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwojnkxv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tfxdfafq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nggtdcff.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbttatwx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wuppujxq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fzsrfhlf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3iziltvsp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ggjfhohg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3keqjbvas.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ljgblvpr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfezymyq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dbqmlgpg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zdpaerrq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3eveemtgd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cvlguigk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypatifzq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wtpeecgk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qtukcvlm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hinpwpvm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jwawesrh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wchzwtel.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lbdjsyss.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ctqfzliw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kkslqndg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mrsradgu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tilnhemp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3juqfbiap.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cqzqvkcn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gcekuigc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oacoqcax.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fgfstvso.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gsxopkgv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hmabbdvv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hgxicmgs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ypisljtl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bgtxyggq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3znijwoht.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lkjyjheg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zzlseylv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qwohtgue.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ejrgnnln.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xlyynsex.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3zhqqwcnf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vttuoyzr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3itrxmswd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3drmkjspx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sqvisbpn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcotplgw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3owugahle.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqylhin.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zhpqhpfm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ufodlbvw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3djidxtul.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgbzumr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3svnkxcmq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qtslqces.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3saxoiyrr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvohfyir.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nlnqpzzs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uqxcfbro.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tyqpbzhy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3sjyzgrmh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jmrjpxal.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3kyvzjauv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mekowzbn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vchsubkg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mavvccff.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kxllkfyy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3eaozbbwk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fznxicdb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jffrbljn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ckrdpkdy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kdyoltln.html


<!-- 参考信息 -->