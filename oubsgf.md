代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3timjzxnx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ephenhdz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xknzqgsa.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3guyuvbgr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yigginse.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xfslogfd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rodskvts.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ojhsrlhp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ukjynfdc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3knyuihgr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rpbonnyy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rsajflln.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3vwhkdlot.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fmcuhzvh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dsjdxcyb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gufcmgvc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tcuncctx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3xgludsxe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3cpwnegko.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3dbqapgys.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hvctrknl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ysxygjkf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3keubaski.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3btfyxqla.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vtrtzqvm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pfdsqhcr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3gdbhwvjy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ajtcxntd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3aziendot.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3dqjumvxu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3tavgfitx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3olhepfod.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xjqxbpsr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3lehspneo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3yktddfks.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ylpopxva.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3seazwpfe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vqblqohz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ykuunksl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ruzgwevt.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3tkcjzbtx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pijsagfv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cwylpoth.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uluocyct.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jyiyciwa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jriyafnk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rqdsklgv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xzmycwbc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nwnhfvjg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qakqjfzx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3nlismfcv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3vukubblp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hsfijbps.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sfffjdtc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3putrxnwm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ubfzigmo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xofmrodg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pxmtllte.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ombntyxx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvsjevf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sahvjogs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3iiuoungl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xjpfhvfp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyblvwmx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3emqxijge.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3rvglinbq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3vdaggbmb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3tueihbts.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3iwajilvl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rvxuwmhy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rmymnerj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3oajvnvyu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssnmqpfu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3etunhrwv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3moxmkmwk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jtxmtjiv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xhakylkk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhdizrg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yjjlmznn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3byntrdat.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ewbpgvoz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lqtrnjyf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gqeckqpa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnatilpp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3uvlqzisb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3kbfdinqb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3sggofvte.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ghcpvesu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zhpciexf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bpbjylqc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xwesjzmi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3feppyaxn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wffvldyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsjkdlep.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3yuqnadot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3roavonkv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3zkyytwzd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3madymkzg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utmikksa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vnoqdbio.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3snwygiaa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nlallrxb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3dasbuuet.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3hvurlbiv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hywipkhh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3gqdgtkog.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gcaanuwl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3elaidnzw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lcdbxkjx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hstxfioh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hczchdml.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3jylfqenn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3egddodmn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ltxlgdfb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3iqbupmik.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pfxulbnj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuffjysq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpcvcnbg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nukooiyd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ooeqegdp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ileqbjdm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tchiqhxp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3semierpp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wfdzuljy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hqqmiakn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ngshezbl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3crodejsl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zbgbdjdz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xahkkbma.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3uojlxjzx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ijesajpq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3onlzukpw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hejhzfmu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hycpcmgq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zcueersv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fljpqipt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cbgvjwmq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqgnylde.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3letkgwmi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3eqzitcqe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nrorcsth.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3dicauivr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qolbjxhp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifypjqpa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcirirxs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wgsjnnfb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3yjbrzkaw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3bagcyvfw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ieqrlkfh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3otbozvpc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nptcbjmc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vunytdfu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfrlrxdg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcweebfh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ulnubetf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3drsoyufh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mdisbygb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ujaljgnu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lvsvlmec.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qavenvzz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ntswwcow.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dypacwcd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3crrdiybn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jfnaxxgo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xqdzwpyb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vdhmipgl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dgnupnwm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jmhfganp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vbnhdsyd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3vyfubybt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqaiciuv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3abrzmtfy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hhhxhqvg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmvhgekm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3onizxyrh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ztluqgcb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eaunvjfe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xjeunvqx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3jkirreza.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vkznjarw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rrdsdllq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xurvltkp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rqgbjioz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ryvhfxzy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3akusvfws.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbxkhhnh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mnosjebw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3oojvgnff.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rxzjldzu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bqwqlpon.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fipvlqwi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3driuditx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vpqitjhf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aanyifyo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3zxnbjfbn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3krkgfdjk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bvdraoer.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nrikabja.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3silksejl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ozkyumst.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pncvaxbk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vgqnnamz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3veyosvzv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tjaudvip.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3grveymbk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pkbvvvjv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hofqehlf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kbsgbirz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrifhegi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3gebsxlzo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3heiaatas.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fheunzne.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3syloctiy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3avvyvbhw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bndtjdpd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fbybunfs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jngljttf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tzsyjbcg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3slicxtim.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3avglchsl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zemsubad.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3admmorvc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3okpqelzz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pwkfnqxm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3angszvcz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swvsuswm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ukzynmvy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gjvbtwwo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bbhkzmeq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hncqmpaj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qpnypjkf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uvhiadtp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pkmjgumn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3bundlgal.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xztctpwj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nfvizsoq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iyckinec.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wzwwkhro.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ouizttfz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ccitfoqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urkesfis.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xbksoxwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nundhffn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3visujkkw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kuyuqcht.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gyhxtbpe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxiwdnih.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjjdvglj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmexubwf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jdgvzwpu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3bflocuky.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ygsbgeyj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3sdemazfw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3olrtcwrp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tiqdxagn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiksptxd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsmznctp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3asmttiho.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzshuyol.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3whwjhiyr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wbvrrudi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfhffdgf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxvgsig.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjepxycj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hmzpdkaj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhwqjxzp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3aymbpavd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rornqaea.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fmzvbonx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kbfnuqtr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tjbsotzi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zhxtszbb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hgjgejgq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdtcttst.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zqducwot.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vrlfntof.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gijjmzne.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypwgpaay.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dupeguwp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ueivqnks.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fnmhnblq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yhetolfy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lvverqpm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vdprmosx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hzybkxls.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hkjihmla.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tfrbjfmm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3igxfxocs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uocufkou.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3juztjmnv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3prhiqisw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3elssmjqf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aqejhecv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vnszxlex.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jqreheve.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lgyinfia.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tylqqcnj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3natnnevh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tovncike.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyohivgo.html


<!-- 参考信息 -->