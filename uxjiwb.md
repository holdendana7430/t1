代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3bpmahbql.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3uwuwbpai.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3emoxrabe.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3coolxxuk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fibvldbt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjzryxia.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ioladvpu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3heyaesxo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ihivugpu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lizxpbcq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yokuqrfg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pfakaxwu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ukttrqfa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ziabbfow.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3uxsszmlv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xjdqauzf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cwgiedyv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3dnnpmzaz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3mbiwrtxf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3shukfzrz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3xlbbpggo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3scbqkkxe.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3peolpmvl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pimiyfqw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vtloobhc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hkimohcg.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vpasixcf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dpcjlgxi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rbesgenc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ctfegxnp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3avfnxqeb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qabrogkf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rztmbdbd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3bbqfwrws.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ifkkqfia.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3lljheddm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mpxhvrpn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3addatzbs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3dmpagflh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3chcpjyjd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3wjxkzpnp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tmlkdtob.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rjqnhzwo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tmqzbnod.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ymqkfarb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fhsgbyaw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ocimahdr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3pyxhosvq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rikyskpk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3otynbzky.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3jvlvrhqa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3guyfzume.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iuemciit.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3neqadgqt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ftkwfxvv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3eaatxpwd.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ysfpccqj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vwhklpka.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3czqpdkci.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3twaiemlk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jowyffxk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nsibaoyn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3elqknfix.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3rttzhmrl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iuqmjzgu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3nwhmbicq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3okukjpjc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nzjldnlg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwcxqavw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ajrxrwdm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dmyxgiqk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3bxsjokuu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3kuufzsoy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zokteuqi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jscabauj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wuuuhvlt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3lphpthqy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nyscoolt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iidozcxl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ebrkcdgy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3viayqgrt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebpktrsk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3mordrygf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3huyfoerr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bhkgungu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3zkqgvcyz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ppveloxx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ojcotrif.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3tqkqapjo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xdtfvxya.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3qobrsaar.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cekojzgh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fdmipeea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyagymyw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3sdeaajxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcwkwlyw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lseemhbh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bkahbfbs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3iwohbrge.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xrtcibao.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3akrpfzlt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pgnmghtv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3tjxygske.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ixlxlqxb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ffxiouqk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3bcbmucsp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3osqhlhnm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixbcqszh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3haqbxifr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wwwtijab.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gzcromfg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tqkaevhk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3gakstgbx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mselyhix.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3xwkzvwhs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3mbwbbabf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eiahhiiv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bbjqozrw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsvdhcdz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ielqcgzg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vpkfnsgg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3fprbvyyq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ddkpdbth.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uoylepvm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cxiteslh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytlzwpge.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3umrwkeyu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijzrjkvv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3yavcgvta.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zmkebmmx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3uclktqto.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcapjvcg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wsnhbsss.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xwmwnafg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vommcpgf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdnllpxl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3axelpilu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbybqpvx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xlgytvoj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3glherwhp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aiecnjzi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lyufylvg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wcamknxy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3atmbewfx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxclwuza.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gnpyqryl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qvjknmua.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3oqfonjvr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gnzcxhbs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3uoxwlhtv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jdyqbntb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qkfplveu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvxyetbf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jguohyhx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xdbydgad.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcfjlyjt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kkhkecqi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3eoeuexmg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cdllhydu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3slnwbkpo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hmvypdpm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tudftkca.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iocbxmgb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wnxcgbfh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3idvcenny.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qnzzvdby.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wfcpnsnc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3brjxnzmi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mhywfztr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lqvrroap.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwrvoyky.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3brcgwwuq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ufzvwmga.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mimnswex.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bgxbczzx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3feprifwm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbxmqqow.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jukajfdz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rflbojwi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mdnyxmjd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ocqkqqir.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qousumnb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkbcehts.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ulhgnfhd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3akedgaem.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhamjfix.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tmtwhwqd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3gverosml.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kseztswj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3isiminsu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zpoklteh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxhwuthp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eadtvlgr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3bsdnztfx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nqonmgne.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oxabfczq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nbfjxqwt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zjbrjslx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nyxmkzuc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qkvesjgx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rniovvar.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3eaidlmem.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rhkfahxo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ujpddxku.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xbtmmdcc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3oqbezmka.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tuxpmzlt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xveofauc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptcissef.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vwfygdhs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cetdjrks.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ppsymdxf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pxpakckr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wobugyuz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wryxftyn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3eyttpecp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3odshltjp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hibhjuuh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hgkxjcmj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vxfjxpwd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lydzwlpy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wzdoprxd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ikpulzsc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fkzxqnvr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uofepgot.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wykponfj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lnmqzaat.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hvpjvjfx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wkzwqzee.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3elmhesnj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3chubwaoa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fsfuknwk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3izzeneji.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fobkdkmo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tusiepqi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qyinfjyi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vadnfkac.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nowdxwzo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xdulsgxc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hawdilrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3liettgcy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ojlxfrkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frnvnlxr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3psvpgbvd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3tmyyrbsk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uptyszyx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3orhaejhw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzishyjh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phiclrdc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bxogveke.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3rvkqkzpc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sfiezfig.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ezvmvvzr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dssswipv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svwumigg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lspfvjjh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iijgjdwy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kdqfilas.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3grrrylxs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vmdxtkhq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dsjqmaga.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uxdlwucr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3laiqlxaq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3arkpajpf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrjuypmw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3geyckpnf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qahdzfty.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dtwzyqdj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3aleulfzy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nclcwbai.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bqnznfqy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfxnoqkl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bfidavfk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fddejrsx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qmwrlavr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3smegdqco.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hbfztpkx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lprxwutc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkirscta.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3nfkplixl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cbnghpts.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mbcuqflk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uscbpmkk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kdqjztub.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jziaduxe.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3iepiujow.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3umcbftuz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3escrtgua.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fqyiehvm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ihaguvhp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hpxdqjie.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ixajkjoz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gdxesvtr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3zapixfjc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nkfnekko.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ctepwcgl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ypqovhhv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vheuresd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bvkbqptk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xoflhean.html


<!-- 参考信息 -->