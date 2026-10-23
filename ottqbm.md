代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rjdkhsuo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uxekqmhu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jrmgtigd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tsrckuiv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3boalcyoo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ghprkstb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mqekvutp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3owhkxora.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zjojxjlw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3capcbrcj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3hdmlyedz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3uqluxind.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mycinqyg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3eqosvmgg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xczxlomz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3yeidagrg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tawotgjc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3henuuvzk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xfxsumiz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bfhdprsc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jcqfhzcz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3qanhwrzv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3myenkstc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jbvbmbcf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rtacbpex.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3txzxuall.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vkzmnxhc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3kniarjdg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ranknkjl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wvlyyuqe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rlteljcw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3houaegwv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3xfgvqhyc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wmmnaugg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcjsvlkh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzsylgtq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xosbhtci.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3aipmlmds.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pplocdbe.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ifkbpysr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jgdyddsh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imrkrsvc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3txsnkbqs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qyghlcjk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mooewfqo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3isblvdqz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywrpdwzr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mczlhtuo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3derpqksu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bsmhjozl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xljxbcsu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yatukjeg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jkivgnmz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nawfateo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ilnbytmn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zxrnezvx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lysptlhp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wbdkrnkg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3qrxeahmj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3itbszopu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3iklrprzt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pxmgvudg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3niehcsvy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3egikqagq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wusqnigc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3yzuvcyiu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mjbqlzbc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rwphjaoe.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ahvtzngh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3bwgytvvv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qeiuyfbx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vymprnlw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xealrpfd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzwaqfv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3szjmahgb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvhizjlg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ndbmwgih.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3akubmgeg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3djlrkwbl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ptzzqcoh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3kcrzaruj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cthywvjw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jqwdvjhe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hfdkxbmr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zgcdhnda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zybsbhtu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3denfsdak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwjchxvx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ycoivmhy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wspvhxkd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lryhddrh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mbdxbjgj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yfgqfsbg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3taxxkrcg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vudzusdt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3njxuiyvo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3idwvrvsw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3nidrkrha.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jgejfpcx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzjjryrn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qviyhrub.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zyryxyeg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3esnxtjsh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yisodwha.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3prsnvzbr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nnontqms.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yriorvnm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xrragpcj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ztpateec.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3znjygmke.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yhaezwrv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqvpqjit.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zddgwucu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ldbojesv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kpdbmojw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ujljoead.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cieyrluu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3kiqsrrlr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jswwygab.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lggiqpex.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ogwqnukg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hmawhzth.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kqcysxaw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhukkylc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gnyadtqb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pzmvfrch.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gdwuwqxb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nygddxmd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rdjlfieg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiipojmx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3auwjcaab.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3crbzptio.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3njhmsezm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3pqgvmbma.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3nqeowjke.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qxyzahby.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qahajuib.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yemneimi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tmnlkurs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3bkcurwzm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tmjawnze.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3awnkgmxn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3uactjazp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3opwveivp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdztdnxi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3avddygyz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfoqcav.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfxcgwfb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kazhhbib.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qldpsdsa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zlvarthk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3cypqhrga.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qfhrwrfq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xboiyjoa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hucxmwmq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wbuaaplh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gwkvawfk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mvaomcqa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lietobas.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3axaxnrfp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3nivtflsi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cqidmvrz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxrmasse.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vcqnertq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ecgfmyjq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjgovpkf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rqnrfrgg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xrmudaow.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3laodisxj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3stletfzp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uhpjikkk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3iczvrvne.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3csnjyopa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3btmhphvq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cbqbkayu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ivztyitk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3nnikmfvw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmfmrljh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qkycyywv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3aphqmiwz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jdogxzlq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nklkqrvz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lauphrik.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dzdvftlo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3okeiyplp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aynqjcbk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3tghnputa.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wuakxyky.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3rwoxneou.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mrqhxddp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ufttaypw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wddiinjz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bpozadea.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tdslgnfb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qbgbuxsg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3igjueyjo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3luckxtps.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3mjfcrofe.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cqqavket.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ipqyxbsu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mecpobae.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3aeapbzts.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gllquhae.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3otddewuu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3itwsazns.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3dzzmuptk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3egwgoczq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jtxmptcz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mwrpoauu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sxzfprlj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymiaemta.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltudvulc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zzykufwd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggaghezn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vzcbtnhl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nilvxrko.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kpqvkclp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xyzsrfxt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xxwfnowi.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hlcmpcry.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qltvuzpx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qocgohue.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pjdgfrpp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vuumuozb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nykoanqk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3affiaqxc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fafawkzz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3difyvcjk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lfektzza.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xusdbjnp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3iprmwqod.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3akhldrec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qokulsny.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3glijbngj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdmrcixu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zeobyftk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pghkevwf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3guneexae.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtcucioc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3meoogrvc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3egtwpgln.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qnqgjipn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3yduogxkr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hxzmqfse.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ynetkgkn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ubhivskp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zevtdoed.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnvuapyw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vedtraza.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3igixwssu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zufdnope.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zcmixrvk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uxszojof.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdsfhpyq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3tfsqwhuy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3jaqzrqft.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3txjnrenh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkqmrihz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wlybvwmy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rnadkqxh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3tiphiljj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lofyxemz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qdwparls.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3suydiarl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zqghgjxw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scuqlpll.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xijlyhps.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3vmihwquk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3numlsrea.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mokrnuwd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tgxsvxvk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3byzvrapj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ytptimub.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3sslyuvqs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3akxvpkam.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jsedwlbt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cxinukts.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3txrjmttp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3stgmbzrt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3xbvwotop.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dfluspfg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3psqbcrjm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qqbeembd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nrlxrqzn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lmzrjura.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3phkogmeb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3exdscmos.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ecielkhp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vfvbbcsa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jqtagpnb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3sufnxcjw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rkjfgbrr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3oclhswii.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwzanbs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxctstgo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xzprsxeq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dnvvjpyf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3azjyitih.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xrxfzsjg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3sarpavzj.html


<!-- 参考信息 -->