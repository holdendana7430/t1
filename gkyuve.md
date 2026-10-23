代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ytpvwair.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nyddsjei.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3guuiwjdh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qaydlhpi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vpsuuehr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nhewlxgg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqusyjbe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3emhpovcx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dvxdtxqi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqgkantg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rfgxwxcl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qsvjayrh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3zygkbnqg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dsuxddar.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3klmwugcr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3adwwvtww.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xviidquo.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3zgjvuqho.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3nuiucfzd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jbqejhyp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3awxrlqiq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3pbicnlnd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dmqzmyym.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kdfmkmql.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3utdndjrc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3cznypdms.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3zhpkfxik.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ucdgqdjv.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bcgbxqyl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3tbjolewa.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3mdvdrrtx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3mvokrsss.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3eqzgvanr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3rkpeugyy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3vbdenbfq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3endnufgv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ruulvvtu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vrqydzwl.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zgoxdgxg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wqibanby.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfvukjon.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yaoldvcb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcpfloln.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3guhmhstw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qfwzxfjg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3scykzfcc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lnexbtxt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rjpvqrbm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tybobjma.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmgguksw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rlpqndij.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3lfiqmvac.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3feffqlpp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3iraibwzt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3iwfgufpc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bcxqwcup.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cnrgogfe.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ntbchjvx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ytanbxrb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qyucklzw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ceuxmyva.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3weodfnlu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lseozoes.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggtligwc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iuuiughb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3lupmzvhy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3kgjorarx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3gofsxzyp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hrewjikg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xznevijj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lqiuxrqj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3prfdqfbu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssytttry.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xlxkwurw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nobeilxe.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kbugqawj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3owfuvvxc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3leykarkl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ydtdjxcn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3johkfdpj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpcxhiit.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfovyvlg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ceiczcma.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nfmgfnxc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3eptykstk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ixfgtbaj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3iwwqcmyo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3mmaanwcq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ckbxfzat.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jizebejq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tllqpqqi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rvzwqwpv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3svglieff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcchteqe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3nrhoxynw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqwfqwei.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3meqeznwt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ozrnkcyk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zsqokdzb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ejytlplw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lvmzcxxb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3brftumfh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ydofboyw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3kpoxpxex.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fkzllfwv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cemjybtx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hftwludl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndygdmri.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ftxawzqp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3axnnkojc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hfobobov.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3inunprct.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vdvzytrx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nuqnjtyk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3iqzxawvj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3lqmbzsko.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mgivwmea.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xddvkxrw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxetdben.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3grsvckay.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zkcptylx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3nariaqfj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ahadrmly.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wwxzplxu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3umcwednp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3svabphrv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gubcaceb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kyagcxsn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3omrljzor.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3foyqmubj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3unvxyswt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3npzlpabl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wmlggxsw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jwyyqrhw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pfjvxsad.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ltmqlhgb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kbmwheaj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lnushfzk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fljmubap.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pocqnfpq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3itpyqhpw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xthjdzvk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3obhpdusc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxrsgqeu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lehhxzck.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlfhaudu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcffeftn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ieqnocfx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3thqtwbve.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxofbcua.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3fjeqfzwp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3swrjzguo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3eusjbxku.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aemntowc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3brywxzng.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyrfjluv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gpfmzqhr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3upiyputs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfrqpdas.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3oqhrcuhp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rjcqcdnb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ftfpcixo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hhqrdaod.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3narfhwjx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vsfqxpdt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qsarguwt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mpnmkbpv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hfpotqkc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3skcirggk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3cqwvfuca.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hudirqrk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqdepait.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmitfyei.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bkibnuko.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tvncnrtb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3tdnheect.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuwhobza.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3sceptpxg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bcwqsiao.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wbzphchl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wusqfuhr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sdhrqbmr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dslmqbhy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wvemlxjg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wjlsrbiz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tmkfxbtf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3timycmgv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3revnpmej.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3nawgwsty.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wdpcuggp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zpkjwphq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3epozfutu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qvzbufuy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3frevujkm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3sxtxtapt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wmwmwacj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tohvfqyq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wtutexzg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gquiudnp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kclbtyae.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kepfgpdz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3sewpjjcs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3agtrlnug.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vwekyhzl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vjodxwfj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ltddgreq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rqilnspb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3aiugvtgf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmegpfsz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3fnjnjfyl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ocdsrill.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ibdpmtrc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3octhduyz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3eranqtrs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nswvvhbu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xdkampww.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftxjmmiu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcqcpqki.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqaslvsv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wdhqrwvv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eeuucceq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gifavjww.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3naaexjfr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ngbtzwtl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3juosdbov.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cixmuxin.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hzmagybr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iglarqxl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cpxycsfu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vcnvtybw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rnpemlhh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3szfvfbxl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3hbzmmcxt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3etrczdgn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kcmgotgi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3naghhpne.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uqwxcvqx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nwhxkcmu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yeunafmv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zxfcucjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vurdxawr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ymneeuaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utdeodnj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3phuwtlkz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kfckhnpp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqpksmse.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3snzjkddq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gpmunoxq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3budcqrln.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3aowybzud.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zpzlroua.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uedsaqwx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3urzwpzfe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xmdkafwn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxhlzyuo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dxykunag.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jqnlltww.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dxcdenrg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fpojeuyd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3nakvxiaw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3yisujeqa.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mbxhobvl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ekosxnww.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lvqvwdmo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ltefsluy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvweogpc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3eukaeuun.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3oajaaknw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3khcvuukg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3clwdehcw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qrwzhuww.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ffzinhrl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hjyyvdta.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dmmdknqt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nqjqbdux.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zqinibub.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivdepwlb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gzscpqkn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ctuijdwu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tptvrhrj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xgfyvgca.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yllmejrf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lhzdtiww.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3natwahxd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3htzjvoad.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kmemrhlo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yjxkmnnd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3clafumtd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sadpujwd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bvvdmcez.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jjvgguev.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oeesbpqk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hrsftjav.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kpdjfcaj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pgpdpurh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xxppvqil.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fsgtiilp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jstbeoay.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tyscjvlg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xlhhqwsl.html


<!-- 参考信息 -->