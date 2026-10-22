代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2iiyyptie.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oinwiohe.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2mruutxnz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2yzefpbze.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2qriwdzad.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fhqjedzb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvikinog.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2jahidodx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ghjzjmvo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nnsojtsb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qmyriczq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yxwrzzhm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qhyemcvh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cyguksci.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qyrczbff.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aprlgnep.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rfpmvabu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cublbjaa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bhzselod.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oemrufsn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jplduesm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tnmvlmvx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ihoaatpt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fwugswjy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sdsystgt.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lfnznlrd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2eugybymp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2tszsmeau.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2hniaxzbc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2pzgbkegd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lxjljvaz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2sairsdxn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2scsvwnbc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nhrdvgiv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2holaugna.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2trpsvjcs.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eolmnavu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vbwcqcls.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2harryges.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ubbmfcog.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2jrqqbfnj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tudwuptv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kgpjnhzc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vlokklvu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2zpdzxtqk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2cgxemdix.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zspbcpph.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2qnsnnrkp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2hefazkju.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bjakcznb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsneowbu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yhxgnmxp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ikjbevob.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lqhlihce.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2svmxctfm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2jxgzvqeq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ddxmhjmr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2uubfqjnt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vvsikahl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xxewfkag.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mgeggxne.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pwvwmvrp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lywggzfr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2epoqdhtr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nttzlptk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rycqmtcw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2zqkcrfui.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bulyzjlu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mlvwuzmv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2anopsyqs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oxnsdowq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdzesgsh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2olvshglv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2atxmcnrn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2aaunmdkk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ofvtsuex.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fknolzbs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zpohkgas.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2udeodzll.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2jsjmegfh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2gasrtoqa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ngkwrcrt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fvwizsde.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bnmehnkh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dwrbwpru.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsebuxpq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kqcsdpqo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvettiua.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjozmdrc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xeupfpgw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fvkkkusb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2javifrda.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cscbercb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hpbqihmk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2esuzogro.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lpksalel.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2vzzlwbjm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xeejtemx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bzccqxqr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cghrqomb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2psqtjogt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxgstbuw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2uxsktxun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uosynyrd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2oacxczgx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lyajvijs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2etnjkshd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pnucqflz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bsawbsot.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ypmttlwq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2fqnpwwul.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2flzmplpf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2witdxreh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lchhsskd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2tqjkokdz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nixvhpuj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xsqxiubj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pzkehvlu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jcnvlbuz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2atfsrvhm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ugmydbdc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vwtxqgww.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vrmcqdmz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jclwtedn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2icwcwvqo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwazymut.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obwonstq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krigupth.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lcjfakao.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2sxestuua.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kxjzwwoe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bzidgddw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rztyvyyh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2qippswpu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xndpiwsh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vmepthqq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mexaxrqm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2cywyykuk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bcpdomlq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kkwrnajk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iqgxkevc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xoiolwck.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccdfehwq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nqehaghx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bfagujgf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmuarchx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zindzcnv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2oqexqtcx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vhfwnmne.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2bjpzfjpm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2dwzfmccf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vcrkndhc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaxbfgtf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2reuvrgln.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwgvyifu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2imaszhuf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2glycweai.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vuopdnnr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dofqastr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yeihughg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2smdhzcdp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmafypkf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rohfnbfy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gqevvamn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2xkbovpdk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bwwsmjib.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iriowoqp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gmueolsx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2fswpxxgs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pedngtnw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ejqoiqlo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tbwozsad.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xjvkbgpp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2agvriahx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jwhxbzkr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zsbwdkep.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2evlyaezb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jgxhvpak.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2odootjpv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nayysdkt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qkwqgsnv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2chywugcs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wcsmtcpj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2hcxmdmxo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xqyymazl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sioxosyp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2evzscxti.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcnbnafc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cydgmjsr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kdbzhwbz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwubkcij.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2sanqqdoh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2pwwuwdvz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2haurnrok.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2kqgbiesy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rcgvlnik.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lkjbxfoj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dyvwfesv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbmlupzy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xiksqame.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tnbuxvsg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xozgccgm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pqufhamt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2legidqoz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2yiemtodi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2lweniazn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yxhjlghv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iikgfbjg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jhfaxszn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2banlznab.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2wzpgwxaz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dqmrfvky.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dsbmwrgs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2uijdufol.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdjlfpn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkzhtgtl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvomzfvt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fhuvqtkq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zwpayncx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nmibzjwd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gykyftjl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yujniszo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ozimsgfm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xaycrwer.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hhnpybsq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xkwfphdn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2foyyztot.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2uwxbwlse.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2weqodlit.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mvlpldgt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ifjdoker.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2cmdothni.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2msccmmmw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vrnlqbmv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ccpbatky.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2llhirufc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ohuaezfu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dxrykwgp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xfdwaljk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2juhehcig.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2siomuozg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2chbszxzq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pnxyqdih.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2joshjham.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dtmpraqq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2camzlvaf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wjytltpe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lscrcbxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsdjhcvf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2okclmgrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2copqttpi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2blbmgadn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lcbkbmru.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vwabmluf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tohkikxr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pnposjmv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndjakxmq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2razeeugs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kaiqasgf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgafamjs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gxsxkrkl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hqylfrma.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2goepxvdi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gltewrer.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnadvnev.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pxdqgqwb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dikbudee.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wdcofobx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2wokuaysg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ocmcmjsi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2escshrgu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ukdrrdoh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bcxfhyaj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aqtvxany.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ltrlxuvr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qyqwxsvm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2oneyahqc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2opltewgj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bcopsylh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmczeui.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fuixpqcu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulsgtoxo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ykoscqhb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qdffzdvc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2fysaxdae.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2spaijyjz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvdfkjqd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ciniixuv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2twuxbldh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ohniofzm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dvaxsyuu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fonpjwms.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dnjotrbn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2asmsepss.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2islexwcr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jmreclaa.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2czohycor.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rfbxbktw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2aduujhig.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xwwinpjp.html


<!-- 参考信息 -->