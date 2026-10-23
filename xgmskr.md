代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wbwcxuzm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3disyypog.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dozxwtxy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3xdetigcp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ztfffzhm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fhlmpffj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksbrxtpr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3noobuhfp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wufqkewj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3naxnghtz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qmymmcpp.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3bwzipvun.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yigfbofh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mqozetym.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yyfsrxew.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mbggkyuc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ddtbttkb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ztusfgvd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jkhicabs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fcpchock.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3dagpibwg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nevdvitf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wksqforr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rzsdkgyd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gffpcljy.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3vxqxrnjb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xehqrhwg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3sfmbedzj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3yzjuklnx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hnzkpcqt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ybiefhbu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3wjhfmboi.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vbdycwae.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3cynfqesr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hntscnhf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kqctuwro.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ejhmmjcn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3eamngikg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wiclwjni.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ehnvqcxv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rolapsiq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bfgdxrny.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3urifxzow.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3bqrrcjbh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ihxaoznt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3otypdyyq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3pglmlcjf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3crwkagju.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hbahtaji.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yypvpqzl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rkwleras.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eelkxhzb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jmienakm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eescyxln.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3svezyabc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ugsrpdgx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3akmjxyci.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3fznikdvx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vqyrzncy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dvsywihg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3eildahoh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jdknshwx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3kgoqvytg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kjlbxyoa.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jjdisqtz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aqnedsqm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vihnuncd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzcbblnb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3iecpmnxz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eeuunpdm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ybmqscqd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aaifhscc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mfrucpvf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3sbcnagel.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3resckayr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3yxfxajvg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ixgdzvxm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3eupbmmzk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3grseuxxo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ehktvapo.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fxvlgpml.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qmcncuyi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sxtbdmgp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3brxysdty.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3gdrwkvjf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3nplxnpqt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ostsazbt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ukowxlaq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3abzrwdjp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3anzgnrut.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3sasdfiec.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3iruhncen.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3dwwfsdqb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3mzbnxoqx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ndfgbuwo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tvkoaqtm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pseiqlgi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mjgzhlpl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fiobxcjm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3izjvisgz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rigzmwbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckiweezy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yuoyfnqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdteoxis.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3uefutxwa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vczorddb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdccvpfs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nngkvekg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3adlmzviq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wplwthxh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wfpkddug.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3imytsahl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3etnmahay.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3nqxqtqdh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3aokyswki.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kjfamcwr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kungxxxj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vlactafb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3doualrlc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zwgorqrx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3tqnygjgq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zhnoojto.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mzhjasqc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3luufnuxx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpgzpfsq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3smfsfwzf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pzsrrbcv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fkoszgat.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zblacvko.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3aiopsrqd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3afkgpcel.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hzbulpyz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yxvmgacx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bpwifbye.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ncryrxxm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zmgzzqsw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3uqctbcku.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kavofabm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hdvippxk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dirggjve.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mpwgpwjq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ojzdutwh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3upptepnz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cjiaegmv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nuqyuekv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygkancem.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rpfqnrdn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wtdaglcv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvsymgot.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wynzambx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3glvwlkga.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spdadrrm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ncrarcnx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vdnkqaaw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3eeaswxjp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gsohjkba.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tksnjmxn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bkumgkau.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3dhlhogeh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qryxjktu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ytdmvzmn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvtkfepw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3brwmqshu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbnivmmq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ughgkaio.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3svddwvce.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqjarpxa.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zxqwenhi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bhhldoxn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ccjjayxn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jbduuqbk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rjcdsndu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rxekcucc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ztrocasp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3liepsior.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hjgfqfnh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3cftuwtwc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mbztzwoc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3svkyydte.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3djisescy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkiezljw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iauswuie.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pzbtraxs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xqgfmzrd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjhajtyi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dszrtotl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sghtrobl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3htkivctd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jujrcxfi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jbounxop.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckgfydbe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ycdycycf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rokxanmz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3smckqbvk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ozkptvvc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sgfcsjid.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qjtssumg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mzjltomb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ieceeyrt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rpcgcdnh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3edcgpdyn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ieojnbin.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3tzjqecbi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lccrzdna.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lblgntwd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cwntszba.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vzahknzp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3khsdbuum.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gdplesuw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3goydvaqr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3dxwoktzy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tfpgeisp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yucjsxti.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rrxrkmfw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3feticjsu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3etdaifcp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uvetokjl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3axvtpsuw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xprlaygq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3isvbgamk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gbobolba.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wsyohgcc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3txuunbzq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3onkvzrdj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ungocoib.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hplrzqfm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yjwrvyit.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tuwruyxk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hmpepgjj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxzqksft.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3szpmlmze.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bcharxpf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3drpuxbdj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uxmyibtq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xhpydvnt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yesvapxh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tsfspwqu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fzhpaqav.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nenjtmuj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ogdduhee.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3sdnivtub.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3opbmeaam.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gctsusyf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ddqjxtim.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kpidswcv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwrhgnk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zgiwjxtx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vsrlrnad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sppayien.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mwhrzkaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etsqgpgl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gjzftyhg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rgxvkcfg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3akvcmzbd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mrjokplw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hkyhbngb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqppdxgr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jgwfsspc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3gwaaafki.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwguviko.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zmybqcvl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3dvzuizoo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xsgsshzg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dmjxkycz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibcrftba.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bsoljmzg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3clyuokmz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bwoaldej.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mqyfofbu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3amfzaokl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3myfmmuzt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kkjbkyzg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nyfdgpux.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrynfpwi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqtddato.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lmkzgcey.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3sudwjxam.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3dlwvlceu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hdzjuwix.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qtxvaitr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3noicmccj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bzvrmdol.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vqllyudd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3gpftuwaa.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3msmijkae.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brevpqtv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmotisev.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pzgjinfz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mtpclnch.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3riiniact.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xzymirnt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rypmkyvv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ffbjkyzq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mvwmoxub.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rlhmpclz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ylkciwzk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jxzkxnlq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qrinmsnc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3joznusrb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sixmvjsm.html


<!-- 参考信息 -->