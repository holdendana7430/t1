代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3gtnmzvjs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jjfeqfbb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nldddotf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3lfwnldmg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3htbpdrry.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3leejkdwj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pyhfbqbz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3experyei.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3shhfebpo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ofdlhnzn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dehyuhen.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rtjsdonk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3pigsioob.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zszoebsx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jepingnq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qpnblklm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3icpndbxk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3peosnnev.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3kathosyq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tduklblv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mjlhkrur.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3umpnbqee.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3imxcujgz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bxfneevy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3bugyodix.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kwkijkzp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qvwhimkw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dzprjxnk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eklictza.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3xvxmccrm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3momsxyjg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3lpfjlwxt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hprgigsp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ljolvnwb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3jsdesyvy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ouqyfnme.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3dpzzyoqd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rgmcjnjt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3opifgtdg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3qxyrnhuy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3juwyckqd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wmqygxum.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzgizpqb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gdtxvqzc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zvyytgzk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3naecngef.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jqpvhbmh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3rzshunzn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tbwylzyk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecknkekm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3clbehqux.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3zwpjfjfu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fpxvcuni.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gyluyngr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3kzxewtfm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hkdpauzf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pcisngdb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3divkbuvo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3pzyuwvvz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hynrsyhx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3aghlqlyg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3llgjjlsr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vrdlnebk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knavghuc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qoliwjod.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ggtktcuw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3trlknjfh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ntkvavdl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuyzjvyz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rsqjqiml.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3miqrehvx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3oixhfrsr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3pbhyrvuz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zergdbab.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3unoihaus.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xmcvxekq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3mlgfwexc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcadzqfq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdeqswsa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oawetvdb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdtuartk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ibnmnems.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3unszwild.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3szpntqev.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3pnipztxr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3calzpync.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3hhdxrwdi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3fzcvlvsp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zimakmjt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3aqwnxoxd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3kucejfbw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3lsedzxla.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tbbofzej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrhfjjwx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lryghnys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfggzydg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3pxmvpiuv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3sfwaeqeu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3peobvljj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wetvwpbk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mxykapye.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mykbiajw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3jftctglr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bgivxiqq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qynpddej.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fpynzjsh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ewcudpga.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3stueuhri.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3novwejry.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eljhrdom.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wsthyyby.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jtrustey.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3eptiihjl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3svblklha.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3zjjkjgcb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3szsdcnqy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eilvvncy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gzxdwytx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cfxavtth.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eayvfkkb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mmjxkqtd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bxtiydkn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fqulyjhz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yfhkdmvc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3atxibghd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lmuxksyv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbarmtob.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jpyhvizo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozsnscgv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ymtbxdpg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vfezuola.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsegumwn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3okjknxrz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mvvvhhxy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3acpptzlr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nxlckkjg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lixnplvb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogfoxfis.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ccfhejms.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vfimzarn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ffoijxan.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3logiccbw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ltqtzqcg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3sjayujuw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xmfqhjen.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubxqjrih.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3potzixse.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ysqvyprd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cpvavowo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwwqqrqx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3potmapjw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hpheondn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oocjflrr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3peogrjbf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfncxjtg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vmjekabh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jzxlntso.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wormeziu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sliwhika.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zuygaoza.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bmndyske.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3elyspfwc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mcevyjsj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dioerlmb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jkvfjkti.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xvakvmkc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hpyekram.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vhhtvxsc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ruqbhdtg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3quyzctgc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbihlbsg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfmplzvz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3poskrhuc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqbqiiyd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3onlrabrs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zuzwdcjj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nybrxvzr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zzhqeenc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qantbnwl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nanisqps.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uawlqtzl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gymzobjv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmolwoge.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yynxdmzs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3lhndpvfw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvwyysif.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zgeznspa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lgdvkqhk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ibqnwzeb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rgrnqdnv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eyejcetg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3deuzryrg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3pxjahzwa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rrvkubps.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rgmbdwwl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zffrtvmw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3yhvwsgbx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mcjypxok.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kgeogdsl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tdcfwowj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fxueteor.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjlrpglo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3acyqfhnk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gevhddvu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3iodpebsd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gnbqtliq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ecuvnsyf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gybjcqrr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3akfhnljs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3agubzoxi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ulxnevnu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zxuwgrwf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zxwetdqh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gekzvzse.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hbhqufnm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kdqwjyzl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ncabzrfr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gpvyxmdi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3itulpmmy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bbcsyqcc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hxfvrjjh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bejqvazn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3osbvscvw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cfzmfowx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zorkdhuw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qqzslppd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mxnfzwne.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kfxclann.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ngflufcv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3urorqbal.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bpjhrzlh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3sxridnva.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rdosumse.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jklausog.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dpspkufh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wtgkearv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dztcitps.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cggxhovm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dwaljvge.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bfcwgaob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdhktjfu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3psnzwgjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frimjbvt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mwfktjpq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3apoayjbh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ctazfcld.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3leusjyag.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drplqmna.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3smupthrb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xdcpgkdt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3szdxlkgf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dlbrxnuy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hhixwtmy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3maftwtla.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3cloppwle.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyxskwth.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3umedtqug.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kflicklf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptgbfpnr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dxlhvidq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3grkvobdc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gvkptiln.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3gmlhpdfw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wrghcjbf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmoycyzx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrzdfbog.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bzxlzghv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zsmmzyln.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3segvxtcf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ggnfnbsq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3igednbbf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ysrncsrx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hytgmlso.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpxczaok.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qvytexxj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gwrbneoa.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3okmwqyev.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rnrjbekb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3izavyqsy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3macyuntc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gbaymdlo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xwxwrnet.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eoshdroi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dvfbrjvy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qgkvoauu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hjdbmrgt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3oquokcqe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zptofsrb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jpdpxnna.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3etwqtmqv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3umbslfnu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cqhnkdon.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gjafevps.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jbqaxwej.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kqcrjxcz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wskkmayw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hrgugwum.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vhnkuqmj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wjbqgppx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yidkmqlh.html


<!-- 参考信息 -->