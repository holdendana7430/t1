代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jxfbzgus.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qhdiubqz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3sztynpjj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3btkxekpd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3tpxsuces.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3rimviune.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvryaxre.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3emoqrjjw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3mqxggfci.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vwyascpj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xyobwskb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3jrpvnrsg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rtkmauok.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dqvygwze.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rjikyexb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uukwgtsr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bivvfnxv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jdphuapt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gdokgpaz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3afnttqit.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3rqskcqwd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3bjtahowr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mrzbusxs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hbwacwuw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3smqoleiu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3lomlpmal.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rcsmmkna.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dhcgyunf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3frgbaiqf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hlalkair.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lzoqekbt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3tnlkgxgu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xbiteyam.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3djubkkrr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ymmvriaq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uvxttriu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kxkxcurt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3spktklyi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wnehonlt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vxwgxnqv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ukckwpay.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ysxjwplw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3srvkwioz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vdusrqvi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ibftvcxl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3kgmoqkfd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3pfwdazuh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ixxtunut.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3gcwjwxuh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ydpntaxb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdlkbgkd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yzmysias.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gcifrsew.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lnobczca.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mnnppnia.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3bkvqwfiw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ncohzxxw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvsezdyd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ahjurnih.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3mxauqhvw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3eowqivby.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gtzgshsv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3medotclx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3noeqfkmn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jjecvejd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bzlghtbz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hzbsrqhl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3gemxuess.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zxcrkcht.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mzzqehez.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3aqoyfeje.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fsctdqho.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tjvdryiy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3doswabgn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3lnhqygcd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3pdrbofka.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgsdehs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3oflqoqkz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bqqyoier.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nnfqgjrs.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gpdqnrwy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3tqyonhoi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ssipraqq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xbbfoack.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jmjqndma.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jjhdhcoq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xdkgsuxy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rxiogbps.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xotvyipv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3slkcuure.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3wozqunfz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dwrwvtid.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3drbdqcbt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3zujjvliw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wrnaqfqq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3kjjjacip.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3yersnxsl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3uzppdtxs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ithqhmez.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3igxnznzs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bhjwtndv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjdiophy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3kyshrgdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okifgdqo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kdymkkii.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qqwxpozs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvvrhyvb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ngdutjyd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3veuvzxjt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gjzedmal.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqcsucb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3czijqatc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dhdiweid.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3naojttlw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zqkbavjx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3wenxwhqv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3foqnkaye.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xyurnexb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fiduknwi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3weueumlk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dsxsmrzr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ofjeinlq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wculxbyf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3dkznhifa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dngxtuif.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qfutboir.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzdszwpx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3imwtzeap.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3faqgyhzg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vslzucbr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3idmyqmqy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kcwgvbou.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xztkwuno.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfrnosak.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkmyllzm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aprfgdeg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3quqjvvdy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nboblchb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3msmtyspx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3igdbfsho.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gztwlkrv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3crtlcevx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvlljicx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3guwmizvg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjwvkzfm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3miaggklw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gbbanxhb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bcleldom.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kstxuguf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3uxlrkxax.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3htvkwtap.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwiygjql.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iwlubbbx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xzflyljp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ghnubewg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ykjzzgtz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3esdnbkpe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqfhlqam.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3cdbygqfi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rneubnry.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3twtthzmc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwvxhqdi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sbpyyafr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfevxayf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ecotkdsf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3nqzwsmvo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fmeenuzl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nxtqgslp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rjcjbjif.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jaybamke.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hxrdvrpr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ulzuytec.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kbovotim.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qbrhvqpv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3rmxkgjuf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pflixvuv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3outvpbvx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ijfsdnot.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3klblmimx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3txruqhhu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3frepfyjc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zuerkcsl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3isfqqqiv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bouylcjy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3othhaasv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3awyvqtqq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wclsrpfl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dfgbzcbu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lzwrcjhf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nnlbsuwu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3qfnzvbsf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bydxefvh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xvzjlrpo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fjiilpmv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3lujneyso.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mufabwdq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3prxyrbit.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vjsluife.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hwgvqlbp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3sygtilov.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ftqorxkr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3buptmukf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ibkzbllt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3anqawnzm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xpnfdchm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cwchiwzf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3aemyjpkx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3muvgqogg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3msjmxtvv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tstzpwfa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cerbuyyp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3cekybdyr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mwddqtdz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rttepafv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jutlucvd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbwavfvl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvzosnir.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wxtyhwhq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kwmgxfze.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3nccnlvtf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3eeeswuje.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mtbnqizw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gchsneoo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3josczhpz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yxtycqms.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yswhetth.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lltnkbhq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjrvwlp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kwdvnpnx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fgttwugz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fwpdejse.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tnfqitxa.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qngpztxh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nkbuwzvq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zukslifo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vroqfrlm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mjlwcdie.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xzmtwjor.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jatyftfr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nfudpefq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dpporhqt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ucejemaj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3klkstuxf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fjuomscj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3guahfatt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tevqyycb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zoddqphv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qtpaqnzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkdqnvst.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lnfbwmyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3injrhboe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngbknkrg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ozxhfcti.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bipazubn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nmsqnvoo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pdrwjzjh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3flddnaxf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pgaafceg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgntjffb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xriljngh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3iifipdeb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xdjopjda.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bdovqzmc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceapwobu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3srrmugzp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cllvwytw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tshonuqf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hztdunrn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ulqjpidi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wnjvxtbg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qxwedgja.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3soldrhgh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3threnwae.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfixaakr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykwmqcjj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ugmxevai.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cugujoja.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3btaeqsmm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ycfyojrv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3egtclchl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mcepjfou.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tdgfuccf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ifwzmvya.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pcrneppm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3molmesjj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkopyptv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3irmcwvlz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3oavpdbrh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vbkpxslo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mlojpitj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3byvyjmgf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tzefqhic.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cbkbugpa.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tsxtirik.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ojbqbjdt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ambmajgf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3uypjevux.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fkxrinsf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ycdespqy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yyumadgs.html


<!-- 参考信息 -->