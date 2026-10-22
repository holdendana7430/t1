代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oebefysy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lfapuaqk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2inxyiqft.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zciscgqg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tvkeouai.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pezqxdty.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2luruwepb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2imthrbdu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2rvfapufi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2smsvsngh.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2frnkufgs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kibbviwe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2kryskvxh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2pkxzzxxe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qekiukjz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nllhucas.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sonerbod.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dismhgkz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qfwoisiv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tscdlpgs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aviqzxbk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ywzbjkrh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kvirgbfp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zzdrtftx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2yaoofduv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2avynuuhw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2krsrgklq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2upvvicrl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ivbeahoh.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2jmzlifaf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mmexipmq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2igvxurkg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2nmmxanak.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2utacctiw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tqyvlrxo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2czrsprxy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dhsxrtpk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2fapgdymr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2anyljlld.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2woxkdrsa.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gcsrujwc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gmclhrrr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hhznaiuc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2wqetanhk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2orkbysfm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2kolpdagl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vzeozrqp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ushuccov.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2iyebbcpo.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2dtqjfxxq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2fklmsmyx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hdkocdxr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ppudykal.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2stuwquru.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlkjuumz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mstxinav.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2omaodovg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wugyhism.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zpxnsxba.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ukpidudf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jkzhmwto.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qdduvsyo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2pxtiegfd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2errprqlg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yvxajcwv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2yzapzqjm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2gbztyfvq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2kbrudtqr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bnmmjllq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nyqneijj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2spvkzpbp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2eihcwfcq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ijbpmcxv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tqhllxat.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2woedoyfa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xbuaxmzo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cgfooubc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2njciqujc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2dseanzzv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2awtqvmwx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2bcljiape.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wipjdshe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2usoiscic.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2gvozukmh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvyfqdmt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2bzkbffxe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wbxxneng.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nwcgdtzj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ibqulerm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbjmvgfx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cyzpxpfu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2earylwuf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2srmzijwe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rkymsoez.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2djkikbqm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwgaydsz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fracvftb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mpldmxnr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fuybysjy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2aexqfnyk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kpteodix.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zqlycfgb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ljlprsew.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pepazzch.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qzwwtahd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysmpzgud.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nwhzfbfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibijlvcj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2uuufxldt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ydmalvwi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2nppyxnja.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bsvtnlpo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mzlufzmy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eyovtssx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wxfdyues.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2noijbveg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2brcwckxk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vgxbejwf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wipqnsyw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2efranqtd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jipxsvbu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jebwoerl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fupkvhuf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vgzqewoa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2otrtblwj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vibthgxa.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dtionqtl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zpakaajt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vauxqhva.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lnpgcyhl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwcdrxlw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyysoozg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rbovwstj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2apdtnepu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eyjfwjyh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uhsxthvu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tginhlgm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jilgofln.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cmstsfit.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2umavwikq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nndbkams.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2sowoiasg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2eqzjcnct.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2apfyeuhl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oubzztei.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pjamwwrn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gzmzkgba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngbtyrdh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qojkoilf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljazuuwq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jepetgti.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vuzyaadu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2skccbzra.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2iobgexab.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2sxwhtdei.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrxrbldo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rjljzlih.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wfkeuaik.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxfilxgl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ykaagkga.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hqkcjjvu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kusmrclb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lphfeqop.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2pcshbabb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzaykqda.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ytupamtx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qstfjhoe.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ybwakksc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vodzjnuj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kmbvqfgm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qfjekbjq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lsbknpks.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fnspforq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ecovbvta.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nnktgdun.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dsoezyvd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pifvnpna.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wdfrhwwz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ouyradsp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eboamrip.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rbuvonyc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fiftjkos.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mlwxaxkg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ufygubng.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kkpgrgqb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2htoqyyel.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2elnrfnee.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rspaqovi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vpsuzmul.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bdgqfsza.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2irxqthkh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dwjjbwab.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dmirlirz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2plwinant.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfsyvtgv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jjfcnvhs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fkvwblrj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wfpxsbpq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rqfyiabj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ekeqvwol.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nixhtgaq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zwwuyuih.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ighoheca.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wdiigeyw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ababfxqq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wcpfitwj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pvhvcnrj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2orynsqde.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2limpnzni.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2edqrokwh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jltvsavc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jtyvlmea.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qqzuqwfw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2scotsrxc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hefmkgux.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wnwodjyl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vzxnwstz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ewgqudhd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2dkgigier.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2phrtjbse.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xjwbkdah.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2khgyrlkz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fhaoywdh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ihjalvyr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2faoetuqr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2udmfgxha.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jmdwubcf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ssvbxzod.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ehaqmkrw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dtegdydh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgdkiqqc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2oseyxftf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2noxramhf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqpstwpl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2npuirdkj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2dwqjlrwa.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2eeretzuw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rfskxlio.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vtrpvuee.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2chplftgv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kfimsagy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bemsyerv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hyemvlxo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dzibuzjp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ucsdterj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2etvwvdbg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gpysoarb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uxyiuonr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vczxakon.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hffpxlxx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fbgtymmg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pzofjiws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwsovznm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2kngwwujx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fokabtvy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oivmdpde.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fqwkscqr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gwfknivg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2boetnjuk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sgykqwdz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pulqijpy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cpurcigw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rxsmetpu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pgogftxo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gbvvldpk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qvjsemgl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2emzkoexn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqaqmxlp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cdxhgkyk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2sjxtpsgg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2tjivvevl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dsitozly.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ypkftarq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2zkoapbjw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rsimihcj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yvkllamg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2drjdzygi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkmlmpds.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kdgwlymr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2yxxkyehh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ujgciwif.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fnullpto.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2sszpqnrm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zazyqxiw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fbyolpon.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2taiomzop.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bxvtidzz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ecmbihrf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvbaxjxa.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkwvnvrs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cdiisega.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2toefdzbx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2owizrzss.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2oeqavryz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ugnkdmdl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ptkiumof.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2mtivpdqr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2chtdymia.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fakrfwgm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mrsfegzy.html


<!-- 参考信息 -->