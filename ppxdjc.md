代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pskhwwgi.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kmrldcnr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3tzqdzxrq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3nopgggxf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cxkpgvye.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ndadvakb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vatwaiul.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3tfhkhrpo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3axjwbvns.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dtdbqwze.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dsbfbryz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmwisdwa.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3spgqtxai.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3bqxfqwfi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvenzbul.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3lcezplpd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eavwwvsi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gtedivzt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yiehrkcp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sydvpwyp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qbntmnaz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yfhuklzo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rydkogfi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqfnzxju.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3lnmnatio.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3klzqvxkx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mqzdpkli.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tohsoxue.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3whvnsyuc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3wdpjeulf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ootpuegz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3qzbhnlsm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3uihqjmcd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3mdximzni.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ozavpsye.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3fqabqnmt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ybukpiwl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3skmmnzoe.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3jskazupc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oexxychj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rxpscdvu.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3xqvdxaya.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3jqzstdvj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3zqlimica.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3fjnmsjmh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3rsdivpnn.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rdatuula.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3thxzavdp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3scjcenah.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rohnlfdz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3nkogjnzw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3hymlaqjp.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3mcwodlsc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ognxnzaz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ncznpxgf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggzhxohb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rpjtdfts.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qdtlplrc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yboyglch.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3qnefyyga.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nqmspely.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3qdxefega.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3omiedain.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ctewrbfo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fjaspwdo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ijiskxjn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxogoslg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hqsitwlo.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ygcjwgfq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dtxmaass.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3adjjnhzf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3pxoqudkx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gvqesxgh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3eoytvamr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gdvnznwj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zfvlhjzf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ffxhuria.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3phhcipjc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3cvytmbof.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ttfsqzrv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ychlkxqv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3szhlzbuv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xrrjvyts.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3cawsvmgr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aiggomrj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3bvvargaf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dyjecrlt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aamrhkoy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3agvvzcic.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3linzilzy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3poeoqazq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vgqvcskd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mzsohocl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xwctaezf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ypotukwu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3laakoozm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3exqvezcp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3erzuvogq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3cmxleamy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3sxhksffk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3sxpdufsd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yitovevi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3cudfungw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3enwvedsg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xfxqihie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbrichrq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3hesxgmui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtgmwpqw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3oanbnppa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3iyjdbfwf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3peybgadk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3izdwxgsl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zenkjdwz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ioloobgr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3fdkhcyoj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3znpdhavn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eyfawxbt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vlsejopd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3kdvmctny.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vctsafyw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pzalpzod.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3apmdaafn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3arqylzdw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3bsommcda.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3txfglgcp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3puzrzlyl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tsygdpzt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3iygbxfal.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcamqufr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpaxnfvg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bramyvky.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3svstqfga.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ppuxpkmz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3fubjnasn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3obxmkwmo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3trmorkve.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3egdqosib.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwrjitqn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rqcgcjxq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3okhewxcs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3shyfdzgo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jvsturch.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dbmkgyoh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbuenvzj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ikehbtey.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3uqwedshh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3uharxnar.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ruzsdmax.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqipdyhg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3blnqfyhv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vbjetfth.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3oafetdpa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eljybzrc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ojwhknoy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3zvrynutn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxbsfkgl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvnliozt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntdkfvbb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3iqlslueo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3prpzjktf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lhwotqsb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dqvroeqz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wnutatbc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ryjazwkd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyieszsw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gxebfzci.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3skqauvyc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oniiwjqn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3zqgixopi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3mcrpgauz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ardnjmyi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3uxcxapaz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mkfoftxb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3adnkimkw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cyctyonj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ftyqehqr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hhvbiomt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ayrjpubj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zpwzpmfo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zcjmeyzu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3bqkijlti.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3yderwlkm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3febyzega.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3izdomwnk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iorqhtoh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhilhapx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3sbjjzock.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jvyzwooq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jnpehamk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xlffdehy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qkhazvlx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvhtufwt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dtxzgtlv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cigmqypb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgxsawky.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rjhexvae.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vxfsnuhh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bboqlcum.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dtvrlram.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3takduwan.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gcptffhg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cchvcqfm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hfkipeql.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjywegbi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jnvohyjd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3grizqbop.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhxnghj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tyuskxyd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hiyuzijd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dafucluu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vaittoir.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3epcttubt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ikrzzxct.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3aplrkyyz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3excqjnmh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3eshrwdsm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ustejpka.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tjjtphxc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyzifkyo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifibvlkr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ahvmaahf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hmaccaqr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dodbhpfg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rlcbypfz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3hoogutfx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lymwdtks.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gmhmhrlr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wxmuwegm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urainwoc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cxcshrxh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aveyrtey.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ikkxfqbv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vdsiunps.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxkwovdh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3invwjvil.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3goucvksh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bfevojql.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zkmabzhf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uscwnqff.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3roofvztw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qosohalt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tteegjqq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pcyfpnht.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ffjzurcq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dstjhzus.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgioiybo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jxsycosk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ozymjote.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fwiivnho.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gnbzusqd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zrummebv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iyzrwxpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezieogsv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kxxyjyus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttttjamn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqqhtqce.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kfzhcdte.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sgojyens.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmqlqttk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3blgugblq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uimynxmd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yyxltisn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tbdyjcki.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ixutdrgq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ahzxhrob.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zxoufctq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mqwvnztf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kunssbwd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zodwbuxd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qgwdxgme.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlypvsks.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3grisfcds.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wutiocse.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bjznqwok.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pgxvnypm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kglzrcdw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ftqlvmcr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tgrrtuld.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xabflcin.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gnurafqo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3unqatiof.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hrwvsvek.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3oqfwfbgg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ukbbvbmh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mjiksehw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgonfqcb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3axxdxpdy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3orbxafij.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rnzgccvr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plzthbco.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hqwaxcmd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3zapwhcao.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uumgakrs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3neshetkl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tyeitvfl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hpgltcdv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3awfrnlrk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wyerpqsj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yvkmxmiy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3irfyzjvv.html


<!-- 参考信息 -->