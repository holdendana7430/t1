代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rpiutzkd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lxyjznie.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssszdouw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhkqnoui.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3xubredcf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bzvhckhe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dllrxhgs.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3grehblau.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxaummuf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qhtglvjt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wycptpzz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pfzlvgeu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jcluapsp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uloouicg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3smyoufwe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pjukjylp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ozvjmzmm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nizckccj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kyestqdq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yavvwvyr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cwsaggiu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3utmjdxww.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zpozwdfi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xupxmphl.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3dfrouquc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ohvdxxts.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cedzjcar.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xizpofvc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3waknleew.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nhrkqbjx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3qiqyciwk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3deqtyhbx.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3icrpxtnm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3rowoypqk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rjvilftf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3lplelrup.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lvulvkuc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hqkzousb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3venrxyrs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ugdaodgc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tyqvdnco.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ncnstpzs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3jmfcgrjo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3slcyxuyd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3prtbvzsd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3psiueyeu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3deruenwe.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3crlljobo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qnktfkei.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3glblbfax.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gcthxfum.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3orevagup.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rogwcmxg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3inyahogt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3drauoypy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3toiwxxys.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3trljxiyi.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nydzbwms.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmwtixjb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pvvkxnjq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pzwknyxo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vneeechc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ernxdwtu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3idtsaofv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3erppivgm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hzbvpcxt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ddrprnni.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gehghgyo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vsuoxpfb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dlylmrfw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3cipscbjv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3qihzfyek.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3azforsej.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ncphiqzw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fwnnihjg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3rpwpsxmb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cwctcpqe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cfnyswbg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mucguivf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wzqesfln.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3gcjqorca.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjmgxkkh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjseihrq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uiiwdcqz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jyppozms.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3eflzhdaz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3vzocgyrm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wokqawpr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ruxcjozi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hhdcsmos.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3grgekuox.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pjldygwf.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3twosarvh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pvdrpfjl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xyszfmid.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ucoxkkzq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bscniqpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvqkkogu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xzilynjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbbqsaqg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ydgvtmsg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mghdegfb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3qmtxswyv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rkxpwnvv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dgakfrha.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sqhwmuqu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3odqqxxww.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3zyfovtty.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tsgaibmf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vuniwxab.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jvmbndex.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfzjkgmn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rwnnbzoa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3evvmrkdb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ywhdeyzd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3apwxuxdx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kugcfgio.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ogiccaln.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rgsmgqze.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qnbseooj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wzolcqnc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imyzvtxd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnsvzqxj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nghvcrmc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3eijxjnhq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3jojhonhg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hpwlpgps.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pypcjvgu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qmowwofm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjztfdlr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpadzyvf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlghvmlt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zrdzwugn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qiltzngp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kiswnymc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3uchnbahj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qomklbcn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3bydyytlf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bziynphi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxmoeibd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dtxurddt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zlchwzxq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tkdobdzj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yzfbshvo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxazlavl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3oofqkyun.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jjucbfcv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pgbbpuuf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3agotkbbu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3exmogwlb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfffipfb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rukcyhel.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3piiejhrs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fffjtbcu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ocbanlsq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3sxlmkedu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ukgwkeus.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxuhsxnb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpbhuzey.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rcrwanfj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xivdibzd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lsqmgqen.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pqmovzuq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bnqgzbzi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3lblctfrn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vzrgysjc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dfyvkhvj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sjualmdn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kjvwkobn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kfvmkehi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jswobgis.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3skwgdpek.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ebkkelvn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mxdvrqmj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dhgdawze.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqnqdmht.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yegqbvwf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xppelmpz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oemyofcq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3sicsehrz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jogbrmfq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zchybxlx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3oppvamtp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckbuffrr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pdogiyoq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xotkbxns.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdeoifwv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3htlututt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3aoqzrgir.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vretywvk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ufypbmep.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3igfnddfk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3blkictdv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3snhygzwf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gbfxlarh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wdlvcgxm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mqdwvjog.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hwlqxfgr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3tegrmvxn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cnqdrphk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3afqgcvol.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ttxecbtx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zegfiyom.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wvuihiuk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xibbfban.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3eaiqhpey.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mhfzqldc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ajybjxsp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3huozzxka.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3bhggofyy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsyoubhk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhmnnjic.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3avyvudok.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bwfpkbmb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3slnsxmzr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lrcawpuk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3iewpiely.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3krexwcvc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hdmfusod.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kyrzqrnq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qcqtiotk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kyabkogg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xqaapbrg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qdhqnwtp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xgmdzvyx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdrenfcs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zdbtpkgt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ivhlozsj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mziqrrfb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3coyqrtuz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ifjkioqm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dnesxbgg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kfvhhfcf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ammlcorg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lekfucob.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3etiijlum.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3foagxqkj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdgjwfhd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gexqxkwy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aumizlse.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3acywkzcf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ikstbblo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3imtdrnyz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bodmvpld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvovbijt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dtjzvzps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjbpmmjf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rumbjcen.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iqedbxlw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hyaqumpm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouchkaew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkyzsbcm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cibchmxa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3skvyifww.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3enuhditn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3asxxrasc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zvyavfsn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3avuwnvtj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vztfbdjo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mnrmrdlf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzmtujtj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3pynomees.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wyvlcjpk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zjicqoyp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hpeoimpp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rpufnyfg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3frvvjcjr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hcxogiif.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxirnxov.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxneyccj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3smgxsnyo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3dnoyrzuk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tcpwlfpy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xewvghkt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vckhrace.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3frrutkyp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3lkrjattt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmbhrgnj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yhtwgnqj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gwskhpvo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3expzmhky.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xedunjxv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ojdzibvj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3sfyenjck.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qfivnukl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3usfnraor.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pmkdvtre.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fbmexpzf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3lsgttdap.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eojiomnb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3wqmytoju.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3yrvkqpfv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3azwyqddv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3iovelysm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3aveduaiz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ppcpynhx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tkwkmbpm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ncdvaryq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mjuzpaom.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nnydbjib.html


<!-- 参考信息 -->