代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfmsdstk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bounuclf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pphmrbgf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3olkwpjtg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3siuocidh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oizdlrvi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zoptszvr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nmjganic.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3vagzoywf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qfyrkmgg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3thvygtnf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ulisbvsr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oxvybyrt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3fupuraib.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mwulkxpg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3zhahvjkz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3fpyjkjtx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3pkdvdtkv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3asigspzl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3leyecwmm.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3oleojgde.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fkyhctfa.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xvrwtgtd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sqxoojbm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mpmtdbpr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3cksnduer.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3yzpkrtlz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kudqeprs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hjaqhhyw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bogmojdd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3coamsgos.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hwwkotty.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wkocbfjg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vlgzhozm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3yformmiz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zgpyvwue.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3upgixdey.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ucvcfpvf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkxgbtc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3inpammlm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fitlbyyi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bsbmaoop.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ahbplmdg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3aquuegjh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zbejnrad.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnrmkyjq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3jibiiiay.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3anvcmctx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3coounrwm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3afndkpno.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ycjtgduj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vgbldndb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rrrinrws.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3newilcry.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3auozrdca.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3urcpeaib.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xleegtbh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tzlbljsy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kojqqaqf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3vlgxptnz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3evuedngx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3tqgycfvs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3yvzgnnpd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nknqnxrh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ehvouxgy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bjrspzjn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3comibgbm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3hqsrnqmk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wssmfwox.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3krqpgjeo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hkjcedug.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvxtgiaa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3gqwflygo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ceqmgalo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxtbidpt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcnqyfzp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssfzjcyp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bxelepjt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ufjvucpz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kddcdxrd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bxygvxjc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3yaqaiidd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3tgnrmcfx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3mvtidpac.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3gotwbbjw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gfbdxcbw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jpewnfxl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3uklsqcxr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xspdjnvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gacbhjzl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wdtfzeno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnxzgbza.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3izijxzga.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wwtqxicn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3etdvqesq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fjoeqvfw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ghpzttif.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jeuzvhum.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3itgpkywr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bcjisgiw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fzahjkuq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3mqizhqvw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xwronptf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3trpjtryu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kiptyldu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mnwexdym.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xfksxgux.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3oafetwiu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3smuobonj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3olzlosnw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3stdlyhws.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jeogykfv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpjixxjw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xsnavzca.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ioamwekc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zxordnwc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ghcvoymm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3zguzwman.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jfrndkqr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zqgenkmd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xlnmqupm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zifgoyhi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nssppkqk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgpuaapx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gxcljxfv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nkquhtjs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xzqzjwzz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3njaaqhtm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fabdraeq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rglwoylc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ljixlycl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcifeloq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zyqmjtpe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3jtvqpazy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bkttwjij.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3cerkgzar.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkuctzno.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gjuipktw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3cvhkiwbx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zesxmcik.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tlbtvrpz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtdtvxxb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qhlzgtqd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uyyvmohr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3svrcbwso.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmqkmxym.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3dvkuecxp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qiikbzlc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dcxpxfec.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukrnekuh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dasycglb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nxllojyg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kstfovpv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3zqsuswlp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcomsyob.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3whcaevbs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3btmafctt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dtidqbbg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xbqgrtqa.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jtssrtlr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3brlmosvg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zrdoaujt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gkpvkvad.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lmjleilh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xwtrjkhz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mdgrdxvy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdttrppy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjenlmli.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfksszho.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oorkgtmz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3geksrtyt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3edowynlv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlioafbr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xamdlioo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3sssaqjrh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxuubvah.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3memkvydx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rwvsanww.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvpouluh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hvcrebkn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ncmeyjpo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cogpfnqn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yngmbsqm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3guabyuct.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kgszudia.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fxwnwhjg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3oqoygesy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ambaglsm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rzyvnncx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3divnfjak.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ycghdllt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3shbnbtcn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tppvfrjc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zcryensf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yqlmrfif.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eqnjgqem.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3menfewic.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3badggppm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kqbezmve.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3lnphxaee.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ziwbhciz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vxpvthiy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zsnytght.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahxggmjg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwtzlolg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vrhnpzxb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3yfusbkfe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lwvmucsr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3sarwgbeg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3klyskgrh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kjqpbyuu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3oowhlcyp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pkllrbpd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3orzkphnl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lclznxrj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3acchjdou.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kagzbkfz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzdffqbn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3mqswuuep.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rfjtyehw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pxlxlhue.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3caxrebkh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kuxlyges.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dzcpomdl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xwbaonxx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sgiupevd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xsjdzfso.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3psvxvlvj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ctilvgfc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ognluasq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fhrtqmyw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3etwlucgu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oykhetsg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3edngxlzw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3lawjtuqn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3clqwizdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzatkckp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3isprbdjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycwtbfti.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkcfkgid.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3lpbiluen.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbjluge.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3blbntfwa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wmefvgoh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wsncggct.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bbwkollg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qfdtulpe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3riyznbfh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mttcoblh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pwveqmjv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghlxrurj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3exljsqwa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sdqcqnuj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jvujqljz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fxzqiigs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qppamvix.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vkckeqao.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3enftjqfe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vawfbkqp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjhussbj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mbuuoxil.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rkuxnovx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3jmdxdlma.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3tqopdxor.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3iweqmqfv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cwqgbudn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mbzvbdhq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxduqgzc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ytfjdfxm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3amikrrvw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yztitxsb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3csyyxukl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rsszooar.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzutajep.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3umpunknn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ocsmyzdp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mpwsthpd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mixhheaz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nhfkjvau.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3raldermv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3naqnqrbq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vftotxbc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xrvxbcnq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3utjshedx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3cuyisuid.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3smpifvol.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nnuggzto.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tkblhdib.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eyghdugp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rfwhrtin.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3cqhcamxc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ovpjbrbc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xvdevqnd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xqmedtjo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3htwcbzku.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vjohffbh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xuizckhk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zfnskjxl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wjkrldmq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3grurfrql.html


<!-- 参考信息 -->