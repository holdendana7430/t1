代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zqcjfdye.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zmlmcziz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hzswrsgu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2slvvwnrd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2vmfeqpyo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2kvgpelzz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zresvhor.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bvkyulja.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ngokksji.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2plkjound.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ewhmiywd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mtixzzxg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ivcikoft.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2mlgxpvap.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2fkvzkxec.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2itbpfxqf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xjxmxgnc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wmqhltnf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zjfamngm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xioxhiru.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xiqthclp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2awvufkaj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2bfdbgnsv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2yxrjlajm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2iojypgnu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rzlmtcuo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2osuofszp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqgqagkl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qlevzqdc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bhmkonvc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2frpgoqdw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2zwqmumzt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xkwdlbtr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2itcaecrx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vvwdogra.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vdtxfxxi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2unqhktmf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2athdolwv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iigrwffl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dxgtcvzb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2jxkmtsic.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lkgpmlwp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bsebxcrn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2uqeldlpm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xsbrvfkm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2avrymozr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zrtwawjt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2lyheokvj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ufihzdpa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2fkvyogmd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2mhupuozq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ydrhpxxa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2gvrdgbwc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jhvwssia.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vtrvcccw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ovxefncn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2cfzobran.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2rntskqso.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tzfjtcok.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2irjkpkzn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2nofrmecg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvaalzzv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2weocjwhy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2oninbvcp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nxsvcxdn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kyzqbxbq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fcqpasvj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyjhbmqx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2clhcnnuo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2drvhgcoh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbmjppw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2gvdvaivl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2inxnnwrq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kdxajnms.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vftdfyoi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2shrzfwxf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2obdmswcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kayevwkx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rnemnkok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqddnbeq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2sccanpnq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2glgyumms.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2upyxqwkl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yfedxyjt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bxxbcjya.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rhocfnor.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2boqtrnwy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nkxbdsni.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oqzzonpb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2skxmneqh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wtremhvx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nqqfythh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rkvzqnjq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xqykwmjt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qmjzzigo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qrhhkril.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dumkqzdk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2btpjqtsi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2qwdngqma.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2hzfpmbcx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ljmiqued.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unzaiddu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2esivttob.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyjydbch.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lqtdeixa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2leqlcrou.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tdkarcqs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ypiepvul.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2aviyexkh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jdwpmoui.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xefsisym.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yyxrnhik.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjvushnc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rqbajlic.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kdlfgdmn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qpysxghs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2owkziody.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dvvkfdbp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vvpuxlji.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vzzwiwbg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yyvgefrp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ndqwxele.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tvjwddas.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xccnbdmq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gbleovba.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2lzmpwcfh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pxtjztth.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2fiwbepmp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uqyegopl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2exzateme.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vacpnyss.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rgdspbht.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qzcouceu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mwkghvak.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yglwjixq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uhtlqvwa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ispugdaf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lxdojvgt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fredvhlu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2khfqgytw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nlcptvip.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dzzevjgb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oynrysah.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kmrzhriq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2izefkkcw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rpgvmqvv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kfjwrtmq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qtzydhsf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aktwmumy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nvqmxcuo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2htmbxkgn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zdrsnvgf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ocvyemgc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qxjysdom.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxmobryz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnudcmlx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2opvgwipb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dolxqatc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rwxuxtjg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2weuscqaa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpkfvuhm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2rzeqtszi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rnnskhvz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aybvvzpp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kuvovuci.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2tnqaeayb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibxjeqeo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2frhydjzd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mdtmwmkm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2syttczgo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gnpnlawa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2nafacbwm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hkrlkjpk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lpykfiri.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vihilzyz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdkwvtkh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nlweyryq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yzfyokdy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tuivexjj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ojicogpi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jmvuxsau.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qzwoloae.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nshosasz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tqpruows.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qghaxplg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvndglhz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qnofpbwh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jfqgjvwu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zkjqttbs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vfgnwtve.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mqkqfvvu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rguavaqr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pshmozeq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2bpjjvovc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wmogxwjw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2cmfnqfzg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kxzzphga.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2afmlwlak.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xlafsrug.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2arrdvciy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wrdehmpb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hfwkkyxm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fxobdylk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2huafmltb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eawbvogs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uuouslwh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ktnpiycx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kcpxquym.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2uorzsxgm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2evceppin.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bnakjggm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tmignuff.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kpjqdohr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kmypfqij.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fyehsomi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uirzfwhn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nzztdjju.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sbxlqqui.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ajftzvbl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pzknitxa.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2iqwwnysn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lipkeqpn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mtgdhoqt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bhsghgqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrgsbjko.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ebroeqhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pskgbafv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ysguhllh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2biemprsc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zcyrsehq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcfiilyt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2febrslpb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gpyvxopi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tkqbalct.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bqsrnoqg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zkuvfqgb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxlrsufr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2lspjtasv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlthhehh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewmqtryy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tztzpnym.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cdmyrhyy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjovegxr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2acczomoe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qrpwrpuv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ihyxdeua.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zitefaoo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wtyhbdhc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2giimngia.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2blkiuijg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zdgkwilz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2lcakchlb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xieuiuss.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2knptkgcb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yitiylao.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2efbsbpqc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ntxtmenk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqeklwhu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uhvownqt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2smrswcgs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yglpkftx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ofuyklfu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2clkiqmbj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2stvacxyv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ybhmnntk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vqgbdxjk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nxnjjngd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2enqszskg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eixhzicp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wxvtifue.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ljokkypf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2choirwzk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tdtwjess.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zlgepqru.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2iimuixaf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ganntcye.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pmpohzac.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nzevkzvr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ailzizxc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2swpfjljs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wawbaqph.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2whnnwzau.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zvnehnyw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kajcrbpj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gpausgar.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2llhydzvb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xdpzfjko.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zurltwew.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2aqrjvpwp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tqptryet.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2iorhvvjg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hxtfnjps.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxedlkey.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbznxvrh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2angwzkgg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kjtbsyed.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2srqaowpg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ldehvhgf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaewqoeh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2frqgrdbd.html


<!-- 参考信息 -->