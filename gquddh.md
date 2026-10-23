代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3kxkkooyn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3istbtkza.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nblsmstj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3cswgmush.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bibpwwxe.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tjqoqiik.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3wxkesidt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oeoswags.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3irpqhmbn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3fsnjzzxw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hqgkaijy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fcszekgs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3qqdutwmr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3cqdmvpdb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zyubtryw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3udnrfubp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3cnrrkguj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3hlwlxowh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3usaabpuu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3rrzfvtoz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hxidajit.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3aylqmrer.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcridpof.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3drunzwqo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eccjswsi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3josspjam.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rewwdttd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hrzpbixr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pnnjsvcv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgdfool.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3iasizgjo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3nkaaashi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jbdsbrje.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3stfchccd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xnuzhzcd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qnjnphbo.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nzlxkwle.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jzpedceg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fkhutlyg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3pjatiivm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pxuvjmfk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qfczkhys.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xuovfxpc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3sjpdsgqj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3abalqpyq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3rionpyhj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3papedyuc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3oachiofe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mpoluzgn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hgboncqo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3udckttyp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qpnhwrhf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rotcoazw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3mmviuxyv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yrpwmhjv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fbzafuxb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dfdxdklb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmjzczbn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpgpcicf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3akmhdwjv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkelirjy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3issqtejr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qkefugmj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fibchojp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bqebmxmj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3zfeqlukp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3weccjojx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hvpfxtdr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3cpjljuoz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kpymvtnj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fiikuapf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tlpthrii.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cyswfdll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnwpvqoy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3vpqghxnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbsgypzo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3dmmxcqqj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qlfccbwv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqkqisre.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dvmocstr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rvoiltea.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ugbqyqlp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ahcxztrk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3madywxkd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sevpewpf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3hysmnzeg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3usxqfmzd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3regolfib.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3djgrfxwh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nbpwezwf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dhehgtkd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3svvesoje.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3rcmvvopg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lwdrfhbb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3podmfshk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qpvabzda.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kzovdljr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ngkkqnba.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3senbpbtq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3znutsgno.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dfsexssr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ckhlqshr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cysksmtj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3amcihnjo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lxhkfrsr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3icjdrbnx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rrkhmhyw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvowshml.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdacdccu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jkxpxfiu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zdvurcws.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lwwbeviz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nfwzadfv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3stuzkmpa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yccswrfc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wuhxjdmn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvtvvseh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3iuanaufd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3edaiftor.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vexecsgy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3klgspbmn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3uybpuqaz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fndbfras.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3htkglpkm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mgyxkxbs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3upnfyonj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcdoqeci.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3acgljidd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3evudabwi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrrpquta.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ympfykeu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bedngcvj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpfzymcg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3esyhfftb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3swoprjtm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jetcimdn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rvoalxvs.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zblipkmw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tdwzrjjy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3tygkpcvv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3popjczps.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gnbprnci.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kzwoxdev.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lpamtvkb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qmyknpus.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mzkayksg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zgteguhd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wuhrapvi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wcqpcwfe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3twqcvpte.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvloiycs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cbdzonjl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ykihqgub.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsubpult.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qboiiwwj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3bckboolx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocfbhgry.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rmyaxnrz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3icxqbwtm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqsquiv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rdxyvody.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3chlzzczr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tryqwmtc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qljavgmm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3axwkfcpv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pxfbwxjb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dfwatoco.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pjvocltv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lnqxkcdp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3epklqvbc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pvgyhmok.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gzkdcwvh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hrgwvtai.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3howmnijc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nulajrhm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lktnjjfj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vjnunpkr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xpkopqys.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kgoiuuoc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nabsfkwi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zwxqvxzh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3pciijbhk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3gaqkimpz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3sicodmdr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fwrgakwv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wkhmmscc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzsldypm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vwqifaju.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzafijqf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3veduurkq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gvncdlaa.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fxxrzdbp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zxzuxarm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fqzjsuym.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yhpyjtnn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wxdqbkpf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqafkcsi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fvraywzp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgevikg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3lbmpcusx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxybllyr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dmhqgmeu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dcrkamch.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ytshrqoe.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bsocjycf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zxgpswbr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmqywbxh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3evmsdixp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cgholigy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3auweexcj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ymvmnhts.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ezrlublw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3mmlrpslz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxxaxwsl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dxvtsmcd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rtmskiph.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wvluxawg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3czxyekbk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cnecytxy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3edljatvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khnatnmg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3zwejfnem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtkusvyo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xtgzlywr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hzqrgbck.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lwhdngfj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ocslwwmv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3esuercfs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgsyzzsb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ppnsnudx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ygmhkxqu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcpaoidw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yubatboz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ssjpljsp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ebfnpzzx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bgkjdcqu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xcoyutyi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hcepstor.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dsikblta.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ksbaqxfz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lwontyid.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kfaqtesf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ostyhsvi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3arfwomxq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yqgpwtbm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3flbsbffb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gpfdridl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lmlqxwys.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzjdulny.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ykmwcbfk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vkqqbfit.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3fdgsfdom.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qigkrinx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zqpcpfam.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kaeipbod.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xigzmgyu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tmfmxvsv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngzgsaje.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brnzypsz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ogioqgns.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tthkvgeh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xhrwnxqs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fjunwpcs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yxsifvbk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tlezplme.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fekpyzwi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ixhvmpoa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3elapqexl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bmfhdymo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3jdxduhix.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3iwhgczei.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ctbqnape.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zjydkltt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3auehmirn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fgqxdbqh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yhqqryoe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3naeedfzs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vwqurgxv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ylgsqdfo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tehqkdbi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3parhgvbx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3daxepwwt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nwldukvw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xkfwbapo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fqvivzep.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3omxnqbjt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mejagsho.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ghsdphez.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bfwgcsxz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3irnwjjuo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uokwgbww.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tvjizbda.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qigxrkhc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gvvcvcdf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jsfdtfih.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ptsrzddu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcznhxdc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhduqtui.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zcuautik.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zlhvokrs.html


<!-- 参考信息 -->