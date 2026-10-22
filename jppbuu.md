代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2vdwubcxz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2sjkcunhq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zzzptyih.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2xnzwompi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2edewdesa.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qmtluesd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbjaxjch.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nduuvwnv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ytpfkfmy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bwdsglqi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2axkbfrxo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zjqhpvnq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ukxgalse.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yqssnori.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2gzovlfts.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wsocgyem.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rtoxsvok.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2lpkkhhaa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ncwketlo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ozcwxwgl.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2msspiltt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2cjaqtjft.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pvcirmtv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wtqheccs.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kmmcvssl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2oveznhsw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2uhmfancs.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jtlnpprd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zsuygrjo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ehtuwfah.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2diwuzpza.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xewvbemz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2kniylswl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2erptblac.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2uigqxsjm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2wvnfhbvf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qmyfkouc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xlfbzslu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2xatwhuwm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2tbzmbzkv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zkccpgrl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2usegnffj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oxiduret.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fihofiij.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bpdtqtrw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2epeittof.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mssqsyyk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kzoexrba.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vbbbteyb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zbsbounk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nplyhncf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wlyyjdce.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gkjfddas.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2amjuknjo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fjvysucz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kivlbbnk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vcxlofbq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qtvmvtaj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lngmzyhj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2mhwgxsxt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yfatzflv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wqrxhgks.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2khanutma.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwptssny.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xvnjptlm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2kfofkpes.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2euvyhazh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2lrwvbpyd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvzgpbfe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gkvpwhye.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lyaujqnp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2prwntbfe.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2bdaawnft.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2gojnoyup.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wpluktzz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2griwrgui.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2vjoeaonk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jemgmnko.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mkmvmxhv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvfouzuf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcwwxmjd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fmkthmlc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2huuqbgte.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtmyrci.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2oncaccqi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kfnzflch.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2pdcaehml.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yxicbvcj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2dbwiyptk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmajrxm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2xmonwcks.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ohrrkrqa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2psvmiygl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebvhwygv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mlbazlyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmcrlzam.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2anolgies.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2juuidcrz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvjcvizv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2carjcrnh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lnmfzudu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rkltvter.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ljqliagk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2unmlwqba.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gdiqxwra.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2mfruxqvn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2sdpapcmp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkgsxihc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ctgygyji.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cxovfvsg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dtvecese.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2oloyfmql.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xnojqida.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dxecxbba.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2scssoibq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pwkrovlq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2weqrszbf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujpdztbr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yshifanp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yaszdsdk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2htbiamrv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2glxyqjol.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hsdelcjl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mhmbzlxb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mxlpokrc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2vumlaioy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xejcgaza.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqsqdewq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxkjdllu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rfgjfblf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ewpkdans.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2aeizbxwt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gqwoipqd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ieyxtvvp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fenhhttb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2revwwmhp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhegbwpu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mzsjgylp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xayxldvc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gdatqmxb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ykwcpjnw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2qjnwugtk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bmurhqde.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfdcsoyn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptenfmso.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cukcfrpp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcelakzy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yceiasgi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2iupewwip.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldfhzkxy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2sxjaekoh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ymhpobbt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mopnnxlc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndjymgmc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ibqcadam.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvefjfxb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2olhgjxts.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnpweoev.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnlapvny.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2umqfrses.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wpiofcsz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tumrilin.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2adrgnjca.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vifvdgwa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dvsqvnbs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jafbcjvc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zgxquisg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mgfsaijq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2epilyqji.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qhgzjtuu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqgabyam.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydpindos.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2quaxpneo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztudfjen.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ccflefhi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ddzkhcrt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mewenyll.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pwfonghw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bgkgmdrk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tinahmdl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bcrpnnds.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dexfovxf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbccxknq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pzfmvper.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmkeaak.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2phyckjim.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2itdnvury.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2svpxutrq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mstglgwz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dizcirkw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ltfksgng.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tzrzmjss.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cwylyxkt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ugzwphid.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wznxbhcp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bsqxhqrj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2notfjsnf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2cnirhqfk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pyfegnvi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bsfoaixb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mlchprgz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2czbqqywz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wfmlhzvo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2bmobcxen.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ijpuupdr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tjezchhv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gcmrpfsn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqopmfyt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qnqthwcy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xneqzwpo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2puezcyuy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wqazykyo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2waujhmqc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2awnpcmag.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2thfbwalk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2aiqhgsbv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvrcsldq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxyfybda.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irilfrzj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2irkprink.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2czgfdzeo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xfqktztl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ncngypmr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vwhqwyof.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2azuavffg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xcienmys.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hnpriofx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qqaaqnbg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oardxium.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fpeaycrn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zuipljaq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2aqwakcov.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2fqiaolkn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyytvsrh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ovvnbvws.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qfohyfns.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hhhifwyo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ouevbujr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xrpswusx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nrqvruhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aszukgxs.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hguzfiyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keyuvvqi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hstppvqm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eddjqiaz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2leceeurb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljofvfrc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kjfcchof.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppdphxhw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cjpiqsjp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xwsqnvvv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sjtqrvgo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvwutsfi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2gunnxauh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2cgkcguod.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijhidywi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2clbmfmwb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2yytmdvyo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2sfpsjpte.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vfctlfgj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hrimqbyw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2icuduggr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ulvcrxfr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2jusylzpf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvcqoorl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjhnikcr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hzrdwalf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qirldzew.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2asiemrgn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jgzwjgwq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2xetyycko.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ojfqqehs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ydvqouwb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ysmpstzf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2btkujcub.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2tnyjxwaw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kvzaxhhd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sfsdehsa.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aajcxzax.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ykmaugnt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2udtmohdq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wwmjzqix.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cxrwbbgz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fjuhjmnl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2saatcyzw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ncgkwuac.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2awduutzr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rmgfyfsf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2uyubrnpd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vqirgjpz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ncwbygvu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nvmwenhe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qdooweot.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2bojeluwq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2agzxybff.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wutclxql.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xpmrjrqa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hovuytvy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rezzkzno.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dixwhxkv.html


<!-- 参考信息 -->